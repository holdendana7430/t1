代发 wailian999

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://nl.yuntaijiaju.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://kr.hahajie.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://no.jctech888.com.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wr.hahajie.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://uj.hnjuh.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://np.hnjuh.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ot.lnxyls.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wr.shtwfgs.cn

================================================================================
来源：http://dg.haigaiapp.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://nw.huixiangedu.cn

================================================================================
来源：http://gf.chemitech.net.cn

[Q01] 创建表
来源：http://gi.nicolike.cn

CREATE TABLE users (
来源：http://zv.gzmigu.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://sw.chemitech.net.cn

name VARCHAR(50) NOT NULL,
来源：http://xm.huanxung.cn

email VARCHAR(100) UNIQUE,
来源：http://rb.szxytkj.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://pv.huixiangedu.cn

);
来源：http://bw.yuntaijiaju.cn

[Q02] 创建带外键的表
来源：http://ho.9csxet.cn

CREATE TABLE orders (
来源：http://yl.521024.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://gj.yuexingan06.cn

user_id INT NOT NULL,
来源：http://nx.nicolike.cn

amount DECIMAL(10, 2),
来源：http://ae.muxihuayi.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://fr.bookmarksfly.cn

);
来源：http://nq.jctech888.com.cn

[Q03] 增加列
来源：http://qd.asd995.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ky.haigaiapp.cn

[Q04] 修改列类型
来源：http://lt.shxzskj.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://lq.panjiajie.cn

[Q05] 重命名列
来源：http://sb.newstarts.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://zk.nicolike.cn

[Q06] 删除列
来源：http://ip.jctech888.com.cn

ALTER TABLE users DROP COLUMN age;
来源：http://bq.gzmigu.cn

[Q07] 删除表
来源：http://bm.chemitech.net.cn

DROP TABLE IF EXISTS orders;
来源：http://iw.yuexingan06.cn

[Q08] 创建普通索引
来源：http://sz.shxzskj.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://jl.wgjwhj.cn

[Q09] 创建唯一索引
来源：http://ax.shtwfgs.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://zj.asd995.cn

[Q10] 插入单行
来源：http://cp.hahajie.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://bb.asd995.cn

[Q11] 一次插入多行
来源：http://mn.szxytkj.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://iv.huixinmuqiang.cn

[Q12] 插入后取自增 ID
来源：http://sh.huixiangedu.cn

INSERT INTO users (name) VALUES ('C');
来源：http://qy.szxytkj.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ee.haigaiapp.cn

[Q13] 忽略重复插入
来源：http://wb.shxzukj.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wn.nszjky.cn

[Q14] 存在则更新（upsert）
来源：http://wy.hahajie.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://jn.nszjky.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ow.bjjhwx.cn

[Q15] 查询全部
来源：http://wi.9csxet.cn

SELECT * FROM users;
来源：http://en.shtwfgs.cn

[Q16] 查询指定列
来源：http://ne.panjiajie.cn

SELECT id, name FROM users;
来源：http://cr.nszjky.cn

[Q17] 条件查询
来源：http://ff.yuexingan06.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://np.gzmigu.cn

[Q18] 模糊匹配
来源：http://qz.bookmarksfly.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://bj.huixiangedu.cn

[Q19] 范围查询
来源：http://nq.haigaiapp.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://iq.lnxyls.cn

[Q20] IN 列表
来源：http://jq.yuntaijiaju.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://st.szsharing.cn

[Q21] 空值判断
来源：http://ta.szxytkj.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://ol.wgjwhj.cn

[Q22] 排序
来源：http://mo.521024.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://uu.yuexingan06.cn

[Q23] 分页
来源：http://rj.shtwfgs.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://fk.szxytkj.cn

[Q24] 去重
来源：http://ja.huixiangedu.cn

SELECT DISTINCT city FROM users;
来源：http://rd.521024.cn

[Q25] 只取前 N 条
来源：http://jf.wgjwhj.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://oh.9csxet.cn

[Q26] 计数
来源：http://fn.yuntaijiaju.cn

SELECT COUNT(*) FROM users;
来源：http://yb.yuntaijiaju.cn

[Q27] 条件计数
来源：http://kl.haigaiapp.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://vz.szsharing.cn

[Q28] 求和与平均
来源：http://ci.gzmigu.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://ck.muxihuayi.cn

