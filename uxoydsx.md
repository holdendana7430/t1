代发 wailian999

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://fb.shxzskj.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://ec.shtwfgs.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ny.colortex.cn

[P08] 处理浮点精度问题
来源：http://ws.muxihuayi.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://fr.asd995.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://am.colortex.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mj.muxihuayi.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://cm.haigaiapp.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://on.yuntaijiaju.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://nm.wgjwhj.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://oi.yuntaijiaju.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://af.jctech888.com.cn

================================================================================
来源：http://qm.chemitech.net.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://yu.bjjhwx.cn

================================================================================
来源：http://fh.asd995.cn

[Q01] 创建表
来源：http://cm.wgjwhj.cn

CREATE TABLE users (
来源：http://lv.jianghongdianzi.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ua.muxihuayi.cn

name VARCHAR(50) NOT NULL,
来源：http://xv.nszjky.cn

email VARCHAR(100) UNIQUE,
来源：http://gj.nszjky.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://xr.shxzskj.cn

);
来源：http://cc.haigaiapp.cn

[Q02] 创建带外键的表
来源：http://ee.huanxung.cn

CREATE TABLE orders (
来源：http://or.huanxung.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://eu.muxihuayi.cn

user_id INT NOT NULL,
来源：http://hp.521024.cn

amount DECIMAL(10, 2),
来源：http://ma.szsharing.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://io.9csxet.cn

);
来源：http://fr.bookmarksfly.cn

[Q03] 增加列
来源：http://sq.newstarts.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://vq.hahajie.cn

[Q04] 修改列类型
来源：http://ie.yuexingan06.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://sg.asd995.cn

[Q05] 重命名列
来源：http://dm.jctech888.com.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://qx.nszjky.cn

[Q06] 删除列
来源：http://ky.jctech888.com.cn

ALTER TABLE users DROP COLUMN age;
来源：http://aw.yuexingan06.cn

[Q07] 删除表
来源：http://fo.hahajie.cn

DROP TABLE IF EXISTS orders;
来源：http://wx.panjiajie.cn

[Q08] 创建普通索引
来源：http://af.huixinmuqiang.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://oa.shxzskj.cn

[Q09] 创建唯一索引
来源：http://yz.colortex.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://yj.shtwfgs.cn

[Q10] 插入单行
来源：http://zl.huixiangedu.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://zn.huanxung.cn

[Q11] 一次插入多行
来源：http://lv.lnxyls.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://xr.jianghongdianzi.cn

[Q12] 插入后取自增 ID
来源：http://hr.panjiajie.cn

INSERT INTO users (name) VALUES ('C');
来源：http://yu.lnxyls.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://yp.muxihuayi.cn

[Q13] 忽略重复插入
来源：http://ei.muxihuayi.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://la.yuntaijiaju.cn

[Q14] 存在则更新（upsert）
来源：http://wx.bjjhwx.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://pl.yuexingan06.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hw.wgjwhj.cn

[Q15] 查询全部
来源：http://it.szsharing.cn

SELECT * FROM users;
来源：http://yd.newstarts.cn

[Q16] 查询指定列
来源：http://rq.colortex.cn

SELECT id, name FROM users;
来源：http://mw.nszjky.cn

[Q17] 条件查询
来源：http://jx.wgjwhj.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://zu.yuntaijiaju.cn

[Q18] 模糊匹配
来源：http://br.lnxyls.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://xn.bjjhwx.cn

[Q19] 范围查询
来源：http://wi.nszjky.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mx.shxzskj.cn

[Q20] IN 列表
来源：http://ce.panjiajie.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wq.huixiangedu.cn

[Q21] 空值判断
来源：http://jg.chemitech.net.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://ys.colortex.cn

[Q22] 排序
来源：http://we.shxzskj.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://jc.huanxung.cn

[Q23] 分页
来源：http://yv.wgjwhj.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://bw.panjiajie.cn

[Q24] 去重
来源：http://fw.szxytkj.cn

SELECT DISTINCT city FROM users;
来源：http://xt.hahajie.cn

[Q25] 只取前 N 条
来源：http://fr.chemitech.net.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mk.colortex.cn

[Q26] 计数
来源：http://sq.huanxung.cn

SELECT COUNT(*) FROM users;
来源：http://mp.asd995.cn

