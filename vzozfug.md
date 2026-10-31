代发 wailian999

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ep.shxzskj.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://ns.bjjhwx.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://xv.shtwfgs.cn

[P08] 处理浮点精度问题
来源：http://vr.hahajie.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hn.huixinmuqiang.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mg.hahajie.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://zz.haigaiapp.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://fq.yuexingan06.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://al.szxytkj.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ez.haigaiapp.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://bq.bjjhwx.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://lf.shtwfgs.cn

================================================================================
来源：http://sy.hnjuh.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://xp.shtwfgs.cn

================================================================================
来源：http://bf.bookmarksfly.cn

[Q01] 创建表
来源：http://hq.huanxung.cn

CREATE TABLE users (
来源：http://rq.gzmigu.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://oc.jctech888.com.cn

name VARCHAR(50) NOT NULL,
来源：http://ps.shxzskj.cn

email VARCHAR(100) UNIQUE,
来源：http://lm.huanxung.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://nc.nicolike.cn

);
来源：http://sa.huixiangedu.cn

[Q02] 创建带外键的表
来源：http://pl.haigaiapp.cn

CREATE TABLE orders (
来源：http://uh.asd995.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://oc.shxzukj.cn

user_id INT NOT NULL,
来源：http://tt.nszjky.cn

amount DECIMAL(10, 2),
来源：http://ru.asd995.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mx.gzmigu.cn

);
来源：http://hp.panjiajie.cn

[Q03] 增加列
来源：http://nf.huixinmuqiang.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://gy.shtwfgs.cn

[Q04] 修改列类型
来源：http://su.yuexingan06.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://uk.szxytkj.cn

[Q05] 重命名列
来源：http://ed.szsharing.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://qj.colortex.cn

[Q06] 删除列
来源：http://ai.nszjky.cn

ALTER TABLE users DROP COLUMN age;
来源：http://bk.newstarts.cn

[Q07] 删除表
来源：http://yv.yuntaijiaju.cn

DROP TABLE IF EXISTS orders;
来源：http://sb.panjiajie.cn

[Q08] 创建普通索引
来源：http://lu.huixinmuqiang.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://qp.haigaiapp.cn

[Q09] 创建唯一索引
来源：http://ze.wgjwhj.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://to.chemitech.net.cn

[Q10] 插入单行
来源：http://lm.chemitech.net.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://jy.hnjuh.cn

[Q11] 一次插入多行
来源：http://rn.shxzukj.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://sj.9csxet.cn

[Q12] 插入后取自增 ID
来源：http://kg.bookmarksfly.cn

INSERT INTO users (name) VALUES ('C');
来源：http://nz.muxihuayi.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://zo.panjiajie.cn

[Q13] 忽略重复插入
来源：http://uv.huanxung.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://nn.9csxet.cn

[Q14] 存在则更新（upsert）
来源：http://bl.521024.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hc.panjiajie.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://xy.szsharing.cn

[Q15] 查询全部
来源：http://rw.nicolike.cn

SELECT * FROM users;
来源：http://fu.szsharing.cn

[Q16] 查询指定列
来源：http://vz.huanxung.cn

SELECT id, name FROM users;
来源：http://xq.szxytkj.cn

[Q17] 条件查询
来源：http://gy.muxihuayi.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://rn.panjiajie.cn

[Q18] 模糊匹配
来源：http://jd.bookmarksfly.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://au.huixiangedu.cn

[Q19] 范围查询
来源：http://mu.bookmarksfly.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://nk.jianghongdianzi.cn

[Q20] IN 列表
来源：http://ry.szsharing.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://il.chemitech.net.cn

[Q21] 空值判断
来源：http://rp.jctech888.com.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://ej.colortex.cn

[Q22] 排序
来源：http://gd.yuexingan06.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://qa.panjiajie.cn

[Q23] 分页
来源：http://rc.chemitech.net.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://da.bjjhwx.cn

[Q24] 去重
来源：http://lp.panjiajie.cn

SELECT DISTINCT city FROM users;
来源：http://zt.wgjwhj.cn

[Q25] 只取前 N 条
来源：http://rj.haigaiapp.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://oc.panjiajie.cn

[Q26] 计数
来源：http://ag.szxytkj.cn

SELECT COUNT(*) FROM users;
来源：http://kr.bjjhwx.cn