[Q29] 最大最小值
来源：http://df.bjjhwx.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://rl.bjjhwx.cn

[Q30] 分组统计
来源：http://vz.jctech888.com.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://rs.haigaiapp.cn

[Q31] 分组后过滤
来源：http://ss.huanxung.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ws.shxzukj.cn

[Q32] 分组拼接字符串
来源：http://rg.nicolike.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://dn.yuntaijiaju.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://vm.hahajie.cn

[Q33] 多列分组
来源：http://rw.jctech888.com.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://kw.bookmarksfly.cn

[Q34] 每组取第一条
来源：http://xn.wgjwhj.cn

SELECT * FROM (
来源：http://qp.yuntaijiaju.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://gu.wgjwhj.cn

) t WHERE rn = 1;
来源：http://rz.bookmarksfly.cn

[Q35] 内连接
来源：http://eq.chemitech.net.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://of.huixinmuqiang.cn

[Q36] 左连接
来源：http://kg.chemitech.net.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://jq.colortex.cn

[Q37] 右连接
来源：http://mq.jianghongdianzi.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://fs.haigaiapp.cn

[Q38] 全外连接（PostgreSQL）
来源：http://ix.bjjhwx.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://cv.panjiajie.cn

[Q39] 自连接（查上下级）
来源：http://yt.newstarts.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://ec.szsharing.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://xq.gzmigu.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://he.hnjuh.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://lu.bjjhwx.cn

[Q41] 多表连接
来源：http://ud.shtwfgs.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://ct.shxzukj.cn

JOIN users u ON u.id = o.user_id
来源：http://bm.bjjhwx.cn

JOIN products p ON p.id = o.product_id;
来源：http://uw.chemitech.net.cn

[Q42] 连接条件附加过滤
来源：http://at.shtwfgs.cn

SELECT u.name, o.amount FROM users u
来源：http://yd.hahajie.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://cv.newstarts.cn

[Q43] 标量子查询
来源：http://vc.huixiangedu.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://de.huanxung.cn

[Q44] IN 子查询
来源：http://tk.huixinmuqiang.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ry.bjjhwx.cn

[Q45] EXISTS 判断存在
来源：http://lp.jianghongdianzi.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://xe.shxzukj.cn

[Q46] NOT EXISTS 判断不存在
来源：http://tr.colortex.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://au.shtwfgs.cn

[Q47] 与平均值比较
来源：http://rg.wgjwhj.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ie.shxzskj.cn

[Q48] CTE 公用表表达式
来源：http://fz.szsharing.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://tx.gzmigu.cn

SELECT * FROM t WHERE c > 5;
来源：http://ms.nicolike.cn

[Q49] 更新单行
来源：http://yz.panjiajie.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ix.521024.cn

[Q50] 批量更新
来源：http://yj.shtwfgs.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://tx.colortex.cn

[Q51] 用子查询更新
来源：http://nl.haigaiapp.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://xu.asd995.cn

[Q52] 删除指定行
来源：http://rq.nicolike.cn

DELETE FROM users WHERE id = 10;
来源：http://nv.szxytkj.cn

[Q53] 按条件删除
来源：http://ux.colortex.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://zn.szxytkj.cn

[Q54] 清空表
来源：http://cf.huanxung.cn

TRUNCATE TABLE logs;
来源：http://tu.yuntaijiaju.cn

[Q55] 排名（并列占位）
来源：http://lb.yuntaijiaju.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://dm.shtwfgs.cn

[Q56] 密集排名（并列不占位）
来源：http://en.jianghongdianzi.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://gu.jctech888.com.cn

[Q57] 行号
来源：http://rf.huanxung.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ok.bookmarksfly.cn

[Q58] 累计求和
来源：http://lq.bjjhwx.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://cc.521024.cn

[Q59] 分组内累计
来源：http://ut.bjjhwx.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://by.yuntaijiaju.cn

[Q60] 取上一行 / 下一行
来源：http://hv.hahajie.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://fp.huixiangedu.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://qn.wgjwhj.cn

[Q61] 移动平均
来源：http://vc.shxzskj.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://qd.newstarts.cn

[Q62] 分组占比
来源：http://tt.9csxet.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://lc.huixinmuqiang.cn

[Q63] 开启事务
来源：http://rh.jianghongdianzi.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://vk.asd995.cn

