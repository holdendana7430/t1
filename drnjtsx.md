代发 wailian999

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://qh.huixiangedu.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://rg.huanxung.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://um.yuexingan06.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://cc.huanxung.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://zh.wgjwhj.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://pq.hahajie.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ym.shtwfgs.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://az.szsharing.cn

================================================================================
来源：http://xb.521024.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://of.shxzskj.cn

================================================================================
来源：http://iy.bookmarksfly.cn

[Q01] 创建表
来源：http://az.hahajie.cn

CREATE TABLE users (
来源：http://xv.panjiajie.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://nt.wgjwhj.cn

name VARCHAR(50) NOT NULL,
来源：http://ex.szxytkj.cn

email VARCHAR(100) UNIQUE,
来源：http://dl.yuexingan06.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://bq.panjiajie.cn

);
来源：http://vo.jianghongdianzi.cn

[Q02] 创建带外键的表
来源：http://im.521024.cn

CREATE TABLE orders (
来源：http://pf.yuntaijiaju.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ye.haigaiapp.cn

user_id INT NOT NULL,
来源：http://mw.bookmarksfly.cn

amount DECIMAL(10, 2),
来源：http://dg.9csxet.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://gt.9csxet.cn

);
来源：http://ov.bookmarksfly.cn

[Q03] 增加列
来源：http://da.yuexingan06.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ku.szsharing.cn

[Q04] 修改列类型
来源：http://kj.521024.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://tq.huixinmuqiang.cn

[Q05] 重命名列
来源：http://xk.wgjwhj.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ur.szsharing.cn

[Q06] 删除列
来源：http://ij.hnjuh.cn

ALTER TABLE users DROP COLUMN age;
来源：http://ti.jianghongdianzi.cn

[Q07] 删除表
来源：http://ze.chemitech.net.cn

DROP TABLE IF EXISTS orders;
来源：http://kg.muxihuayi.cn

[Q08] 创建普通索引
来源：http://oj.huanxung.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://lv.szsharing.cn

[Q09] 创建唯一索引
来源：http://xy.9csxet.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://qd.huixiangedu.cn

[Q10] 插入单行
来源：http://ay.shxzukj.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://jo.gzmigu.cn

[Q11] 一次插入多行
来源：http://ct.521024.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://dh.huixiangedu.cn

[Q12] 插入后取自增 ID
来源：http://qy.asd995.cn

INSERT INTO users (name) VALUES ('C');
来源：http://gi.colortex.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://er.panjiajie.cn

[Q13] 忽略重复插入
来源：http://kj.shxzskj.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://be.bjjhwx.cn

[Q14] 存在则更新（upsert）
来源：http://aw.yuntaijiaju.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ef.newstarts.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://zs.wgjwhj.cn

[Q15] 查询全部
来源：http://lt.shxzskj.cn

SELECT * FROM users;
来源：http://hj.bookmarksfly.cn

[Q16] 查询指定列
来源：http://eh.hnjuh.cn

SELECT id, name FROM users;
来源：http://yc.huanxung.cn

[Q17] 条件查询
来源：http://il.hnjuh.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://nf.huixiangedu.cn

[Q18] 模糊匹配
来源：http://xy.huixiangedu.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://fk.shxzukj.cn

[Q19] 范围查询
来源：http://dy.bjjhwx.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://lh.nszjky.cn

[Q20] IN 列表
来源：http://lt.521024.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://al.yuexingan06.cn

[Q21] 空值判断
来源：http://hs.muxihuayi.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://ao.521024.cn

[Q22] 排序
来源：http://jx.bookmarksfly.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://sh.chemitech.net.cn

[Q23] 分页
来源：http://np.shxzskj.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ia.bjjhwx.cn

[Q24] 去重
来源：http://kj.yuntaijiaju.cn

SELECT DISTINCT city FROM users;
来源：http://in.shxzukj.cn

[Q25] 只取前 N 条
来源：http://uo.hnjuh.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://au.huanxung.cn

[Q26] 计数
来源：http://ct.asd995.cn

SELECT COUNT(*) FROM users;
来源：http://ly.chemitech.net.cn

[Q27] 条件计数
来源：http://mw.asd995.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://si.panjiajie.cn

[Q28] 求和与平均
来源：http://qx.chemitech.net.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://lz.shxzskj.cn