[Q27] 条件计数
来源：http://ft.shtwfgs.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://az.hahajie.cn

[Q28] 求和与平均
来源：http://rs.shxzukj.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://zl.yuexingan06.cn

[Q29] 最大最小值
来源：http://rp.bookmarksfly.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://yp.shtwfgs.cn

[Q30] 分组统计
来源：http://qx.yuntaijiaju.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ie.newstarts.cn

[Q31] 分组后过滤
来源：http://hk.shtwfgs.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://vt.shxzukj.cn

[Q32] 分组拼接字符串
来源：http://uy.shtwfgs.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ye.nicolike.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://qy.newstarts.cn

[Q33] 多列分组
来源：http://sr.yuntaijiaju.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://el.panjiajie.cn

[Q34] 每组取第一条
来源：http://mz.wgjwhj.cn

SELECT * FROM (
来源：http://ig.gzmigu.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://cw.szxytkj.cn

) t WHERE rn = 1;
来源：http://fp.bookmarksfly.cn

[Q35] 内连接
来源：http://qz.gzmigu.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://xs.newstarts.cn

[Q36] 左连接
来源：http://sq.haigaiapp.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ap.chemitech.net.cn

[Q37] 右连接
来源：http://fd.shtwfgs.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://eu.huixinmuqiang.cn

[Q38] 全外连接（PostgreSQL）
来源：http://ie.yuexingan06.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ro.bookmarksfly.cn

[Q39] 自连接（查上下级）
来源：http://we.haigaiapp.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://zi.huixinmuqiang.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://nv.haigaiapp.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://rb.jctech888.com.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://qf.huixiangedu.cn

[Q41] 多表连接
来源：http://kr.asd995.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://hb.hahajie.cn

JOIN users u ON u.id = o.user_id
来源：http://ar.huanxung.cn

JOIN products p ON p.id = o.product_id;
来源：http://sn.9csxet.cn

[Q42] 连接条件附加过滤
来源：http://pd.shxzukj.cn

SELECT u.name, o.amount FROM users u
来源：http://hq.hahajie.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://yq.wgjwhj.cn

[Q43] 标量子查询
来源：http://az.bookmarksfly.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://rr.hnjuh.cn

[Q44] IN 子查询
来源：http://sw.hahajie.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://os.szsharing.cn

[Q45] EXISTS 判断存在
来源：http://dq.nszjky.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://qg.muxihuayi.cn

[Q46] NOT EXISTS 判断不存在
来源：http://vz.huixinmuqiang.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wv.shxzskj.cn

[Q47] 与平均值比较
来源：http://by.shxzukj.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://iz.shxzukj.cn

[Q48] CTE 公用表表达式
来源：http://qi.chemitech.net.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://cd.szxytkj.cn

SELECT * FROM t WHERE c > 5;
来源：http://fg.hahajie.cn

[Q49] 更新单行
来源：http://qv.yuntaijiaju.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://zs.jctech888.com.cn

[Q50] 批量更新
来源：http://nl.haigaiapp.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://ee.colortex.cn

[Q51] 用子查询更新
来源：http://gi.jctech888.com.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://uh.bjjhwx.cn

[Q52] 删除指定行
来源：http://vo.nszjky.cn

DELETE FROM users WHERE id = 10;
来源：http://xp.huixinmuqiang.cn

[Q53] 按条件删除
来源：http://oh.huanxung.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wh.9csxet.cn

[Q54] 清空表
来源：http://zx.colortex.cn

TRUNCATE TABLE logs;
来源：http://am.muxihuayi.cn

[Q55] 排名（并列占位）
来源：http://kw.yuntaijiaju.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://rm.gzmigu.cn

[Q56] 密集排名（并列不占位）
来源：http://nh.bjjhwx.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ng.9csxet.cn

[Q57] 行号
来源：http://oh.huixinmuqiang.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://sz.wgjwhj.cn

[Q58] 累计求和
来源：http://lt.bookmarksfly.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://al.colortex.cn

[Q59] 分组内累计
来源：http://ki.jianghongdianzi.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://sf.hnjuh.cn

[Q60] 取上一行 / 下一行
来源：http://ra.colortex.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hi.muxihuayi.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://sh.jctech888.com.cn

[Q61] 移动平均
来源：http://ud.haigaiapp.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hb.newstarts.cn

