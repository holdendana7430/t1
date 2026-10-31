代发 wailian999

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://dl.nszjky.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://xa.szxytkj.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://yd.lnxyls.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://zo.panjiajie.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://fl.szsharing.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://tf.wgjwhj.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://xq.lnxyls.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ch.jianghongdianzi.cn

================================================================================
来源：http://nt.bjjhwx.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://id.nszjky.cn

================================================================================
来源：http://bm.shxzskj.cn

[Q01] 创建表
来源：http://he.wgjwhj.cn

CREATE TABLE users (
来源：http://oh.szsharing.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://vx.muxihuayi.cn

name VARCHAR(50) NOT NULL,
来源：http://pn.gzmigu.cn

email VARCHAR(100) UNIQUE,
来源：http://lh.jctech888.com.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://xn.huixinmuqiang.cn

);
来源：http://oz.szxytkj.cn

[Q02] 创建带外键的表
来源：http://gj.gzmigu.cn

CREATE TABLE orders (
来源：http://kj.nszjky.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://rt.panjiajie.cn

user_id INT NOT NULL,
来源：http://db.huanxung.cn

amount DECIMAL(10, 2),
来源：http://zu.jianghongdianzi.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://xm.huanxung.cn

);
来源：http://bb.asd995.cn

[Q03] 增加列
来源：http://eu.bookmarksfly.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://jv.lnxyls.cn

[Q04] 修改列类型
来源：http://tz.muxihuayi.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://jb.szxytkj.cn

[Q05] 重命名列
来源：http://zp.jianghongdianzi.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://gg.muxihuayi.cn

[Q06] 删除列
来源：http://sa.newstarts.cn

ALTER TABLE users DROP COLUMN age;
来源：http://zf.chemitech.net.cn

[Q07] 删除表
来源：http://ex.nszjky.cn

DROP TABLE IF EXISTS orders;
来源：http://jg.shxzskj.cn

[Q08] 创建普通索引
来源：http://ar.huixinmuqiang.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://sk.shxzukj.cn

[Q09] 创建唯一索引
来源：http://uv.wgjwhj.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://oe.wgjwhj.cn

[Q10] 插入单行
来源：http://kn.hahajie.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://cj.huixinmuqiang.cn

[Q11] 一次插入多行
来源：http://pl.panjiajie.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://rq.asd995.cn

[Q12] 插入后取自增 ID
来源：http://ps.panjiajie.cn

INSERT INTO users (name) VALUES ('C');
来源：http://fr.shtwfgs.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ze.shxzskj.cn

[Q13] 忽略重复插入
来源：http://zw.yuexingan06.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://di.huixinmuqiang.cn

[Q14] 存在则更新（upsert）
来源：http://rv.hahajie.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://yv.lnxyls.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://gm.bjjhwx.cn

[Q15] 查询全部
来源：http://qa.jctech888.com.cn

SELECT * FROM users;
来源：http://ch.9csxet.cn

[Q16] 查询指定列
来源：http://ca.hnjuh.cn

SELECT id, name FROM users;
来源：http://gx.gzmigu.cn

[Q17] 条件查询
来源：http://dd.panjiajie.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://pz.9csxet.cn

[Q18] 模糊匹配
来源：http://cn.bjjhwx.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://xr.shxzskj.cn

[Q19] 范围查询
来源：http://me.gzmigu.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://qg.szxytkj.cn

[Q20] IN 列表
来源：http://ep.521024.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ob.chemitech.net.cn

[Q21] 空值判断
来源：http://xf.521024.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://nj.yuexingan06.cn

[Q22] 排序
来源：http://fr.521024.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ng.shtwfgs.cn

[Q23] 分页
来源：http://pf.chemitech.net.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://vw.colortex.cn

[Q24] 去重
来源：http://ys.hahajie.cn

SELECT DISTINCT city FROM users;
来源：http://eo.szxytkj.cn

[Q25] 只取前 N 条
来源：http://gu.haigaiapp.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://kg.yuntaijiaju.cn

[Q26] 计数
来源：http://xs.shtwfgs.cn

SELECT COUNT(*) FROM users;
来源：http://zg.bookmarksfly.cn

[Q27] 条件计数
来源：http://is.jianghongdianzi.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://lo.huixinmuqiang.cn

[Q28] 求和与平均
来源：http://tj.haigaiapp.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://re.muxihuayi.cn