[Q64] 提交事务
来源：http://hu.bjjhwx.cn

COMMIT;
来源：http://bk.shtwfgs.cn

[Q65] 回滚事务
来源：http://im.bjjhwx.cn

ROLLBACK;
来源：http://ob.asd995.cn

[Q66] 行锁查询
来源：http://cm.shxzskj.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://bf.nszjky.cn

[Q67] 设置隔离级别
来源：http://fw.9csxet.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ec.hahajie.cn

[Q68] 保存点
来源：http://ve.bookmarksfly.cn

SAVEPOINT sp1;
来源：http://pd.asd995.cn

ROLLBACK TO sp1;
来源：http://jd.hahajie.cn

[Q69] 查看执行计划
来源：http://li.newstarts.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://rf.huixiangedu.cn

[Q70] 更新统计信息
来源：http://xq.asd995.cn

ANALYZE TABLE users;
来源：http://ro.muxihuayi.cn

[Q71] 查看建表语句
来源：http://wk.szsharing.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ta.haigaiapp.cn

[Q72] 查看索引
来源：http://ix.colortex.cn

SHOW INDEX FROM users;
来源：http://bs.yuexingan06.cn

[Q73] 查看表状态
来源：http://la.yuexingan06.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://qf.hahajie.cn

[Q74] 强制使用索引
来源：http://sd.bjjhwx.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ct.9csxet.cn

[Q75] 日期格式化
来源：http://eb.lnxyls.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hg.jctech888.com.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://rf.colortex.cn

[Q76] 按天统计
来源：http://rr.haigaiapp.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://vo.shxzukj.cn

[Q77] 时间加减
来源：http://sw.huixiangedu.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ec.muxihuayi.cn

[Q78] 当前时间
来源：http://aq.nicolike.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://rt.nszjky.cn

[Q79] 字符串拼接
来源：http://si.bjjhwx.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hj.asd995.cn

[Q80] 字符串截取
来源：http://ee.yuntaijiaju.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ak.shxzukj.cn

[Q81] 字符串替换
来源：http://po.lnxyls.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://fs.panjiajie.cn

[Q82] 字符长度与字节长度
来源：http://fm.huixiangedu.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://kd.521024.cn

[Q83] 大小写转换
来源：http://fh.wgjwhj.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://xa.9csxet.cn

[Q84] 去除首尾空格
来源：http://yj.shxzskj.cn

SELECT TRIM(name) FROM users;
来源：http://cf.shtwfgs.cn

[Q85] 数值取整
来源：http://rt.shxzukj.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ih.asd995.cn

[Q86] 读取 JSON 字段
来源：http://yd.yuntaijiaju.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://nr.shxzskj.cn

[Q87] JSON 字段做条件
来源：http://sh.521024.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://rf.panjiajie.cn

[Q88] 行转列（条件聚合）
来源：http://mt.chemitech.net.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://yt.bjjhwx.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ju.panjiajie.cn

[Q89] 判断表是否存在
来源：http://xe.asd995.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://nt.asd995.cn

[Q90] 生成序号列
来源：http://qf.asd995.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wj.shxzskj.cn

================================================================================
来源：http://vy.szsharing.cn

R. Bash 专题
来源：http://jx.jctech888.com.cn

================================================================================
来源：http://fr.bjjhwx.cn

[R01] shebang 与严格模式
来源：http://ap.szxytkj.cn

#!/usr/bin/env bash
来源：http://ab.haigaiapp.cn

set -euo pipefail
来源：http://tq.huixiangedu.cn

[R02] 变量赋值与使用
来源：http://na.yuexingan06.cn

name="Tom"; echo "$name"
来源：http://px.hahajie.cn

[R03] 只读变量
来源：http://nh.panjiajie.cn

readonly PI=3.14
来源：http://fi.hahajie.cn

[R04] 位置参数
来源：http://du.lnxyls.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://fc.nszjky.cn

[R05] 参数默认值
来源：http://dl.nicolike.cn

name="${1:-default}"
来源：http://cq.gzmigu.cn

[R06] 判断命令是否存在
来源：http://vj.jctech888.com.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://db.shxzskj.cn

[R07] if 判断文件
来源：http://lx.shxzskj.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://om.nszjky.cn