[Q62] 分组占比
来源：http://tj.huixinmuqiang.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://rm.521024.cn

[Q63] 开启事务
来源：http://rp.bjjhwx.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://hd.hnjuh.cn

[Q64] 提交事务
来源：http://am.bjjhwx.cn

COMMIT;
来源：http://yf.gzmigu.cn

[Q65] 回滚事务
来源：http://yc.hahajie.cn

ROLLBACK;
来源：http://wy.panjiajie.cn

[Q66] 行锁查询
来源：http://mt.huanxung.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://qi.huanxung.cn

[Q67] 设置隔离级别
来源：http://ja.muxihuayi.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://yh.huixiangedu.cn

[Q68] 保存点
来源：http://gj.9csxet.cn

SAVEPOINT sp1;
来源：http://lf.521024.cn

ROLLBACK TO sp1;
来源：http://oy.hahajie.cn

[Q69] 查看执行计划
来源：http://ir.jianghongdianzi.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://bf.szxytkj.cn

[Q70] 更新统计信息
来源：http://bs.yuntaijiaju.cn

ANALYZE TABLE users;
来源：http://qy.nicolike.cn

[Q71] 查看建表语句
来源：http://cm.huixiangedu.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ug.szxytkj.cn

[Q72] 查看索引
来源：http://uf.521024.cn

SHOW INDEX FROM users;
来源：http://le.colortex.cn

[Q73] 查看表状态
来源：http://hv.bjjhwx.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://up.huixinmuqiang.cn

[Q74] 强制使用索引
来源：http://ov.asd995.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://rx.shxzukj.cn

[Q75] 日期格式化
来源：http://vv.jctech888.com.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://xf.newstarts.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://vq.nicolike.cn

[Q76] 按天统计
来源：http://ak.shxzskj.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hh.huixiangedu.cn

[Q77] 时间加减
来源：http://kh.nszjky.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hg.chemitech.net.cn

[Q78] 当前时间
来源：http://dt.muxihuayi.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ar.shxzskj.cn

[Q79] 字符串拼接
来源：http://ss.jianghongdianzi.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://kj.lnxyls.cn

[Q80] 字符串截取
来源：http://po.colortex.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ig.gzmigu.cn

[Q81] 字符串替换
来源：http://yv.shxzskj.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ia.huixiangedu.cn

[Q82] 字符长度与字节长度
来源：http://ov.yuntaijiaju.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://sr.gzmigu.cn

[Q83] 大小写转换
来源：http://vu.wgjwhj.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://pe.hahajie.cn

[Q84] 去除首尾空格
来源：http://to.gzmigu.cn

SELECT TRIM(name) FROM users;
来源：http://yo.hnjuh.cn

[Q85] 数值取整
来源：http://ny.wgjwhj.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mk.shtwfgs.cn

[Q86] 读取 JSON 字段
来源：http://nh.asd995.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://fg.newstarts.cn

[Q87] JSON 字段做条件
来源：http://xv.yuntaijiaju.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hu.bookmarksfly.cn

[Q88] 行转列（条件聚合）
来源：http://sc.bookmarksfly.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mh.yuexingan06.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://qn.szxytkj.cn

[Q89] 判断表是否存在
来源：http://sb.panjiajie.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ko.chemitech.net.cn

[Q90] 生成序号列
来源：http://iq.szxytkj.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ok.chemitech.net.cn

================================================================================
来源：http://hp.szxytkj.cn

R. Bash 专题
来源：http://ks.huixinmuqiang.cn

================================================================================
来源：http://kl.colortex.cn

[R01] shebang 与严格模式
来源：http://su.shxzskj.cn

#!/usr/bin/env bash
来源：http://eh.huixiangedu.cn

set -euo pipefail
来源：http://tt.nicolike.cn

[R02] 变量赋值与使用
来源：http://bt.muxihuayi.cn

name="Tom"; echo "$name"
来源：http://tr.wgjwhj.cn

[R03] 只读变量
来源：http://td.lnxyls.cn

readonly PI=3.14
来源：http://xo.9csxet.cn

[R04] 位置参数
来源：http://rn.huixinmuqiang.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://jd.bookmarksfly.cn

[R05] 参数默认值
来源：http://ja.shxzskj.cn

name="${1:-default}"
来源：http://xg.colortex.cn

