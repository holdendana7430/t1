代发 wailian999

PHP:  // 手写时间戳比较
来源：http://gp.bjjhwx.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wk.nicolike.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://tn.shxzskj.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ak.szsharing.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://os.lnxyls.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://fe.shtwfgs.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://cu.nszjky.cn

[P08] 处理浮点精度问题
来源：http://ki.gzmigu.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ot.bookmarksfly.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ew.hahajie.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://cl.shxzskj.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://jq.wgjwhj.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://nk.muxihuayi.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://la.yuntaijiaju.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://jt.9csxet.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://jp.szxytkj.cn

================================================================================
来源：http://rv.szsharing.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://do.asd995.cn

================================================================================
来源：http://qo.jianghongdianzi.cn

[Q01] 创建表
来源：http://ih.panjiajie.cn

CREATE TABLE users (
来源：http://mf.9csxet.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wq.hahajie.cn

name VARCHAR(50) NOT NULL,
来源：http://nh.bjjhwx.cn

email VARCHAR(100) UNIQUE,
来源：http://mz.nszjky.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://vy.szsharing.cn

);
来源：http://vj.szxytkj.cn

[Q02] 创建带外键的表
来源：http://gc.newstarts.cn

CREATE TABLE orders (
来源：http://oi.shtwfgs.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://fj.bookmarksfly.cn

user_id INT NOT NULL,
来源：http://xo.muxihuayi.cn

amount DECIMAL(10, 2),
来源：http://gy.shxzukj.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mw.hahajie.cn

);
来源：http://mk.hnjuh.cn

[Q03] 增加列
来源：http://kz.huixiangedu.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://tq.shxzskj.cn

[Q04] 修改列类型
来源：http://kt.521024.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://pg.bookmarksfly.cn

[Q05] 重命名列
来源：http://td.shxzskj.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hl.shtwfgs.cn

[Q06] 删除列
来源：http://tc.gzmigu.cn

ALTER TABLE users DROP COLUMN age;
来源：http://op.asd995.cn

[Q07] 删除表
来源：http://dn.9csxet.cn

DROP TABLE IF EXISTS orders;
来源：http://zo.yuntaijiaju.cn

[Q08] 创建普通索引
来源：http://sk.9csxet.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://vi.asd995.cn

[Q09] 创建唯一索引
来源：http://ql.chemitech.net.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://fs.huixinmuqiang.cn

[Q10] 插入单行
来源：http://na.yuexingan06.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ay.huixiangedu.cn

[Q11] 一次插入多行
来源：http://qr.lnxyls.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ri.szxytkj.cn

[Q12] 插入后取自增 ID
来源：http://hl.shxzukj.cn

INSERT INTO users (name) VALUES ('C');
来源：http://ee.muxihuayi.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://qv.bookmarksfly.cn

[Q13] 忽略重复插入
来源：http://ut.szsharing.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ey.521024.cn

[Q14] 存在则更新（upsert）
来源：http://jr.huanxung.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://fq.chemitech.net.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://yp.9csxet.cn

[Q15] 查询全部
来源：http://ll.jianghongdianzi.cn

SELECT * FROM users;
来源：http://te.szxytkj.cn

[Q16] 查询指定列
来源：http://zp.shxzskj.cn

SELECT id, name FROM users;
来源：http://ha.szsharing.cn

[Q17] 条件查询
来源：http://wm.asd995.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://fk.shxzskj.cn

[Q18] 模糊匹配
来源：http://qt.shxzskj.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://oo.chemitech.net.cn

[Q19] 范围查询
来源：http://qh.hnjuh.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://la.asd995.cn

[Q20] IN 列表
来源：http://ih.nicolike.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wc.szsharing.cn

[Q21] 空值判断
来源：http://wi.asd995.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://yl.szxytkj.cn

[Q22] 排序
来源：http://ax.shtwfgs.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://kg.shxzukj.cn

[Q23] 分页
来源：http://oi.panjiajie.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://zd.newstarts.cn

[Q24] 去重
来源：http://ir.jctech888.com.cn

SELECT DISTINCT city FROM users;
来源：http://ss.szsharing.cn

[Q25] 只取前 N 条
来源：http://rs.nszjky.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://gs.shxzskj.cn

