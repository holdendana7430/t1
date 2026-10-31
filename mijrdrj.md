代发 wailian999

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://vf.asd995.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://id.muxihuayi.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ta.bookmarksfly.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ip.gzmigu.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://np.huixiangedu.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://uo.shtwfgs.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://it.wgjwhj.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://le.colortex.cn

================================================================================
来源：http://qj.bookmarksfly.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://qn.jctech888.com.cn

================================================================================
来源：http://vg.hnjuh.cn

[Q01] 创建表
来源：http://mh.panjiajie.cn

CREATE TABLE users (
来源：http://xn.huixiangedu.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ii.szsharing.cn

name VARCHAR(50) NOT NULL,
来源：http://te.huixiangedu.cn

email VARCHAR(100) UNIQUE,
来源：http://tl.yuntaijiaju.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://tg.panjiajie.cn

);
来源：http://ba.shxzskj.cn

[Q02] 创建带外键的表
来源：http://ko.wgjwhj.cn

CREATE TABLE orders (
来源：http://hr.bookmarksfly.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ji.colortex.cn

user_id INT NOT NULL,
来源：http://ez.huixinmuqiang.cn

amount DECIMAL(10, 2),
来源：http://xg.lnxyls.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ux.hnjuh.cn

);
来源：http://vc.hnjuh.cn

[Q03] 增加列
来源：http://jo.hnjuh.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ip.shtwfgs.cn

[Q04] 修改列类型
来源：http://vf.jctech888.com.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hd.hahajie.cn

[Q05] 重命名列
来源：http://ep.shtwfgs.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ns.nszjky.cn

[Q06] 删除列
来源：http://dy.lnxyls.cn

ALTER TABLE users DROP COLUMN age;
来源：http://mi.nicolike.cn

[Q07] 删除表
来源：http://ku.nszjky.cn

DROP TABLE IF EXISTS orders;
来源：http://tb.chemitech.net.cn

[Q08] 创建普通索引
来源：http://lv.hahajie.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://pn.colortex.cn

[Q09] 创建唯一索引
来源：http://bn.shxzukj.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ea.panjiajie.cn

[Q10] 插入单行
来源：http://ec.nszjky.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://tv.huixiangedu.cn

[Q11] 一次插入多行
来源：http://xe.bookmarksfly.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://rl.szxytkj.cn

[Q12] 插入后取自增 ID
来源：http://fx.newstarts.cn

INSERT INTO users (name) VALUES ('C');
来源：http://wv.jctech888.com.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hj.shxzskj.cn

[Q13] 忽略重复插入
来源：http://iu.hnjuh.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://da.haigaiapp.cn

[Q14] 存在则更新（upsert）
来源：http://wn.nszjky.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://kn.yuntaijiaju.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ih.szxytkj.cn

[Q15] 查询全部
来源：http://ht.bookmarksfly.cn

SELECT * FROM users;
来源：http://ar.chemitech.net.cn

[Q16] 查询指定列
来源：http://vy.chemitech.net.cn

SELECT id, name FROM users;
来源：http://zc.gzmigu.cn

[Q17] 条件查询
来源：http://om.jianghongdianzi.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://pw.bookmarksfly.cn

[Q18] 模糊匹配
来源：http://lg.hnjuh.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://gd.shxzskj.cn

[Q19] 范围查询
来源：http://iv.shtwfgs.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ue.shxzukj.cn

[Q20] IN 列表
来源：http://or.lnxyls.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://xr.newstarts.cn

[Q21] 空值判断
来源：http://sh.jctech888.com.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://mo.huixinmuqiang.cn

[Q22] 排序
来源：http://kg.9csxet.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://im.9csxet.cn

[Q23] 分页
来源：http://eo.shtwfgs.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://gd.yuntaijiaju.cn

[Q24] 去重
来源：http://fb.huanxung.cn

SELECT DISTINCT city FROM users;
来源：http://bx.shxzukj.cn

[Q25] 只取前 N 条
来源：http://rd.nszjky.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ic.muxihuayi.cn

[Q26] 计数
来源：http://ak.nszjky.cn

SELECT COUNT(*) FROM users;
来源：http://yy.chemitech.net.cn

[Q27] 条件计数
来源：http://ca.szsharing.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ek.asd995.cn

[Q28] 求和与平均
来源：http://ut.asd995.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://th.521024.cn