[Q27] 条件计数
来源：http://ya.hnjuh.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://za.lnxyls.cn

[Q28] 求和与平均
来源：http://gq.huixinmuqiang.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://xk.haigaiapp.cn

[Q29] 最大最小值
来源：http://rt.yuexingan06.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://nn.asd995.cn

[Q30] 分组统计
来源：http://rt.huixinmuqiang.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://jt.asd995.cn

[Q31] 分组后过滤
来源：http://mq.szsharing.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://uc.huixiangedu.cn

[Q32] 分组拼接字符串
来源：http://vy.panjiajie.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://tb.9csxet.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://zb.haigaiapp.cn

[Q33] 多列分组
来源：http://ow.huanxung.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://sg.shtwfgs.cn

[Q34] 每组取第一条
来源：http://ym.szsharing.cn

SELECT * FROM (
来源：http://gm.9csxet.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://rz.muxihuayi.cn

) t WHERE rn = 1;
来源：http://ln.huanxung.cn

[Q35] 内连接
来源：http://nl.haigaiapp.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://lf.nszjky.cn

[Q36] 左连接
来源：http://fd.shxzukj.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://xz.haigaiapp.cn

[Q37] 右连接
来源：http://cb.huanxung.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://jl.lnxyls.cn

[Q38] 全外连接（PostgreSQL）
来源：http://dj.panjiajie.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://lw.gzmigu.cn

[Q39] 自连接（查上下级）
来源：http://lh.shxzukj.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://wj.bookmarksfly.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ij.wgjwhj.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://pp.huixinmuqiang.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://oj.wgjwhj.cn

[Q41] 多表连接
来源：http://rr.521024.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://cw.yuntaijiaju.cn

JOIN users u ON u.id = o.user_id
来源：http://ht.hnjuh.cn

JOIN products p ON p.id = o.product_id;
来源：http://fh.bjjhwx.cn

[Q42] 连接条件附加过滤
来源：http://rj.hnjuh.cn

SELECT u.name, o.amount FROM users u
来源：http://jp.yuntaijiaju.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://qc.newstarts.cn

[Q43] 标量子查询
来源：http://vi.jctech888.com.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://ax.shxzukj.cn

[Q44] IN 子查询
来源：http://jc.9csxet.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ua.bookmarksfly.cn

[Q45] EXISTS 判断存在
来源：http://wd.9csxet.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://eu.haigaiapp.cn

[Q46] NOT EXISTS 判断不存在
来源：http://jr.jianghongdianzi.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://vs.asd995.cn

[Q47] 与平均值比较
来源：http://yq.hnjuh.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://cu.lnxyls.cn

[Q48] CTE 公用表表达式
来源：http://wt.lnxyls.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://do.hnjuh.cn

SELECT * FROM t WHERE c > 5;
来源：http://ky.muxihuayi.cn

[Q49] 更新单行
来源：http://zx.colortex.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://oh.9csxet.cn

[Q50] 批量更新
来源：http://wa.hahajie.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://lo.521024.cn

[Q51] 用子查询更新
来源：http://fb.yuexingan06.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://ag.hahajie.cn

[Q52] 删除指定行
来源：http://ap.huixinmuqiang.cn

DELETE FROM users WHERE id = 10;
来源：http://ej.hnjuh.cn

[Q53] 按条件删除
来源：http://al.haigaiapp.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://zi.9csxet.cn

[Q54] 清空表
来源：http://jd.huanxung.cn

TRUNCATE TABLE logs;
来源：http://by.haigaiapp.cn

[Q55] 排名（并列占位）
来源：http://iq.huixiangedu.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://pg.szsharing.cn

[Q56] 密集排名（并列不占位）
来源：http://ox.nicolike.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://eo.huixinmuqiang.cn

[Q57] 行号
来源：http://ia.huixinmuqiang.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://lg.huixinmuqiang.cn

[Q58] 累计求和
来源：http://om.chemitech.net.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://cl.muxihuayi.cn

[Q59] 分组内累计
来源：http://gb.shxzskj.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://vi.wgjwhj.cn

[Q60] 取上一行 / 下一行
来源：http://jg.521024.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://qg.hahajie.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wo.panjiajie.cn

[Q61] 移动平均
来源：http://me.shxzskj.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hf.asd995.cn

