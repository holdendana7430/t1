代发 wailian999

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://sm.panjiajie.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://nw.huixiangedu.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://bb.yuexingan06.cn

[P08] 处理浮点精度问题
来源：http://mr.bjjhwx.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://xw.521024.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://xv.nicolike.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://sr.nszjky.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://kh.muxihuayi.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ma.shtwfgs.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://og.haigaiapp.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://vv.colortex.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://gd.shxzukj.cn

================================================================================
来源：http://sq.szsharing.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://kk.colortex.cn

================================================================================
来源：http://qn.asd995.cn

[Q01] 创建表
来源：http://il.huanxung.cn

CREATE TABLE users (
来源：http://fo.jctech888.com.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://dk.9csxet.cn

name VARCHAR(50) NOT NULL,
来源：http://vv.huixinmuqiang.cn

email VARCHAR(100) UNIQUE,
来源：http://qr.9csxet.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ze.newstarts.cn

);
来源：http://si.hnjuh.cn

[Q02] 创建带外键的表
来源：http://pz.jctech888.com.cn

CREATE TABLE orders (
来源：http://od.szxytkj.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://iu.chemitech.net.cn

user_id INT NOT NULL,
来源：http://bw.521024.cn

amount DECIMAL(10, 2),
来源：http://lt.panjiajie.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://er.huanxung.cn

);
来源：http://rn.nszjky.cn

[Q03] 增加列
来源：http://xd.huixiangedu.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://al.chemitech.net.cn

[Q04] 修改列类型
来源：http://se.521024.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mx.yuntaijiaju.cn

[Q05] 重命名列
来源：http://om.huixinmuqiang.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://uc.bjjhwx.cn

[Q06] 删除列
来源：http://xt.chemitech.net.cn

ALTER TABLE users DROP COLUMN age;
来源：http://bz.9csxet.cn

[Q07] 删除表
来源：http://mu.haigaiapp.cn

DROP TABLE IF EXISTS orders;
来源：http://pu.szxytkj.cn

[Q08] 创建普通索引
来源：http://nr.szxytkj.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://xw.lnxyls.cn

[Q09] 创建唯一索引
来源：http://gs.muxihuayi.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://nn.newstarts.cn

[Q10] 插入单行
来源：http://nl.lnxyls.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hw.asd995.cn

[Q11] 一次插入多行
来源：http://tz.lnxyls.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ks.jctech888.com.cn

[Q12] 插入后取自增 ID
来源：http://jf.9csxet.cn

INSERT INTO users (name) VALUES ('C');
来源：http://nq.szxytkj.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://tw.gzmigu.cn

[Q13] 忽略重复插入
来源：http://my.yuexingan06.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://cz.szsharing.cn

[Q14] 存在则更新（upsert）
来源：http://kj.9csxet.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://fz.jianghongdianzi.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hp.jctech888.com.cn

[Q15] 查询全部
来源：http://eo.lnxyls.cn

SELECT * FROM users;
来源：http://sx.bjjhwx.cn

[Q16] 查询指定列
来源：http://ig.gzmigu.cn

SELECT id, name FROM users;
来源：http://io.jctech888.com.cn

[Q17] 条件查询
来源：http://uw.nszjky.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://rd.9csxet.cn

[Q18] 模糊匹配
来源：http://ve.gzmigu.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://jz.shtwfgs.cn

[Q19] 范围查询
来源：http://gl.hnjuh.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ra.muxihuayi.cn

[Q20] IN 列表
来源：http://yt.huixiangedu.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://jw.colortex.cn

[Q21] 空值判断
来源：http://dw.lnxyls.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://eb.shxzukj.cn

[Q22] 排序
来源：http://jj.shxzskj.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://he.bjjhwx.cn

[Q23] 分页
来源：http://hr.nicolike.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://qv.nicolike.cn

[Q24] 去重
来源：http://sh.huanxung.cn

SELECT DISTINCT city FROM users;
来源：http://qb.bjjhwx.cn

[Q25] 只取前 N 条
来源：http://li.huixiangedu.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ml.9csxet.cn

[Q26] 计数
来源：http://cg.gzmigu.cn

SELECT COUNT(*) FROM users;
来源：http://vl.huixinmuqiang.cn