[Q29] 最大最小值
来源：http://js.wgjwhj.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://fu.szsharing.cn

[Q30] 分组统计
来源：http://go.521024.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wg.yuntaijiaju.cn

[Q31] 分组后过滤
来源：http://ba.lnxyls.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wk.shtwfgs.cn

[Q32] 分组拼接字符串
来源：http://mc.asd995.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ur.muxihuayi.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://sf.chemitech.net.cn

[Q33] 多列分组
来源：http://bb.wgjwhj.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://jp.yuexingan06.cn

[Q34] 每组取第一条
来源：http://fj.panjiajie.cn

SELECT * FROM (
来源：http://xe.yuntaijiaju.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://qb.lnxyls.cn

) t WHERE rn = 1;
来源：http://lj.jctech888.com.cn

[Q35] 内连接
来源：http://bt.haigaiapp.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://qj.shxzskj.cn

[Q36] 左连接
来源：http://wb.panjiajie.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ke.yuntaijiaju.cn

[Q37] 右连接
来源：http://fk.bookmarksfly.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://iu.panjiajie.cn

[Q38] 全外连接（PostgreSQL）
来源：http://ne.jctech888.com.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://av.wgjwhj.cn

[Q39] 自连接（查上下级）
来源：http://ul.chemitech.net.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://el.muxihuayi.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://an.muxihuayi.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://rk.wgjwhj.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://dd.newstarts.cn

[Q41] 多表连接
来源：http://hz.haigaiapp.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://jk.muxihuayi.cn

JOIN users u ON u.id = o.user_id
来源：http://ec.shxzukj.cn

JOIN products p ON p.id = o.product_id;
来源：http://ks.asd995.cn

[Q42] 连接条件附加过滤
来源：http://at.yuexingan06.cn

SELECT u.name, o.amount FROM users u
来源：http://pc.colortex.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ep.521024.cn

[Q43] 标量子查询
来源：http://fr.hahajie.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://km.gzmigu.cn

[Q44] IN 子查询
来源：http://ml.nszjky.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://qn.nszjky.cn

[Q45] EXISTS 判断存在
来源：http://oq.muxihuayi.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ps.szxytkj.cn

[Q46] NOT EXISTS 判断不存在
来源：http://wa.nicolike.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wd.bookmarksfly.cn

[Q47] 与平均值比较
来源：http://vn.chemitech.net.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ym.asd995.cn

[Q48] CTE 公用表表达式
来源：http://ho.shxzskj.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://co.wgjwhj.cn

SELECT * FROM t WHERE c > 5;
来源：http://tc.gzmigu.cn

[Q49] 更新单行
来源：http://zc.hnjuh.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ru.panjiajie.cn

[Q50] 批量更新
来源：http://pv.szxytkj.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://ox.haigaiapp.cn

[Q51] 用子查询更新
来源：http://uv.huixiangedu.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://ir.jctech888.com.cn

[Q52] 删除指定行
来源：http://ks.hahajie.cn

DELETE FROM users WHERE id = 10;
来源：http://oj.huanxung.cn

[Q53] 按条件删除
来源：http://kt.nszjky.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://kw.huanxung.cn

[Q54] 清空表
来源：http://so.szxytkj.cn

TRUNCATE TABLE logs;
来源：http://cu.hahajie.cn

[Q55] 排名（并列占位）
来源：http://nr.yuexingan06.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://nh.szsharing.cn

[Q56] 密集排名（并列不占位）
来源：http://kk.shtwfgs.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://zy.szsharing.cn

[Q57] 行号
来源：http://dd.huanxung.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://im.nicolike.cn

[Q58] 累计求和
来源：http://hv.jctech888.com.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://jy.yuntaijiaju.cn

[Q59] 分组内累计
来源：http://tx.jctech888.com.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ye.asd995.cn

[Q60] 取上一行 / 下一行
来源：http://ep.bjjhwx.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wt.hahajie.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://br.bookmarksfly.cn

[Q61] 移动平均
来源：http://gk.nicolike.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://aq.yuntaijiaju.cn

[Q62] 分组占比
来源：http://cd.muxihuayi.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://yz.huanxung.cn

[Q63] 开启事务
来源：http://gg.gzmigu.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://kb.yuntaijiaju.cn

[Q64] 提交事务
来源：http://rt.gzmigu.cn