[Q62] 分组占比
来源：http://fx.wgjwhj.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://dx.hahajie.cn

[Q63] 开启事务
来源：http://wy.muxihuayi.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://cz.bookmarksfly.cn

[Q64] 提交事务
来源：http://ih.jctech888.com.cn

COMMIT;
来源：http://iu.szsharing.cn

[Q65] 回滚事务
来源：http://hj.colortex.cn

ROLLBACK;
来源：http://me.yuntaijiaju.cn

[Q66] 行锁查询
来源：http://ib.hnjuh.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://tn.colortex.cn

[Q67] 设置隔离级别
来源：http://yz.lnxyls.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://jc.jctech888.com.cn

[Q68] 保存点
来源：http://qk.shxzukj.cn

SAVEPOINT sp1;
来源：http://xz.haigaiapp.cn

ROLLBACK TO sp1;
来源：http://yj.huixinmuqiang.cn

[Q69] 查看执行计划
来源：http://sh.lnxyls.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://vf.hahajie.cn

[Q70] 更新统计信息
来源：http://oj.chemitech.net.cn

ANALYZE TABLE users;
来源：http://ue.huanxung.cn

[Q71] 查看建表语句
来源：http://el.huixinmuqiang.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mi.521024.cn

[Q72] 查看索引
来源：http://iy.yuexingan06.cn

SHOW INDEX FROM users;
来源：http://de.muxihuayi.cn

[Q73] 查看表状态
来源：http://ln.nszjky.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://lv.gzmigu.cn

[Q74] 强制使用索引
来源：http://fm.nicolike.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://kp.jianghongdianzi.cn

[Q75] 日期格式化
来源：http://dt.hnjuh.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ha.panjiajie.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://kx.nicolike.cn

[Q76] 按天统计
来源：http://fm.muxihuayi.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ue.jianghongdianzi.cn

[Q77] 时间加减
来源：http://fx.bookmarksfly.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://gn.bjjhwx.cn

[Q78] 当前时间
来源：http://di.chemitech.net.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://dj.chemitech.net.cn

[Q79] 字符串拼接
来源：http://fk.shxzukj.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://je.jctech888.com.cn

[Q80] 字符串截取
来源：http://bi.szxytkj.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://aa.lnxyls.cn

[Q81] 字符串替换
来源：http://ra.huanxung.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://dz.yuntaijiaju.cn

[Q82] 字符长度与字节长度
来源：http://zq.bookmarksfly.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://lh.haigaiapp.cn

[Q83] 大小写转换
来源：http://an.huanxung.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://jh.shxzskj.cn

[Q84] 去除首尾空格
来源：http://jc.huixinmuqiang.cn

SELECT TRIM(name) FROM users;
来源：http://jy.shtwfgs.cn

[Q85] 数值取整
来源：http://qm.shxzukj.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://og.hahajie.cn

[Q86] 读取 JSON 字段
来源：http://if.jianghongdianzi.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://tv.muxihuayi.cn

[Q87] JSON 字段做条件
来源：http://hf.lnxyls.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://rb.shxzukj.cn

[Q88] 行转列（条件聚合）
来源：http://cq.newstarts.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://kq.bjjhwx.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://xc.huanxung.cn

[Q89] 判断表是否存在
来源：http://vg.colortex.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ow.chemitech.net.cn

[Q90] 生成序号列
来源：http://jv.nicolike.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://qo.bookmarksfly.cn

================================================================================
来源：http://uu.hnjuh.cn

R. Bash 专题
来源：http://gu.huixiangedu.cn

================================================================================
来源：http://uy.gzmigu.cn

[R01] shebang 与严格模式
来源：http://wx.jctech888.com.cn

#!/usr/bin/env bash
来源：http://rr.521024.cn

set -euo pipefail
来源：http://ye.hahajie.cn

[R02] 变量赋值与使用
来源：http://dv.szsharing.cn

name="Tom"; echo "$name"
来源：http://af.nszjky.cn

[R03] 只读变量
来源：http://ao.shxzukj.cn

readonly PI=3.14
来源：http://sd.colortex.cn

[R04] 位置参数
来源：http://ay.jianghongdianzi.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://vm.nicolike.cn

[R05] 参数默认值
来源：http://dv.panjiajie.cn

name="${1:-default}"
来源：http://ny.jianghongdianzi.cn