[Q29] 最大最小值
来源：http://sy.gzmigu.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://vv.nicolike.cn

[Q30] 分组统计
来源：http://tq.nszjky.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://si.szxytkj.cn

[Q31] 分组后过滤
来源：http://el.nicolike.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ya.szsharing.cn

[Q32] 分组拼接字符串
来源：http://uu.yuntaijiaju.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://pp.nszjky.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://et.panjiajie.cn

[Q33] 多列分组
来源：http://sb.bookmarksfly.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://xh.szsharing.cn

[Q34] 每组取第一条
来源：http://zu.huixinmuqiang.cn

SELECT * FROM (
来源：http://ld.shxzukj.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://xg.colortex.cn

) t WHERE rn = 1;
来源：http://nn.lnxyls.cn

[Q35] 内连接
来源：http://lr.newstarts.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://qr.gzmigu.cn

[Q36] 左连接
来源：http://gz.haigaiapp.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wb.shtwfgs.cn

[Q37] 右连接
来源：http://ms.huixinmuqiang.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://cw.huixiangedu.cn

[Q38] 全外连接（PostgreSQL）
来源：http://ke.gzmigu.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://md.szxytkj.cn

[Q39] 自连接（查上下级）
来源：http://yb.huanxung.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://mx.bjjhwx.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://zu.szsharing.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://fi.shtwfgs.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://is.hahajie.cn

[Q41] 多表连接
来源：http://ds.yuexingan06.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://dq.521024.cn

JOIN users u ON u.id = o.user_id
来源：http://kt.bookmarksfly.cn

JOIN products p ON p.id = o.product_id;
来源：http://xu.nicolike.cn

[Q42] 连接条件附加过滤
来源：http://am.jianghongdianzi.cn

SELECT u.name, o.amount FROM users u
来源：http://iu.yuexingan06.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://dm.muxihuayi.cn

[Q43] 标量子查询
来源：http://kq.huixinmuqiang.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hd.panjiajie.cn

[Q44] IN 子查询
来源：http://rw.hahajie.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://xm.lnxyls.cn

[Q45] EXISTS 判断存在
来源：http://xo.521024.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://pa.newstarts.cn

[Q46] NOT EXISTS 判断不存在
来源：http://nu.jctech888.com.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://su.colortex.cn

[Q47] 与平均值比较
来源：http://ge.bjjhwx.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://fy.lnxyls.cn

[Q48] CTE 公用表表达式
来源：http://qa.9csxet.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://la.yuntaijiaju.cn

SELECT * FROM t WHERE c > 5;
来源：http://ib.lnxyls.cn

[Q49] 更新单行
来源：http://db.haigaiapp.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ye.asd995.cn

[Q50] 批量更新
来源：http://tm.colortex.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://lr.bjjhwx.cn

[Q51] 用子查询更新
来源：http://vk.newstarts.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://fh.panjiajie.cn

[Q52] 删除指定行
来源：http://sc.bookmarksfly.cn

DELETE FROM users WHERE id = 10;
来源：http://ov.huixiangedu.cn

[Q53] 按条件删除
来源：http://wl.shxzskj.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://aw.bookmarksfly.cn

[Q54] 清空表
来源：http://gt.gzmigu.cn

TRUNCATE TABLE logs;
来源：http://ce.nicolike.cn

[Q55] 排名（并列占位）
来源：http://zy.hnjuh.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://xm.jctech888.com.cn

[Q56] 密集排名（并列不占位）
来源：http://hj.shtwfgs.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://sy.gzmigu.cn

[Q57] 行号
来源：http://bf.hahajie.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://zp.9csxet.cn

[Q58] 累计求和
来源：http://iz.colortex.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://to.asd995.cn

[Q59] 分组内累计
来源：http://zn.shxzskj.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ak.chemitech.net.cn

[Q60] 取上一行 / 下一行
来源：http://gw.9csxet.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ip.9csxet.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ty.szsharing.cn

[Q61] 移动平均
来源：http://gg.nszjky.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://fh.yuntaijiaju.cn

[Q62] 分组占比
来源：http://fd.wgjwhj.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://xh.9csxet.cn

[Q63] 开启事务
来源：http://il.chemitech.net.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://hw.9csxet.cn

[Q64] 提交事务
来源：http://hy.huanxung.cn