[R06] 判断命令是否存在
来源：http://ks.panjiajie.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://io.shxzskj.cn

[R07] if 判断文件
来源：http://jm.huixiangedu.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://aa.yuntaijiaju.cn

[R08] 数值比较
来源：http://fm.gzmigu.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://qd.jctech888.com.cn

[R09] 字符串比较
来源：http://gj.nicolike.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://re.shtwfgs.cn

[R10] 正则匹配
来源：http://bz.jctech888.com.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://cf.jianghongdianzi.cn

[R11] case 多分支
来源：http://bs.shxzukj.cn

case "$1" in
来源：http://ia.newstarts.cn

start) echo "启动" ;;
来源：http://lb.hahajie.cn

stop)  echo "停止" ;;
来源：http://mg.huanxung.cn

*)     echo "未知命令" ;;
来源：http://ks.haigaiapp.cn

esac
来源：http://hz.bookmarksfly.cn

[R12] for 遍历文件
来源：http://lv.huanxung.cn

for f in *.txt; do echo "$f"; done
来源：http://zq.newstarts.cn

[R13] for 计数循环
来源：http://vb.szxytkj.cn

for i in {1..10}; do echo "$i"; done
来源：http://ze.hnjuh.cn

[R14] C 风格 for
来源：http://bg.panjiajie.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://cf.nicolike.cn

[R15] while 逐行读文件
来源：http://wf.colortex.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mu.huanxung.cn

[R16] until 等待条件
来源：http://zx.szsharing.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ax.gzmigu.cn

[R17] 数组定义与取值
来源：http://hw.yuntaijiaju.cn

arr=(a b c); echo "${arr[0]}"
来源：http://ae.haigaiapp.cn

[R18] 遍历数组
来源：http://vg.nicolike.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://kv.hnjuh.cn

[R19] 数组长度
来源：http://ju.bjjhwx.cn

echo "${#arr[@]}"
来源：http://tw.asd995.cn

[R20] 关联数组（字典）
来源：http://yg.huixiangedu.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://zg.panjiajie.cn

[R21] 字符串长度
来源：http://pz.huixiangedu.cn

echo "${#s}"
来源：http://fi.9csxet.cn

[R22] 截取子串
来源：http://uj.nszjky.cn

echo "${s:0:5}"
来源：http://vd.shtwfgs.cn

[R23] 字符串替换
来源：http://qm.colortex.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://tw.haigaiapp.cn

[R24] 大小写转换
来源：http://kz.shtwfgs.cn

echo "${s^^}"; echo "${s,,}"
来源：http://eb.jctech888.com.cn

[R25] 去后缀 / 去前缀
来源：http://xi.szxytkj.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://pn.bookmarksfly.cn

[R26] 命令替换
来源：http://wj.jianghongdianzi.cn

now=$(date +%F); echo "$now"
来源：http://ap.colortex.cn

[R27] 算术展开
来源：http://eb.haigaiapp.cn

echo $((1 + 2 * 3))
来源：http://iq.newstarts.cn

[R28] 浮点运算
来源：http://su.panjiajie.cn

echo "scale=2; 10/3" | bc
来源：http://bh.nszjky.cn

[R29] 定义函数
来源：http://kw.nicolike.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://xg.nszjky.cn

[R30] 函数返回状态码
来源：http://fv.colortex.cn

f() { return 0; }; f || echo "失败了"
来源：http://ft.bjjhwx.cn

[R31] 局部变量
来源：http://bs.nicolike.cn

f() { local x=1; echo "$x"; }
来源：http://mu.muxihuayi.cn

[R32] 参数个数校验
来源：http://cg.bjjhwx.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://yk.chemitech.net.cn

[R33] 捕获错误并提示行号
来源：http://cv.huanxung.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://oj.huixinmuqiang.cn

[R34] 退出时清理
来源：http://eu.huixinmuqiang.cn

trap 'rm -f "$tmp"' EXIT
来源：http://lk.bjjhwx.cn

[R35] 后台执行并等待
来源：http://tj.hahajie.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://ob.haigaiapp.cn

[R36] 并发执行多个任务
来源：http://ug.asd995.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://as.chemitech.net.cn

[R37] 把输出赋给变量
来源：http://xb.wgjwhj.cn


<!-- 参考信息 -->