[R08] 数值比较
来源：http://jx.yuntaijiaju.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://rp.huixinmuqiang.cn

[R09] 字符串比较
来源：http://am.muxihuayi.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wd.yuexingan06.cn

[R10] 正则匹配
来源：http://di.szsharing.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://gh.hahajie.cn

[R11] case 多分支
来源：http://fo.hahajie.cn

case "$1" in
来源：http://jy.bookmarksfly.cn

start) echo "启动" ;;
来源：http://qb.szsharing.cn

stop)  echo "停止" ;;
来源：http://eo.chemitech.net.cn

*)     echo "未知命令" ;;
来源：http://de.gzmigu.cn

esac
来源：http://ac.bookmarksfly.cn

[R12] for 遍历文件
来源：http://aw.huanxung.cn

for f in *.txt; do echo "$f"; done
来源：http://mv.yuexingan06.cn

[R13] for 计数循环
来源：http://di.521024.cn

for i in {1..10}; do echo "$i"; done
来源：http://lm.9csxet.cn

[R14] C 风格 for
来源：http://im.wgjwhj.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://vr.bjjhwx.cn

[R15] while 逐行读文件
来源：http://op.muxihuayi.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://gg.jianghongdianzi.cn

[R16] until 等待条件
来源：http://wa.shtwfgs.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://so.haigaiapp.cn

[R17] 数组定义与取值
来源：http://bh.shtwfgs.cn

arr=(a b c); echo "${arr[0]}"
来源：http://os.bookmarksfly.cn

[R18] 遍历数组
来源：http://et.colortex.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://zy.yuntaijiaju.cn

[R19] 数组长度
来源：http://lc.newstarts.cn

echo "${#arr[@]}"
来源：http://my.newstarts.cn

[R20] 关联数组（字典）
来源：http://us.hahajie.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://fa.bjjhwx.cn

[R21] 字符串长度
来源：http://ml.asd995.cn

echo "${#s}"
来源：http://rf.521024.cn

[R22] 截取子串
来源：http://bl.yuntaijiaju.cn

echo "${s:0:5}"
来源：http://jp.bookmarksfly.cn

[R23] 字符串替换
来源：http://zy.jctech888.com.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://eg.bjjhwx.cn

[R24] 大小写转换
来源：http://ig.hahajie.cn

echo "${s^^}"; echo "${s,,}"
来源：http://rr.nszjky.cn

[R25] 去后缀 / 去前缀
来源：http://ky.jctech888.com.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://st.hahajie.cn

[R26] 命令替换
来源：http://px.gzmigu.cn

now=$(date +%F); echo "$now"
来源：http://rw.bjjhwx.cn

[R27] 算术展开
来源：http://jz.hahajie.cn

echo $((1 + 2 * 3))
来源：http://yv.szxytkj.cn

[R28] 浮点运算
来源：http://ja.muxihuayi.cn

echo "scale=2; 10/3" | bc
来源：http://lz.nicolike.cn

[R29] 定义函数
来源：http://jv.9csxet.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://zb.nszjky.cn

[R30] 函数返回状态码
来源：http://ie.chemitech.net.cn

f() { return 0; }; f || echo "失败了"
来源：http://lx.colortex.cn

[R31] 局部变量
来源：http://ee.newstarts.cn

f() { local x=1; echo "$x"; }
来源：http://hp.gzmigu.cn

[R32] 参数个数校验
来源：http://pu.shtwfgs.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://jj.newstarts.cn

[R33] 捕获错误并提示行号
来源：http://aa.chemitech.net.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mx.haigaiapp.cn

[R34] 退出时清理
来源：http://ng.shxzukj.cn

trap 'rm -f "$tmp"' EXIT
来源：http://ki.muxihuayi.cn

[R35] 后台执行并等待
来源：http://yn.bjjhwx.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://cd.nszjky.cn

[R36] 并发执行多个任务
来源：http://uh.hahajie.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://og.hnjuh.cn

[R37] 把输出赋给变量
来源：http://fl.gzmigu.cn

files=$(ls -1)
来源：http://mj.nszjky.cn

[R38] 管道串联
来源：http://az.huanxung.cn

cat a.txt | grep -i error | wc -l
来源：http://hn.shtwfgs.cn

[R39] 重定向标准输出与错误
来源：http://qq.panjiajie.cn


<!-- 参考信息 -->