[R06] 判断命令是否存在
来源：http://sb.huixinmuqiang.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://uh.shxzukj.cn

[R07] if 判断文件
来源：http://lw.szsharing.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://vz.szsharing.cn

[R08] 数值比较
来源：http://wx.9csxet.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://cn.panjiajie.cn

[R09] 字符串比较
来源：http://qq.nicolike.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://bj.newstarts.cn

[R10] 正则匹配
来源：http://ky.jianghongdianzi.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://us.huixiangedu.cn

[R11] case 多分支
来源：http://gd.asd995.cn

case "$1" in
来源：http://hx.wgjwhj.cn

start) echo "启动" ;;
来源：http://ul.lnxyls.cn

stop)  echo "停止" ;;
来源：http://iq.chemitech.net.cn

*)     echo "未知命令" ;;
来源：http://bg.asd995.cn

esac
来源：http://rd.haigaiapp.cn

[R12] for 遍历文件
来源：http://ab.asd995.cn

for f in *.txt; do echo "$f"; done
来源：http://vj.wgjwhj.cn

[R13] for 计数循环
来源：http://qf.colortex.cn

for i in {1..10}; do echo "$i"; done
来源：http://cl.nszjky.cn

[R14] C 风格 for
来源：http://aa.panjiajie.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://my.yuntaijiaju.cn

[R15] while 逐行读文件
来源：http://dt.shtwfgs.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://cc.yuntaijiaju.cn

[R16] until 等待条件
来源：http://dd.521024.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://an.huixinmuqiang.cn

[R17] 数组定义与取值
来源：http://bd.yuntaijiaju.cn

arr=(a b c); echo "${arr[0]}"
来源：http://aw.hnjuh.cn

[R18] 遍历数组
来源：http://nw.haigaiapp.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://vz.shtwfgs.cn

[R19] 数组长度
来源：http://mt.huixiangedu.cn

echo "${#arr[@]}"
来源：http://eh.huixinmuqiang.cn

[R20] 关联数组（字典）
来源：http://sj.gzmigu.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://vs.nszjky.cn

[R21] 字符串长度
来源：http://tm.shxzukj.cn

echo "${#s}"
来源：http://mn.shxzskj.cn

[R22] 截取子串
来源：http://fj.521024.cn

echo "${s:0:5}"
来源：http://zq.szsharing.cn

[R23] 字符串替换
来源：http://mo.colortex.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://na.colortex.cn

[R24] 大小写转换
来源：http://jp.huixiangedu.cn

echo "${s^^}"; echo "${s,,}"
来源：http://xv.yuexingan06.cn

[R25] 去后缀 / 去前缀
来源：http://et.jianghongdianzi.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://as.jianghongdianzi.cn

[R26] 命令替换
来源：http://xq.shtwfgs.cn

now=$(date +%F); echo "$now"
来源：http://sc.huixiangedu.cn

[R27] 算术展开
来源：http://du.asd995.cn

echo $((1 + 2 * 3))
来源：http://nt.haigaiapp.cn

[R28] 浮点运算
来源：http://ss.colortex.cn

echo "scale=2; 10/3" | bc
来源：http://fj.hnjuh.cn

[R29] 定义函数
来源：http://rr.gzmigu.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://tq.chemitech.net.cn

[R30] 函数返回状态码
来源：http://lg.chemitech.net.cn

f() { return 0; }; f || echo "失败了"
来源：http://ba.bookmarksfly.cn

[R31] 局部变量
来源：http://el.yuntaijiaju.cn

f() { local x=1; echo "$x"; }
来源：http://xn.haigaiapp.cn

[R32] 参数个数校验
来源：http://qx.hahajie.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mu.bjjhwx.cn

[R33] 捕获错误并提示行号
来源：http://tt.9csxet.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ks.jctech888.com.cn

[R34] 退出时清理
来源：http://vv.yuexingan06.cn

trap 'rm -f "$tmp"' EXIT
来源：http://ug.bjjhwx.cn

[R35] 后台执行并等待
来源：http://yq.nszjky.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://uf.shtwfgs.cn

[R36] 并发执行多个任务
来源：http://kd.wgjwhj.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://xb.huixiangedu.cn

[R37] 把输出赋给变量
来源：http://wd.chemitech.net.cn


<!-- 参考信息 -->