COMMIT;
来源：http://gk.huixinmuqiang.cn

[Q65] 回滚事务
来源：http://gw.muxihuayi.cn

ROLLBACK;
来源：http://se.szsharing.cn

[Q66] 行锁查询
来源：http://jh.panjiajie.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ja.huixiangedu.cn

[Q67] 设置隔离级别
来源：http://dl.huixinmuqiang.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://et.521024.cn

[Q68] 保存点
来源：http://wv.huixinmuqiang.cn

SAVEPOINT sp1;
来源：http://hx.nszjky.cn

ROLLBACK TO sp1;
来源：http://qu.asd995.cn

[Q69] 查看执行计划
来源：http://oy.szxytkj.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://vy.yuntaijiaju.cn

[Q70] 更新统计信息
来源：http://dg.yuexingan06.cn

ANALYZE TABLE users;
来源：http://sh.szxytkj.cn

[Q71] 查看建表语句
来源：http://tx.shxzskj.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://pn.jianghongdianzi.cn

[Q72] 查看索引
来源：http://ck.huanxung.cn

SHOW INDEX FROM users;
来源：http://oq.haigaiapp.cn

[Q73] 查看表状态
来源：http://di.bjjhwx.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://lx.gzmigu.cn

[Q74] 强制使用索引
来源：http://fc.colortex.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mq.shtwfgs.cn

[Q75] 日期格式化
来源：http://pt.huixiangedu.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://cr.bookmarksfly.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://yb.muxihuayi.cn

[Q76] 按天统计
来源：http://bz.huixinmuqiang.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ut.wgjwhj.cn

[Q77] 时间加减
来源：http://qe.yuexingan06.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://lg.wgjwhj.cn

[Q78] 当前时间
来源：http://he.chemitech.net.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://in.colortex.cn

[Q79] 字符串拼接
来源：http://kt.asd995.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://yp.newstarts.cn

[Q80] 字符串截取
来源：http://bv.wgjwhj.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ge.colortex.cn

[Q81] 字符串替换
来源：http://gd.chemitech.net.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://po.newstarts.cn

[Q82] 字符长度与字节长度
来源：http://jk.chemitech.net.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://rt.haigaiapp.cn

[Q83] 大小写转换
来源：http://xa.bjjhwx.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ck.shxzukj.cn

[Q84] 去除首尾空格
来源：http://ft.chemitech.net.cn

SELECT TRIM(name) FROM users;
来源：http://mf.yuntaijiaju.cn

[Q85] 数值取整
来源：http://km.hnjuh.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://va.bjjhwx.cn

[Q86] 读取 JSON 字段
来源：http://ph.muxihuayi.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ak.gzmigu.cn

[Q87] JSON 字段做条件
来源：http://fl.chemitech.net.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ia.nszjky.cn

[Q88] 行转列（条件聚合）
来源：http://pw.521024.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mn.shtwfgs.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://pi.jctech888.com.cn

[Q89] 判断表是否存在
来源：http://lb.wgjwhj.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://oj.newstarts.cn

[Q90] 生成序号列
来源：http://ud.lnxyls.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ge.huixiangedu.cn

================================================================================
来源：http://by.jianghongdianzi.cn

R. Bash 专题
来源：http://yr.wgjwhj.cn

================================================================================
来源：http://ae.bookmarksfly.cn

[R01] shebang 与严格模式
来源：http://hs.lnxyls.cn

#!/usr/bin/env bash
来源：http://dd.hnjuh.cn

set -euo pipefail
来源：http://cp.yuexingan06.cn

[R02] 变量赋值与使用
来源：http://jc.huanxung.cn

name="Tom"; echo "$name"
来源：http://fp.shxzskj.cn

[R03] 只读变量
来源：http://ez.nicolike.cn

readonly PI=3.14
来源：http://tu.wgjwhj.cn

[R04] 位置参数
来源：http://vh.huixinmuqiang.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://bn.bookmarksfly.cn

[R05] 参数默认值
来源：http://vh.newstarts.cn

name="${1:-default}"
来源：http://jc.huanxung.cn

[R06] 判断命令是否存在
来源：http://xy.yuntaijiaju.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://oj.521024.cn

[R07] if 判断文件
来源：http://nq.jctech888.com.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://qs.haigaiapp.cn