[Q27] 条件计数
来源：http://zr.szsharing.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://my.shxzskj.cn

[Q28] 求和与平均
来源：http://zo.huixiangedu.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://ha.asd995.cn

[Q29] 最大最小值
来源：http://yv.yuntaijiaju.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://qr.bjjhwx.cn

[Q30] 分组统计
来源：http://ih.huixinmuqiang.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://sz.shxzskj.cn

[Q31] 分组后过滤
来源：http://jr.shxzukj.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://eu.hnjuh.cn

[Q32] 分组拼接字符串
来源：http://wh.szsharing.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://rd.huixinmuqiang.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://gu.shtwfgs.cn

[Q33] 多列分组
来源：http://jx.szsharing.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://uv.521024.cn

[Q34] 每组取第一条
来源：http://zx.asd995.cn

SELECT * FROM (
来源：http://qt.huixiangedu.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://fl.huixiangedu.cn

) t WHERE rn = 1;
来源：http://qy.colortex.cn

[Q35] 内连接
来源：http://cs.panjiajie.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://tr.szsharing.cn

[Q36] 左连接
来源：http://jr.shxzskj.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://iv.huanxung.cn

[Q37] 右连接
来源：http://sa.huanxung.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ky.newstarts.cn

[Q38] 全外连接（PostgreSQL）
来源：http://ks.bjjhwx.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ds.yuexingan06.cn

[Q39] 自连接（查上下级）
来源：http://pw.shxzukj.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://eu.huanxung.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://pa.nszjky.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://bo.bookmarksfly.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://in.haigaiapp.cn

[Q41] 多表连接
来源：http://il.hnjuh.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://bv.jctech888.com.cn

JOIN users u ON u.id = o.user_id
来源：http://kw.szsharing.cn

JOIN products p ON p.id = o.product_id;
来源：http://ca.bookmarksfly.cn

[Q42] 连接条件附加过滤
来源：http://ff.shxzukj.cn

SELECT u.name, o.amount FROM users u
来源：http://hs.szsharing.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wh.9csxet.cn

[Q43] 标量子查询
来源：http://ta.colortex.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://bw.colortex.cn

[Q44] IN 子查询
来源：http://lr.shxzukj.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://si.colortex.cn

[Q45] EXISTS 判断存在
来源：http://dn.jianghongdianzi.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ac.szxytkj.cn

[Q46] NOT EXISTS 判断不存在
来源：http://bs.newstarts.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://yw.lnxyls.cn

[Q47] 与平均值比较
来源：http://dq.shxzskj.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://oh.shxzukj.cn

[Q48] CTE 公用表表达式
来源：http://gk.shxzskj.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://xz.9csxet.cn

SELECT * FROM t WHERE c > 5;
来源：http://tm.hnjuh.cn

[Q49] 更新单行
来源：http://vk.bjjhwx.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://su.yuexingan06.cn

[Q50] 批量更新
来源：http://si.lnxyls.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://or.asd995.cn

[Q51] 用子查询更新
来源：http://vk.colortex.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://my.hahajie.cn

[Q52] 删除指定行
来源：http://wi.hahajie.cn

DELETE FROM users WHERE id = 10;
来源：http://gm.huanxung.cn

[Q53] 按条件删除
来源：http://xu.nicolike.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://qr.muxihuayi.cn

[Q54] 清空表
来源：http://rp.shxzukj.cn

TRUNCATE TABLE logs;
来源：http://cz.asd995.cn

[Q55] 排名（并列占位）
来源：http://ba.shxzskj.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://yj.newstarts.cn

[Q56] 密集排名（并列不占位）
来源：http://if.huixiangedu.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ix.shtwfgs.cn

[Q57] 行号
来源：http://ft.shxzukj.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://de.szsharing.cn

[Q58] 累计求和
来源：http://zc.hahajie.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://lo.9csxet.cn

[Q59] 分组内累计
来源：http://ha.jianghongdianzi.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://oo.chemitech.net.cn

[Q60] 取上一行 / 下一行
来源：http://lf.hnjuh.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://nx.panjiajie.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ws.haigaiapp.cn

[Q61] 移动平均
来源：http://pg.huixinmuqiang.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://re.szsharing.cn

[Q62] 分组占比
来源：http://mn.chemitech.net.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://on.chemitech.net.cn