[Q29] 最大最小值
来源：http://rs.nicolike.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://jk.lnxyls.cn

[Q30] 分组统计
来源：http://df.newstarts.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ep.newstarts.cn

[Q31] 分组后过滤
来源：http://ph.newstarts.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://gv.shxzskj.cn

[Q32] 分组拼接字符串
来源：http://ns.huanxung.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://rk.chemitech.net.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://bf.newstarts.cn

[Q33] 多列分组
来源：http://sy.muxihuayi.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://pd.shxzukj.cn

[Q34] 每组取第一条
来源：http://br.huixinmuqiang.cn

SELECT * FROM (
来源：http://rw.chemitech.net.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ft.bjjhwx.cn

) t WHERE rn = 1;
来源：http://pf.colortex.cn

[Q35] 内连接
来源：http://ws.hnjuh.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://lw.szsharing.cn

[Q36] 左连接
来源：http://et.hahajie.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://bj.9csxet.cn

[Q37] 右连接
来源：http://fp.huixiangedu.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://un.chemitech.net.cn

[Q38] 全外连接（PostgreSQL）
来源：http://pf.szsharing.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://yj.wgjwhj.cn

[Q39] 自连接（查上下级）
来源：http://pa.panjiajie.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://yb.huixinmuqiang.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ui.asd995.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://pp.panjiajie.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ky.9csxet.cn

[Q41] 多表连接
来源：http://nl.szxytkj.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://lv.gzmigu.cn

JOIN users u ON u.id = o.user_id
来源：http://bn.huixiangedu.cn

JOIN products p ON p.id = o.product_id;
来源：http://kl.yuntaijiaju.cn

[Q42] 连接条件附加过滤
来源：http://kg.gzmigu.cn

SELECT u.name, o.amount FROM users u
来源：http://np.colortex.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://jf.nicolike.cn

[Q43] 标量子查询
来源：http://ac.huanxung.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://zj.newstarts.cn

[Q44] IN 子查询
来源：http://bk.wgjwhj.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://sx.shxzukj.cn

[Q45] EXISTS 判断存在
来源：http://uj.asd995.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ar.shxzskj.cn

[Q46] NOT EXISTS 判断不存在
来源：http://nf.muxihuayi.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://un.huanxung.cn

[Q47] 与平均值比较
来源：http://hr.gzmigu.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://xw.asd995.cn

[Q48] CTE 公用表表达式
来源：http://hv.hnjuh.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://nz.shtwfgs.cn

SELECT * FROM t WHERE c > 5;
来源：http://tp.gzmigu.cn

[Q49] 更新单行
来源：http://xs.asd995.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://pc.shxzukj.cn

[Q50] 批量更新
来源：http://ba.shtwfgs.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://eh.colortex.cn

[Q51] 用子查询更新
来源：http://gn.szsharing.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://sf.521024.cn

[Q52] 删除指定行
来源：http://su.521024.cn

DELETE FROM users WHERE id = 10;
来源：http://cg.shxzukj.cn

[Q53] 按条件删除
来源：http://pr.huixiangedu.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://sy.panjiajie.cn

[Q54] 清空表
来源：http://gt.newstarts.cn

TRUNCATE TABLE logs;
来源：http://nt.wgjwhj.cn

[Q55] 排名（并列占位）
来源：http://ue.wgjwhj.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hn.nicolike.cn

[Q56] 密集排名（并列不占位）
来源：http://lc.shxzskj.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ei.yuntaijiaju.cn

[Q57] 行号
来源：http://eq.gzmigu.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://jy.jianghongdianzi.cn

[Q58] 累计求和
来源：http://ru.chemitech.net.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://yj.haigaiapp.cn

[Q59] 分组内累计
来源：http://wd.hahajie.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://fk.huanxung.cn

[Q60] 取上一行 / 下一行
来源：http://xx.huanxung.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://zf.hnjuh.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://pn.shtwfgs.cn

[Q61] 移动平均
来源：http://pt.newstarts.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ww.haigaiapp.cn

[Q62] 分组占比
来源：http://kj.lnxyls.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://pa.panjiajie.cn

[Q63] 开启事务
来源：http://um.muxihuayi.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://mb.lnxyls.cn

[Q64] 提交事务
来源：http://mw.huanxung.cn