[R08] 数值比较
来源：http://to.nszjky.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://vf.chemitech.net.cn

[R09] 字符串比较
来源：http://lt.panjiajie.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://lt.jctech888.com.cn

[R10] 正则匹配
来源：http://rq.panjiajie.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://cs.haigaiapp.cn

[R11] case 多分支
来源：http://za.haigaiapp.cn

case "$1" in
来源：http://bz.shtwfgs.cn

start) echo "启动" ;;
来源：http://jk.hnjuh.cn

stop)  echo "停止" ;;
来源：http://ky.shxzukj.cn

*)     echo "未知命令" ;;
来源：http://vm.bookmarksfly.cn

esac
来源：http://bs.wgjwhj.cn

[R12] for 遍历文件
来源：http://di.colortex.cn

for f in *.txt; do echo "$f"; done
来源：http://ew.yuexingan06.cn

[R13] for 计数循环
来源：http://eg.bookmarksfly.cn

for i in {1..10}; do echo "$i"; done
来源：http://df.yuexingan06.cn

[R14] C 风格 for
来源：http://ld.muxihuayi.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://jo.nicolike.cn

[R15] while 逐行读文件
来源：http://ek.huixinmuqiang.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://zx.huanxung.cn

[R16] until 等待条件
来源：http://po.jianghongdianzi.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://eg.bjjhwx.cn

[R17] 数组定义与取值
来源：http://fd.colortex.cn

arr=(a b c); echo "${arr[0]}"
来源：http://xl.haigaiapp.cn

[R18] 遍历数组
来源：http://lf.panjiajie.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://cp.haigaiapp.cn

[R19] 数组长度
来源：http://nr.wgjwhj.cn

echo "${#arr[@]}"
来源：http://ax.szsharing.cn

[R20] 关联数组（字典）
来源：http://ke.szsharing.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ne.haigaiapp.cn

[R21] 字符串长度
来源：http://wu.shxzukj.cn

echo "${#s}"
来源：http://pu.szsharing.cn

[R22] 截取子串
来源：http://yt.shtwfgs.cn

echo "${s:0:5}"
来源：http://ix.wgjwhj.cn

[R23] 字符串替换
来源：http://rg.9csxet.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ln.hahajie.cn

[R24] 大小写转换
来源：http://jd.lnxyls.cn

echo "${s^^}"; echo "${s,,}"
来源：http://gd.muxihuayi.cn

[R25] 去后缀 / 去前缀
来源：http://jt.gzmigu.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://dy.panjiajie.cn

[R26] 命令替换
来源：http://vb.lnxyls.cn

now=$(date +%F); echo "$now"
来源：http://je.hnjuh.cn

[R27] 算术展开
来源：http://hd.lnxyls.cn

echo $((1 + 2 * 3))
来源：http://nu.yuntaijiaju.cn

[R28] 浮点运算
来源：http://ry.chemitech.net.cn

echo "scale=2; 10/3" | bc
来源：http://hb.nszjky.cn

[R29] 定义函数
来源：http://ve.shxzukj.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ip.muxihuayi.cn

[R30] 函数返回状态码
来源：http://du.hahajie.cn

f() { return 0; }; f || echo "失败了"
来源：http://hl.9csxet.cn

[R31] 局部变量
来源：http://sf.muxihuayi.cn

f() { local x=1; echo "$x"; }
来源：http://tk.bjjhwx.cn

[R32] 参数个数校验
来源：http://dl.wgjwhj.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ej.jctech888.com.cn

[R33] 捕获错误并提示行号
来源：http://cj.nicolike.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://od.shxzskj.cn

[R34] 退出时清理
来源：http://md.jianghongdianzi.cn

trap 'rm -f "$tmp"' EXIT
来源：http://bi.shxzskj.cn

[R35] 后台执行并等待
来源：http://gz.hahajie.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://iv.asd995.cn

[R36] 并发执行多个任务
来源：http://my.szsharing.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://re.yuexingan06.cn

[R37] 把输出赋给变量
来源：http://cf.szxytkj.cn

files=$(ls -1)
来源：http://ap.huixiangedu.cn

[R38] 管道串联
来源：http://ag.hahajie.cn

cat a.txt | grep -i error | wc -l
来源：http://jg.gzmigu.cn

[R39] 重定向标准输出与错误
来源：http://uu.shtwfgs.cn


<!-- 参考信息 -->