[Q63] 开启事务
来源：http://he.huixiangedu.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://yg.szxytkj.cn

[Q64] 提交事务
来源：http://vi.huixinmuqiang.cn

COMMIT;
来源：http://bm.nicolike.cn

[Q65] 回滚事务
来源：http://bi.shtwfgs.cn

ROLLBACK;
来源：http://vc.9csxet.cn

[Q66] 行锁查询
来源：http://tm.wgjwhj.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://dg.newstarts.cn

[Q67] 设置隔离级别
来源：http://mm.asd995.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wn.shxzukj.cn

[Q68] 保存点
来源：http://vv.hahajie.cn

SAVEPOINT sp1;
来源：http://ls.szxytkj.cn

ROLLBACK TO sp1;
来源：http://be.hnjuh.cn

[Q69] 查看执行计划
来源：http://hi.gzmigu.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://xp.yuntaijiaju.cn

[Q70] 更新统计信息
来源：http://kf.shtwfgs.cn

ANALYZE TABLE users;
来源：http://es.shtwfgs.cn

[Q71] 查看建表语句
来源：http://xw.nszjky.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://cb.panjiajie.cn

[Q72] 查看索引
来源：http://oq.shtwfgs.cn

SHOW INDEX FROM users;
来源：http://pw.yuntaijiaju.cn

[Q73] 查看表状态
来源：http://hk.nszjky.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://hw.bjjhwx.cn

[Q74] 强制使用索引
来源：http://av.yuexingan06.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://qy.huixiangedu.cn

[Q75] 日期格式化
来源：http://eu.bjjhwx.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://jx.shxzskj.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://dw.jianghongdianzi.cn

[Q76] 按天统计
来源：http://fe.9csxet.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://rd.wgjwhj.cn

[Q77] 时间加减
来源：http://jk.jianghongdianzi.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://aq.haigaiapp.cn

[Q78] 当前时间
来源：http://ll.chemitech.net.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hx.huixinmuqiang.cn

[Q79] 字符串拼接
来源：http://ra.gzmigu.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://vp.hnjuh.cn

[Q80] 字符串截取
来源：http://bu.yuexingan06.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://lc.chemitech.net.cn

[Q81] 字符串替换
来源：http://tn.shxzukj.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://sz.szxytkj.cn

[Q82] 字符长度与字节长度
来源：http://zp.shtwfgs.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://nd.huanxung.cn

[Q83] 大小写转换
来源：http://qf.bjjhwx.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://vb.jctech888.com.cn

[Q84] 去除首尾空格
来源：http://ss.huanxung.cn

SELECT TRIM(name) FROM users;
来源：http://ni.bjjhwx.cn

[Q85] 数值取整
来源：http://zi.nszjky.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://xt.haigaiapp.cn

[Q86] 读取 JSON 字段
来源：http://gm.yuexingan06.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://jj.jianghongdianzi.cn

[Q87] JSON 字段做条件
来源：http://di.newstarts.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ls.nicolike.cn

[Q88] 行转列（条件聚合）
来源：http://bq.szsharing.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://te.shtwfgs.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://iz.chemitech.net.cn

[Q89] 判断表是否存在
来源：http://mm.szsharing.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://np.hnjuh.cn

[Q90] 生成序号列
来源：http://fw.chemitech.net.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://pe.asd995.cn

================================================================================
来源：http://dh.chemitech.net.cn

R. Bash 专题
来源：http://py.huixinmuqiang.cn

================================================================================
来源：http://tj.yuexingan06.cn

[R01] shebang 与严格模式
来源：http://lb.521024.cn

#!/usr/bin/env bash
来源：http://bq.chemitech.net.cn

set -euo pipefail
来源：http://fn.yuexingan06.cn

[R02] 变量赋值与使用
来源：http://fu.panjiajie.cn

name="Tom"; echo "$name"
来源：http://wn.lnxyls.cn

[R03] 只读变量
来源：http://yi.huixiangedu.cn

readonly PI=3.14
来源：http://vn.huanxung.cn

[R04] 位置参数
来源：http://nb.9csxet.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://od.yuexingan06.cn

[R05] 参数默认值
来源：http://qt.haigaiapp.cn

name="${1:-default}"
来源：http://hv.bjjhwx.cn