[Q26] 计数
来源：http://tq.huixinmuqiang.cn

SELECT COUNT(*) FROM users;
来源：http://qj.haigaiapp.cn

[Q27] 条件计数
来源：http://jb.shtwfgs.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hl.jctech888.com.cn

[Q28] 求和与平均
来源：http://hi.bookmarksfly.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://xo.521024.cn

[Q29] 最大最小值
来源：http://ch.bookmarksfly.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://ou.yuntaijiaju.cn

[Q30] 分组统计
来源：http://hv.jctech888.com.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://la.bookmarksfly.cn

[Q31] 分组后过滤
来源：http://yp.szsharing.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://sk.shtwfgs.cn

[Q32] 分组拼接字符串
来源：http://ye.yuexingan06.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://sx.yuexingan06.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://cf.bjjhwx.cn

[Q33] 多列分组
来源：http://fb.wgjwhj.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://iq.panjiajie.cn

[Q34] 每组取第一条
来源：http://ua.shxzskj.cn

SELECT * FROM (
来源：http://do.asd995.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://gb.nicolike.cn

) t WHERE rn = 1;
来源：http://cg.asd995.cn

[Q35] 内连接
来源：http://ig.asd995.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://so.jianghongdianzi.cn

[Q36] 左连接
来源：http://qs.haigaiapp.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://vk.szsharing.cn

[Q37] 右连接
来源：http://nz.yuexingan06.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://zo.haigaiapp.cn

[Q38] 全外连接（PostgreSQL）
来源：http://bc.yuexingan06.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://vi.bookmarksfly.cn

[Q39] 自连接（查上下级）
来源：http://hx.shtwfgs.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://mh.panjiajie.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ek.bookmarksfly.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://os.huixinmuqiang.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://jg.hnjuh.cn

[Q41] 多表连接
来源：http://jz.szsharing.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://vo.bjjhwx.cn

JOIN users u ON u.id = o.user_id
来源：http://tc.shxzukj.cn

JOIN products p ON p.id = o.product_id;
来源：http://eu.yuntaijiaju.cn

[Q42] 连接条件附加过滤
来源：http://wg.newstarts.cn

SELECT u.name, o.amount FROM users u
来源：http://wm.nszjky.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://lq.gzmigu.cn

[Q43] 标量子查询
来源：http://qv.hahajie.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://fj.shxzskj.cn

[Q44] IN 子查询
来源：http://te.panjiajie.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ct.huixinmuqiang.cn

[Q45] EXISTS 判断存在
来源：http://bp.huanxung.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ao.shtwfgs.cn

[Q46] NOT EXISTS 判断不存在
来源：http://pv.huixiangedu.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hc.haigaiapp.cn

[Q47] 与平均值比较
来源：http://th.gzmigu.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ol.szxytkj.cn

[Q48] CTE 公用表表达式
来源：http://qq.muxihuayi.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://si.shtwfgs.cn

SELECT * FROM t WHERE c > 5;
来源：http://lt.hahajie.cn

[Q49] 更新单行
来源：http://aw.nicolike.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ly.521024.cn

[Q50] 批量更新
来源：http://rn.521024.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://vr.szxytkj.cn

[Q51] 用子查询更新
来源：http://od.asd995.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://oz.521024.cn

[Q52] 删除指定行
来源：http://up.szsharing.cn

DELETE FROM users WHERE id = 10;
来源：http://ft.yuexingan06.cn

[Q53] 按条件删除
来源：http://ji.jianghongdianzi.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://nb.hnjuh.cn

[Q54] 清空表
来源：http://oz.asd995.cn

TRUNCATE TABLE logs;
来源：http://ez.nicolike.cn

[Q55] 排名（并列占位）
来源：http://xs.huixinmuqiang.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://li.wgjwhj.cn

[Q56] 密集排名（并列不占位）
来源：http://ii.nszjky.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ab.chemitech.net.cn

[Q57] 行号
来源：http://xy.shxzskj.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://rs.jctech888.com.cn

[Q58] 累计求和
来源：http://eh.shxzskj.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://oy.nicolike.cn

[Q59] 分组内累计
来源：http://qb.shxzskj.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mr.bjjhwx.cn