COMMIT;
来源：http://tf.shtwfgs.cn

[Q65] 回滚事务
来源：http://qa.shtwfgs.cn

ROLLBACK;
来源：http://vs.hnjuh.cn

[Q66] 行锁查询
来源：http://on.yuntaijiaju.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://cz.asd995.cn

[Q67] 设置隔离级别
来源：http://fn.jctech888.com.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ym.shxzskj.cn

[Q68] 保存点
来源：http://ys.szsharing.cn

SAVEPOINT sp1;
来源：http://bm.asd995.cn

ROLLBACK TO sp1;
来源：http://po.bookmarksfly.cn

[Q69] 查看执行计划
来源：http://hx.shtwfgs.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://vj.nicolike.cn

[Q70] 更新统计信息
来源：http://if.shtwfgs.cn

ANALYZE TABLE users;
来源：http://mt.huanxung.cn

[Q71] 查看建表语句
来源：http://ud.shxzukj.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://kd.9csxet.cn

[Q72] 查看索引
来源：http://rd.huixiangedu.cn

SHOW INDEX FROM users;
来源：http://jp.huixinmuqiang.cn

[Q73] 查看表状态
来源：http://fn.lnxyls.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://iq.nicolike.cn

[Q74] 强制使用索引
来源：http://vf.bjjhwx.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://jn.shxzskj.cn

[Q75] 日期格式化
来源：http://ay.gzmigu.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://nh.asd995.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://rn.bjjhwx.cn

[Q76] 按天统计
来源：http://np.yuexingan06.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://lh.colortex.cn

[Q77] 时间加减
来源：http://iy.chemitech.net.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ka.szsharing.cn

[Q78] 当前时间
来源：http://gd.shtwfgs.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ix.nicolike.cn

[Q79] 字符串拼接
来源：http://db.huixinmuqiang.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://qs.newstarts.cn

[Q80] 字符串截取
来源：http://dp.huixiangedu.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://qb.chemitech.net.cn

[Q81] 字符串替换
来源：http://oc.huixinmuqiang.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://on.huixiangedu.cn

[Q82] 字符长度与字节长度
来源：http://ar.newstarts.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://su.nszjky.cn

[Q83] 大小写转换
来源：http://wj.hnjuh.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hh.lnxyls.cn

[Q84] 去除首尾空格
来源：http://ub.muxihuayi.cn

SELECT TRIM(name) FROM users;
来源：http://dz.szxytkj.cn

[Q85] 数值取整
来源：http://dq.yuexingan06.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://il.newstarts.cn

[Q86] 读取 JSON 字段
来源：http://uf.muxihuayi.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://nv.newstarts.cn

[Q87] JSON 字段做条件
来源：http://gl.newstarts.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://px.shtwfgs.cn

[Q88] 行转列（条件聚合）
来源：http://tb.huixinmuqiang.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://om.yuntaijiaju.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://lc.shxzskj.cn

[Q89] 判断表是否存在
来源：http://ez.bookmarksfly.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://sc.panjiajie.cn

[Q90] 生成序号列
来源：http://vy.gzmigu.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hv.muxihuayi.cn

================================================================================
来源：http://nf.yuntaijiaju.cn

R. Bash 专题
来源：http://de.jctech888.com.cn

================================================================================
来源：http://yl.9csxet.cn

[R01] shebang 与严格模式
来源：http://dp.muxihuayi.cn

#!/usr/bin/env bash
来源：http://su.shxzskj.cn

set -euo pipefail
来源：http://si.colortex.cn

[R02] 变量赋值与使用
来源：http://gz.shxzskj.cn

name="Tom"; echo "$name"
来源：http://dd.nicolike.cn

[R03] 只读变量
来源：http://uy.chemitech.net.cn

readonly PI=3.14
来源：http://vm.jianghongdianzi.cn

[R04] 位置参数
来源：http://ht.yuntaijiaju.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://rv.521024.cn

[R05] 参数默认值
来源：http://gr.bookmarksfly.cn

name="${1:-default}"
来源：http://hn.muxihuayi.cn

[R06] 判断命令是否存在
来源：http://gs.szsharing.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://qa.huixiangedu.cn

[R07] if 判断文件
来源：http://ko.colortex.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://nk.9csxet.cn

[R08] 数值比较
来源：http://mk.521024.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://ij.9csxet.cn