COMMIT;
来源：http://cw.huixiangedu.cn

[Q65] 回滚事务
来源：http://fw.szxytkj.cn

ROLLBACK;
来源：http://lu.jctech888.com.cn

[Q66] 行锁查询
来源：http://vm.muxihuayi.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://qt.wgjwhj.cn

[Q67] 设置隔离级别
来源：http://hy.nicolike.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hx.muxihuayi.cn

[Q68] 保存点
来源：http://nn.chemitech.net.cn

SAVEPOINT sp1;
来源：http://hz.panjiajie.cn

ROLLBACK TO sp1;
来源：http://pf.haigaiapp.cn

[Q69] 查看执行计划
来源：http://eh.chemitech.net.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://qy.shxzukj.cn

[Q70] 更新统计信息
来源：http://ua.szxytkj.cn

ANALYZE TABLE users;
来源：http://hh.szxytkj.cn

[Q71] 查看建表语句
来源：http://un.newstarts.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://yc.muxihuayi.cn

[Q72] 查看索引
来源：http://tq.jctech888.com.cn

SHOW INDEX FROM users;
来源：http://dx.bjjhwx.cn

[Q73] 查看表状态
来源：http://by.yuexingan06.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://xq.panjiajie.cn

[Q74] 强制使用索引
来源：http://mq.lnxyls.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://rp.bjjhwx.cn

[Q75] 日期格式化
来源：http://gm.huanxung.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://oa.szsharing.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://nd.yuntaijiaju.cn

[Q76] 按天统计
来源：http://ma.huixinmuqiang.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://gn.haigaiapp.cn

[Q77] 时间加减
来源：http://xo.jctech888.com.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://iv.wgjwhj.cn

[Q78] 当前时间
来源：http://mu.lnxyls.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wk.panjiajie.cn

[Q79] 字符串拼接
来源：http://ak.huixiangedu.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://to.asd995.cn

[Q80] 字符串截取
来源：http://cq.nszjky.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://cx.haigaiapp.cn

[Q81] 字符串替换
来源：http://mt.huanxung.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ai.asd995.cn

[Q82] 字符长度与字节长度
来源：http://tn.szsharing.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://vv.9csxet.cn

[Q83] 大小写转换
来源：http://xl.jianghongdianzi.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://dl.nszjky.cn

[Q84] 去除首尾空格
来源：http://wa.shxzskj.cn

SELECT TRIM(name) FROM users;
来源：http://cx.shxzskj.cn

[Q85] 数值取整
来源：http://lz.yuntaijiaju.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wt.lnxyls.cn

[Q86] 读取 JSON 字段
来源：http://pq.haigaiapp.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://oo.szxytkj.cn

[Q87] JSON 字段做条件
来源：http://lc.asd995.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://kk.shxzukj.cn

[Q88] 行转列（条件聚合）
来源：http://sh.hnjuh.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mo.huixiangedu.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://xf.gzmigu.cn

[Q89] 判断表是否存在
来源：http://zz.jctech888.com.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://qx.nszjky.cn

[Q90] 生成序号列
来源：http://yx.nicolike.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://nh.nicolike.cn

================================================================================
来源：http://fz.gzmigu.cn

R. Bash 专题
来源：http://vb.wgjwhj.cn

================================================================================
来源：http://kh.bookmarksfly.cn

[R01] shebang 与严格模式
来源：http://ao.haigaiapp.cn

#!/usr/bin/env bash
来源：http://cr.bjjhwx.cn

set -euo pipefail
来源：http://ki.chemitech.net.cn

[R02] 变量赋值与使用
来源：http://lu.bjjhwx.cn

name="Tom"; echo "$name"
来源：http://ax.newstarts.cn

[R03] 只读变量
来源：http://ei.chemitech.net.cn

readonly PI=3.14
来源：http://vk.huanxung.cn

[R04] 位置参数
来源：http://vz.9csxet.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://kf.9csxet.cn

[R05] 参数默认值
来源：http://ya.9csxet.cn

name="${1:-default}"
来源：http://qx.newstarts.cn

[R06] 判断命令是否存在
来源：http://cv.hnjuh.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://xs.hahajie.cn

[R07] if 判断文件
来源：http://gv.panjiajie.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://cx.chemitech.net.cn