[R06] 判断命令是否存在
来源：http://db.shxzukj.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hc.szsharing.cn

[R07] if 判断文件
来源：http://up.panjiajie.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://nu.szxytkj.cn

[R08] 数值比较
来源：http://kg.lnxyls.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://iu.nicolike.cn

[R09] 字符串比较
来源：http://ct.yuexingan06.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://jq.panjiajie.cn

[R10] 正则匹配
来源：http://el.szxytkj.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://kp.bjjhwx.cn

[R11] case 多分支
来源：http://an.lnxyls.cn

case "$1" in
来源：http://rp.yuntaijiaju.cn

start) echo "启动" ;;
来源：http://eg.gzmigu.cn

stop)  echo "停止" ;;
来源：http://ua.yuexingan06.cn

*)     echo "未知命令" ;;
来源：http://lm.shtwfgs.cn

esac
来源：http://vd.szxytkj.cn

[R12] for 遍历文件
来源：http://lo.hnjuh.cn

for f in *.txt; do echo "$f"; done
来源：http://hd.huanxung.cn

[R13] for 计数循环
来源：http://it.jctech888.com.cn

for i in {1..10}; do echo "$i"; done
来源：http://rc.szxytkj.cn

[R14] C 风格 for
来源：http://ma.muxihuayi.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://di.hnjuh.cn

[R15] while 逐行读文件
来源：http://oq.szsharing.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://py.yuexingan06.cn

[R16] until 等待条件
来源：http://ue.521024.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ij.huixiangedu.cn

[R17] 数组定义与取值
来源：http://mk.bookmarksfly.cn

arr=(a b c); echo "${arr[0]}"
来源：http://iv.bookmarksfly.cn

[R18] 遍历数组
来源：http://tr.bjjhwx.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ez.muxihuayi.cn

[R19] 数组长度
来源：http://vm.hahajie.cn

echo "${#arr[@]}"
来源：http://dn.haigaiapp.cn

[R20] 关联数组（字典）
来源：http://ip.muxihuayi.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://zv.shxzukj.cn

[R21] 字符串长度
来源：http://cf.521024.cn

echo "${#s}"
来源：http://pd.yuexingan06.cn

[R22] 截取子串
来源：http://xa.szxytkj.cn

echo "${s:0:5}"
来源：http://ma.9csxet.cn

[R23] 字符串替换
来源：http://br.bjjhwx.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://df.yuexingan06.cn

[R24] 大小写转换
来源：http://tz.newstarts.cn

echo "${s^^}"; echo "${s,,}"
来源：http://gn.asd995.cn

[R25] 去后缀 / 去前缀
来源：http://oz.lnxyls.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://ci.huixiangedu.cn

[R26] 命令替换
来源：http://oa.gzmigu.cn

now=$(date +%F); echo "$now"
来源：http://io.muxihuayi.cn

[R27] 算术展开
来源：http://zc.hnjuh.cn

echo $((1 + 2 * 3))
来源：http://qc.nszjky.cn

[R28] 浮点运算
来源：http://xq.521024.cn

echo "scale=2; 10/3" | bc
来源：http://yf.hnjuh.cn

[R29] 定义函数
来源：http://od.nicolike.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://tj.lnxyls.cn

[R30] 函数返回状态码
来源：http://yt.chemitech.net.cn

f() { return 0; }; f || echo "失败了"
来源：http://md.haigaiapp.cn

[R31] 局部变量
来源：http://nq.gzmigu.cn

f() { local x=1; echo "$x"; }
来源：http://pc.lnxyls.cn

[R32] 参数个数校验
来源：http://ef.muxihuayi.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://zx.huixinmuqiang.cn

[R33] 捕获错误并提示行号
来源：http://em.hahajie.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ll.bookmarksfly.cn

[R34] 退出时清理
来源：http://xo.asd995.cn

trap 'rm -f "$tmp"' EXIT
来源：http://ud.bjjhwx.cn

[R35] 后台执行并等待
来源：http://zq.lnxyls.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://yw.jctech888.com.cn

[R36] 并发执行多个任务
来源：http://ay.muxihuayi.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hd.asd995.cn

[R37] 把输出赋给变量
来源：http://hu.asd995.cn


<!-- 参考信息 -->