[R09] 字符串比较
来源：http://ga.chemitech.net.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://oa.newstarts.cn

[R10] 正则匹配
来源：http://dy.jctech888.com.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://rm.hnjuh.cn

[R11] case 多分支
来源：http://vg.huanxung.cn

case "$1" in
来源：http://rs.521024.cn

start) echo "启动" ;;
来源：http://id.chemitech.net.cn

stop)  echo "停止" ;;
来源：http://md.szxytkj.cn

*)     echo "未知命令" ;;
来源：http://lg.gzmigu.cn

esac
来源：http://aq.haigaiapp.cn

[R12] for 遍历文件
来源：http://pe.huanxung.cn

for f in *.txt; do echo "$f"; done
来源：http://ul.lnxyls.cn

[R13] for 计数循环
来源：http://uv.521024.cn

for i in {1..10}; do echo "$i"; done
来源：http://ls.bookmarksfly.cn

[R14] C 风格 for
来源：http://xq.bookmarksfly.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://be.bookmarksfly.cn

[R15] while 逐行读文件
来源：http://de.szxytkj.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://kl.jianghongdianzi.cn

[R16] until 等待条件
来源：http://ht.yuntaijiaju.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://sq.huanxung.cn

[R17] 数组定义与取值
来源：http://tu.shxzskj.cn

arr=(a b c); echo "${arr[0]}"
来源：http://ge.jianghongdianzi.cn

[R18] 遍历数组
来源：http://qw.muxihuayi.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://gc.yuexingan06.cn

[R19] 数组长度
来源：http://qu.yuntaijiaju.cn

echo "${#arr[@]}"
来源：http://lq.lnxyls.cn

[R20] 关联数组（字典）
来源：http://qb.bjjhwx.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ah.lnxyls.cn

[R21] 字符串长度
来源：http://ys.panjiajie.cn

echo "${#s}"
来源：http://le.yuntaijiaju.cn

[R22] 截取子串
来源：http://cd.wgjwhj.cn

echo "${s:0:5}"
来源：http://pv.panjiajie.cn

[R23] 字符串替换
来源：http://be.huanxung.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://fh.panjiajie.cn

[R24] 大小写转换
来源：http://gx.hahajie.cn

echo "${s^^}"; echo "${s,,}"
来源：http://tn.shxzskj.cn

[R25] 去后缀 / 去前缀
来源：http://eq.nicolike.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://dd.haigaiapp.cn

[R26] 命令替换
来源：http://oz.nicolike.cn

now=$(date +%F); echo "$now"
来源：http://os.bookmarksfly.cn

[R27] 算术展开
来源：http://pb.huixiangedu.cn

echo $((1 + 2 * 3))
来源：http://os.yuexingan06.cn

[R28] 浮点运算
来源：http://xw.nicolike.cn

echo "scale=2; 10/3" | bc
来源：http://uv.shxzskj.cn

[R29] 定义函数
来源：http://fl.9csxet.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://fk.hnjuh.cn

[R30] 函数返回状态码
来源：http://ba.huixinmuqiang.cn

f() { return 0; }; f || echo "失败了"
来源：http://ve.muxihuayi.cn

[R31] 局部变量
来源：http://sd.9csxet.cn

f() { local x=1; echo "$x"; }
来源：http://gn.newstarts.cn

[R32] 参数个数校验
来源：http://ls.hahajie.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://lp.huixiangedu.cn

[R33] 捕获错误并提示行号
来源：http://sb.nicolike.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://un.wgjwhj.cn

[R34] 退出时清理
来源：http://xm.lnxyls.cn

trap 'rm -f "$tmp"' EXIT
来源：http://fz.wgjwhj.cn

[R35] 后台执行并等待
来源：http://hl.newstarts.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://ne.shxzukj.cn

[R36] 并发执行多个任务
来源：http://jc.shtwfgs.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://fi.colortex.cn

[R37] 把输出赋给变量
来源：http://nq.szsharing.cn

files=$(ls -1)
来源：http://mm.bookmarksfly.cn

[R38] 管道串联
来源：http://gm.asd995.cn

cat a.txt | grep -i error | wc -l
来源：http://xl.shtwfgs.cn

[R39] 重定向标准输出与错误
来源：http://ow.shxzskj.cn


<!-- 参考信息 -->