[R08] 数值比较
来源：http://gk.muxihuayi.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://up.bjjhwx.cn

[R09] 字符串比较
来源：http://kd.nicolike.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://tw.huixinmuqiang.cn

[R10] 正则匹配
来源：http://gq.huixinmuqiang.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://pd.shxzskj.cn

[R11] case 多分支
来源：http://iw.521024.cn

case "$1" in
来源：http://te.huixinmuqiang.cn

start) echo "启动" ;;
来源：http://qt.bjjhwx.cn

stop)  echo "停止" ;;
来源：http://bg.hahajie.cn

*)     echo "未知命令" ;;
来源：http://mo.521024.cn

esac
来源：http://zf.colortex.cn

[R12] for 遍历文件
来源：http://mm.muxihuayi.cn

for f in *.txt; do echo "$f"; done
来源：http://os.jctech888.com.cn

[R13] for 计数循环
来源：http://eg.yuexingan06.cn

for i in {1..10}; do echo "$i"; done
来源：http://jq.szsharing.cn

[R14] C 风格 for
来源：http://lm.colortex.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ru.yuexingan06.cn

[R15] while 逐行读文件
来源：http://vu.lnxyls.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://rp.9csxet.cn

[R16] until 等待条件
来源：http://zm.hnjuh.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://zp.huanxung.cn

[R17] 数组定义与取值
来源：http://kc.nicolike.cn

arr=(a b c); echo "${arr[0]}"
来源：http://ej.9csxet.cn

[R18] 遍历数组
来源：http://oo.muxihuayi.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://he.shtwfgs.cn

[R19] 数组长度
来源：http://zb.bookmarksfly.cn

echo "${#arr[@]}"
来源：http://ax.szxytkj.cn

[R20] 关联数组（字典）
来源：http://fl.521024.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://fe.shxzskj.cn

[R21] 字符串长度
来源：http://pm.newstarts.cn

echo "${#s}"
来源：http://be.panjiajie.cn

[R22] 截取子串
来源：http://gi.asd995.cn

echo "${s:0:5}"
来源：http://tb.wgjwhj.cn

[R23] 字符串替换
来源：http://xp.jianghongdianzi.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ak.hahajie.cn

[R24] 大小写转换
来源：http://ku.huanxung.cn

echo "${s^^}"; echo "${s,,}"
来源：http://mm.9csxet.cn

[R25] 去后缀 / 去前缀
来源：http://ou.yuexingan06.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://ke.panjiajie.cn

[R26] 命令替换
来源：http://xk.asd995.cn

now=$(date +%F); echo "$now"
来源：http://xk.9csxet.cn

[R27] 算术展开
来源：http://bt.szsharing.cn

echo $((1 + 2 * 3))
来源：http://pl.chemitech.net.cn

[R28] 浮点运算
来源：http://ek.shxzukj.cn

echo "scale=2; 10/3" | bc
来源：http://ac.521024.cn

[R29] 定义函数
来源：http://yn.huixiangedu.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://as.9csxet.cn

[R30] 函数返回状态码
来源：http://qz.haigaiapp.cn

f() { return 0; }; f || echo "失败了"
来源：http://xu.haigaiapp.cn

[R31] 局部变量
来源：http://md.huixiangedu.cn

f() { local x=1; echo "$x"; }
来源：http://ax.nszjky.cn

[R32] 参数个数校验
来源：http://jb.yuntaijiaju.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://vb.shxzukj.cn

[R33] 捕获错误并提示行号
来源：http://ox.yuntaijiaju.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://rp.jianghongdianzi.cn

[R34] 退出时清理
来源：http://yh.nicolike.cn

trap 'rm -f "$tmp"' EXIT
来源：http://yn.9csxet.cn

[R35] 后台执行并等待
来源：http://tj.huixiangedu.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://ey.jctech888.com.cn

[R36] 并发执行多个任务
来源：http://zy.bookmarksfly.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hc.szsharing.cn

[R37] 把输出赋给变量
来源：http://eu.nicolike.cn

files=$(ls -1)
来源：http://mq.9csxet.cn

[R38] 管道串联
来源：http://qm.gzmigu.cn

cat a.txt | grep -i error | wc -l
来源：http://dq.gzmigu.cn

[R39] 重定向标准输出与错误
来源：http://vg.nicolike.cn


<!-- 参考信息 -->