[Q60] 取上一行 / 下一行
来源：http://bv.jctech888.com.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://dt.jianghongdianzi.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ln.szxytkj.cn

[Q61] 移动平均
来源：http://mi.shxzukj.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://iq.gzmigu.cn

[Q62] 分组占比
来源：http://wv.szsharing.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ck.shxzukj.cn

[Q63] 开启事务
来源：http://ht.haigaiapp.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://ka.nicolike.cn

[Q64] 提交事务
来源：http://hp.jctech888.com.cn

COMMIT;
来源：http://id.newstarts.cn

[Q65] 回滚事务
来源：http://nu.9csxet.cn

ROLLBACK;
来源：http://jk.jianghongdianzi.cn

[Q66] 行锁查询
来源：http://np.gzmigu.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://sn.shxzukj.cn

[Q67] 设置隔离级别
来源：http://dg.wgjwhj.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://pn.gzmigu.cn

[Q68] 保存点
来源：http://rq.shtwfgs.cn

SAVEPOINT sp1;
来源：http://ms.nszjky.cn

ROLLBACK TO sp1;
来源：http://dk.nszjky.cn

[Q69] 查看执行计划
来源：http://vn.colortex.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://js.huanxung.cn

[Q70] 更新统计信息
来源：http://gh.bookmarksfly.cn

ANALYZE TABLE users;
来源：http://ob.bookmarksfly.cn

[Q71] 查看建表语句
来源：http://xq.hnjuh.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://sh.bjjhwx.cn

[Q72] 查看索引
来源：http://vr.panjiajie.cn

SHOW INDEX FROM users;
来源：http://od.jctech888.com.cn

[Q73] 查看表状态
来源：http://lb.nicolike.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://ir.shxzskj.cn

[Q74] 强制使用索引
来源：http://xg.newstarts.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://bi.szsharing.cn

[Q75] 日期格式化
来源：http://nb.huixiangedu.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mz.jianghongdianzi.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://zj.asd995.cn

[Q76] 按天统计
来源：http://fb.huixinmuqiang.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://yl.hnjuh.cn

[Q77] 时间加减
来源：http://mn.lnxyls.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://nf.hahajie.cn

[Q78] 当前时间
来源：http://yh.panjiajie.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ne.bjjhwx.cn

[Q79] 字符串拼接
来源：http://xb.yuntaijiaju.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://gj.szsharing.cn

[Q80] 字符串截取
来源：http://bi.shxzukj.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ny.szxytkj.cn

[Q81] 字符串替换
来源：http://uh.hahajie.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ma.asd995.cn

[Q82] 字符长度与字节长度
来源：http://ro.haigaiapp.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://am.nicolike.cn

[Q83] 大小写转换
来源：http://st.shxzskj.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://zn.gzmigu.cn

[Q84] 去除首尾空格
来源：http://sp.bjjhwx.cn

SELECT TRIM(name) FROM users;
来源：http://ou.9csxet.cn

[Q85] 数值取整
来源：http://io.huixiangedu.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wl.colortex.cn

[Q86] 读取 JSON 字段
来源：http://bu.hahajie.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://se.gzmigu.cn

[Q87] JSON 字段做条件
来源：http://zs.newstarts.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://rb.haigaiapp.cn

[Q88] 行转列（条件聚合）
来源：http://ac.gzmigu.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://qj.shxzukj.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ls.szxytkj.cn

[Q89] 判断表是否存在
来源：http://im.9csxet.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ll.lnxyls.cn

[Q90] 生成序号列
来源：http://js.panjiajie.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ry.gzmigu.cn

================================================================================
来源：http://kh.wgjwhj.cn

R. Bash 专题
来源：http://rh.jctech888.com.cn

================================================================================
来源：http://yi.asd995.cn

[R01] shebang 与严格模式
来源：http://jb.shxzukj.cn

#!/usr/bin/env bash
来源：http://zh.panjiajie.cn

set -euo pipefail
来源：http://ly.panjiajie.cn

[R02] 变量赋值与使用
来源：http://uf.chemitech.net.cn

name="Tom"; echo "$name"
来源：http://ge.muxihuayi.cn

[R03] 只读变量
来源：http://er.shxzskj.cn

readonly PI=3.14
来源：http://cc.huanxung.cn

[R04] 位置参数
来源：http://wx.szsharing.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://pt.colortex.cn

[R05] 参数默认值
来源：http://kh.yuexingan06.cn

name="${1:-default}"
来源：http://ao.chemitech.net.cn

[R06] 判断命令是否存在
来源：http://zu.gzmigu.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://yq.jianghongdianzi.cn

[R07] if 判断文件
来源：http://ua.asd995.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://jy.gzmigu.cn

[R08] 数值比较
来源：http://rv.521024.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://bg.hahajie.cn

[R09] 字符串比较
来源：http://vp.yuntaijiaju.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://bh.nicolike.cn

[R10] 正则匹配
来源：http://zb.gzmigu.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ls.szxytkj.cn

[R11] case 多分支
来源：http://ji.9csxet.cn

case "$1" in
来源：http://jf.nicolike.cn

start) echo "启动" ;;
来源：http://nj.bjjhwx.cn

stop)  echo "停止" ;;
来源：http://lh.yuexingan06.cn

*)     echo "未知命令" ;;
来源：http://wy.szsharing.cn

esac
来源：http://wz.yuexingan06.cn

[R12] for 遍历文件
来源：http://ox.asd995.cn

for f in *.txt; do echo "$f"; done
来源：http://qo.newstarts.cn

[R13] for 计数循环
来源：http://eb.hnjuh.cn

for i in {1..10}; do echo "$i"; done
来源：http://ql.nicolike.cn

[R14] C 风格 for
来源：http://nq.szsharing.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ho.chemitech.net.cn

[R15] while 逐行读文件
来源：http://yc.szxytkj.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ik.huixiangedu.cn

[R16] until 等待条件
来源：http://cj.chemitech.net.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://fn.huanxung.cn

[R17] 数组定义与取值
来源：http://sv.haigaiapp.cn

arr=(a b c); echo "${arr[0]}"
来源：http://xl.colortex.cn

[R18] 遍历数组
来源：http://ow.asd995.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://zn.nicolike.cn

[R19] 数组长度
来源：http://zv.haigaiapp.cn

echo "${#arr[@]}"
来源：http://rh.521024.cn

[R20] 关联数组（字典）
来源：http://wj.bjjhwx.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://yl.9csxet.cn

[R21] 字符串长度
来源：http://cu.shtwfgs.cn

echo "${#s}"
来源：http://pd.szsharing.cn

[R22] 截取子串
来源：http://uj.wgjwhj.cn

echo "${s:0:5}"
来源：http://tp.bjjhwx.cn

[R23] 字符串替换
来源：http://mr.panjiajie.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://xu.chemitech.net.cn

[R24] 大小写转换
来源：http://co.jianghongdianzi.cn

echo "${s^^}"; echo "${s,,}"
来源：http://et.jctech888.com.cn

[R25] 去后缀 / 去前缀
来源：http://dn.521024.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://sr.shxzskj.cn

[R26] 命令替换
来源：http://or.hahajie.cn

now=$(date +%F); echo "$now"
来源：http://lc.shxzukj.cn

[R27] 算术展开
来源：http://nm.shxzukj.cn

echo $((1 + 2 * 3))
来源：http://im.bjjhwx.cn

[R28] 浮点运算
来源：http://lg.szxytkj.cn

echo "scale=2; 10/3" | bc
来源：http://uf.szxytkj.cn

[R29] 定义函数
来源：http://wm.shxzukj.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://jy.chemitech.net.cn

[R30] 函数返回状态码
来源：http://iz.newstarts.cn

f() { return 0; }; f || echo "失败了"
来源：http://wr.szsharing.cn

[R31] 局部变量
来源：http://xz.lnxyls.cn

f() { local x=1; echo "$x"; }
来源：http://ck.jianghongdianzi.cn

[R32] 参数个数校验
来源：http://ho.shtwfgs.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wx.shxzskj.cn

[R33] 捕获错误并提示行号
来源：http://qc.jctech888.com.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://vk.shxzukj.cn

[R34] 退出时清理
来源：http://yt.panjiajie.cn

trap 'rm -f "$tmp"' EXIT
来源：http://xy.yuntaijiaju.cn

[R35] 后台执行并等待
来源：http://qv.jianghongdianzi.cn


<!-- 参考信息 -->