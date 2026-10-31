代发 wailian999

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ew.shxzskj.cn

C#:   if (x is null) {}
来源：http://et.wgjwhj.cn

[P07] 防抖与节流
来源：http://bi.chemitech.net.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://qn.jianghongdianzi.cn

PHP:  // 手写时间戳比较
来源：http://or.colortex.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://xu.wgjwhj.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wr.huixinmuqiang.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://vv.nicolike.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ge.9csxet.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://jr.shxzukj.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://fa.huixinmuqiang.cn

[P08] 处理浮点精度问题
来源：http://ya.bjjhwx.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://fl.szxytkj.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://bn.hnjuh.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://pf.asd995.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ji.nszjky.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://pj.shtwfgs.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://iy.huixiangedu.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://re.newstarts.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://yf.shxzukj.cn

================================================================================
来源：http://em.chemitech.net.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://on.haigaiapp.cn

================================================================================
来源：http://es.haigaiapp.cn

[Q01] 创建表
来源：http://zk.chemitech.net.cn

CREATE TABLE users (
来源：http://kn.hahajie.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://cu.muxihuayi.cn

name VARCHAR(50) NOT NULL,
来源：http://do.szxytkj.cn

email VARCHAR(100) UNIQUE,
来源：http://qh.wgjwhj.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://il.wgjwhj.cn

);
来源：http://ck.chemitech.net.cn

[Q02] 创建带外键的表
来源：http://qi.521024.cn

CREATE TABLE orders (
来源：http://kn.shtwfgs.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://gl.haigaiapp.cn

user_id INT NOT NULL,
来源：http://oz.colortex.cn

amount DECIMAL(10, 2),
来源：http://nc.shtwfgs.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://xj.nszjky.cn

);
来源：http://ms.9csxet.cn

[Q03] 增加列
来源：http://nw.huanxung.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ix.yuntaijiaju.cn

[Q04] 修改列类型
来源：http://ru.huanxung.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://zh.shxzskj.cn

[Q05] 重命名列
来源：http://ne.shtwfgs.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://tp.szxytkj.cn

[Q06] 删除列
来源：http://wx.9csxet.cn

ALTER TABLE users DROP COLUMN age;
来源：http://db.huanxung.cn

[Q07] 删除表
来源：http://eo.wgjwhj.cn

DROP TABLE IF EXISTS orders;
来源：http://vm.huanxung.cn

[Q08] 创建普通索引
来源：http://cf.hahajie.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://mk.newstarts.cn

[Q09] 创建唯一索引
来源：http://ii.nszjky.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://jj.szxytkj.cn

[Q10] 插入单行
来源：http://ln.hnjuh.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://py.hnjuh.cn

[Q11] 一次插入多行
来源：http://fl.huixiangedu.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ne.9csxet.cn

[Q12] 插入后取自增 ID
来源：http://wl.haigaiapp.cn

INSERT INTO users (name) VALUES ('C');
来源：http://ud.huixiangedu.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://fm.newstarts.cn

[Q13] 忽略重复插入
来源：http://nz.wgjwhj.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://kz.huanxung.cn

[Q14] 存在则更新（upsert）
来源：http://tf.wgjwhj.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ax.szsharing.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://yd.wgjwhj.cn

[Q15] 查询全部
来源：http://ee.bjjhwx.cn

SELECT * FROM users;
来源：http://ox.shxzukj.cn

[Q16] 查询指定列
来源：http://yn.wgjwhj.cn

SELECT id, name FROM users;
来源：http://qb.521024.cn

[Q17] 条件查询
来源：http://pc.lnxyls.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wg.haigaiapp.cn

[Q18] 模糊匹配
来源：http://kh.huixinmuqiang.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://oc.haigaiapp.cn

[Q19] 范围查询
来源：http://na.gzmigu.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wc.panjiajie.cn

[Q20] IN 列表
来源：http://ap.jctech888.com.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://yt.lnxyls.cn

[Q21] 空值判断
来源：http://fo.hnjuh.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://pt.jctech888.com.cn

[Q22] 排序
来源：http://ft.szsharing.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://eh.huixiangedu.cn

[Q23] 分页
来源：http://my.chemitech.net.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://vf.gzmigu.cn

[Q24] 去重
来源：http://hn.nicolike.cn

SELECT DISTINCT city FROM users;
来源：http://gv.hahajie.cn

[Q25] 只取前 N 条
来源：http://wq.521024.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ht.shxzskj.cn

[Q26] 计数
来源：http://fl.szxytkj.cn

SELECT COUNT(*) FROM users;
来源：http://jp.huixiangedu.cn

[Q27] 条件计数
来源：http://kr.szxytkj.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://xa.nicolike.cn

[Q28] 求和与平均
来源：http://rf.chemitech.net.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://fd.jianghongdianzi.cn

[Q29] 最大最小值
来源：http://ri.shtwfgs.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://cs.huanxung.cn

[Q30] 分组统计
来源：http://ef.gzmigu.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://px.wgjwhj.cn

[Q31] 分组后过滤
来源：http://ls.hahajie.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://pf.gzmigu.cn

[Q32] 分组拼接字符串
来源：http://dl.gzmigu.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://uj.muxihuayi.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ri.lnxyls.cn

[Q33] 多列分组
来源：http://yq.521024.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://cp.newstarts.cn

[Q34] 每组取第一条
来源：http://on.panjiajie.cn

SELECT * FROM (
来源：http://eq.nicolike.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://cm.gzmigu.cn

) t WHERE rn = 1;
来源：http://gf.shxzskj.cn

[Q35] 内连接
来源：http://nl.hahajie.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://bv.huixinmuqiang.cn

[Q36] 左连接
来源：http://fr.hnjuh.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ql.huanxung.cn

[Q37] 右连接
来源：http://qj.haigaiapp.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://iy.521024.cn

[Q38] 全外连接（PostgreSQL）
来源：http://ys.yuexingan06.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://jf.9csxet.cn

[Q39] 自连接（查上下级）
来源：http://kf.huanxung.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://pa.asd995.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ds.521024.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://ci.shxzukj.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mj.asd995.cn

[Q41] 多表连接
来源：http://fa.shtwfgs.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://mu.szsharing.cn

JOIN users u ON u.id = o.user_id
来源：http://pj.shxzukj.cn

JOIN products p ON p.id = o.product_id;
来源：http://uw.bookmarksfly.cn

[Q42] 连接条件附加过滤
来源：http://kb.szsharing.cn

SELECT u.name, o.amount FROM users u
来源：http://ax.nicolike.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://oh.szsharing.cn

[Q43] 标量子查询
来源：http://wn.huixiangedu.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://er.panjiajie.cn

[Q44] IN 子查询
来源：http://ik.shtwfgs.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ar.shxzukj.cn

[Q45] EXISTS 判断存在
来源：http://hp.yuntaijiaju.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hx.jctech888.com.cn

[Q46] NOT EXISTS 判断不存在
来源：http://vm.panjiajie.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://rp.hnjuh.cn

[Q47] 与平均值比较
来源：http://jt.chemitech.net.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://yr.chemitech.net.cn

[Q48] CTE 公用表表达式
来源：http://ie.jianghongdianzi.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://dl.hahajie.cn

SELECT * FROM t WHERE c > 5;
来源：http://rf.nicolike.cn

[Q49] 更新单行
来源：http://zb.colortex.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://es.yuexingan06.cn

[Q50] 批量更新
来源：http://tz.huixiangedu.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://jb.yuntaijiaju.cn

[Q51] 用子查询更新
来源：http://tr.hahajie.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://yn.jianghongdianzi.cn

[Q52] 删除指定行
来源：http://vb.asd995.cn

DELETE FROM users WHERE id = 10;
来源：http://jk.panjiajie.cn

[Q53] 按条件删除
来源：http://nm.bjjhwx.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://zo.jctech888.com.cn

[Q54] 清空表
来源：http://rf.huixiangedu.cn

TRUNCATE TABLE logs;
来源：http://wk.gzmigu.cn

[Q55] 排名（并列占位）
来源：http://ke.wgjwhj.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://vh.wgjwhj.cn

[Q56] 密集排名（并列不占位）
来源：http://ya.bjjhwx.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ya.shxzskj.cn

[Q57] 行号
来源：http://mk.chemitech.net.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://sv.nicolike.cn

[Q58] 累计求和
来源：http://kd.haigaiapp.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hj.bjjhwx.cn

[Q59] 分组内累计
来源：http://zn.wgjwhj.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://tc.yuexingan06.cn

[Q60] 取上一行 / 下一行
来源：http://nf.shxzukj.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://fj.bjjhwx.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ih.szsharing.cn

[Q61] 移动平均
来源：http://ns.huanxung.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://kh.nszjky.cn

[Q62] 分组占比
来源：http://bd.jctech888.com.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://un.nicolike.cn

[Q63] 开启事务
来源：http://kf.huixiangedu.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://nc.colortex.cn

[Q64] 提交事务
来源：http://gj.huixiangedu.cn

COMMIT;
来源：http://bh.bookmarksfly.cn

[Q65] 回滚事务
来源：http://mp.521024.cn

ROLLBACK;
来源：http://de.9csxet.cn

[Q66] 行锁查询
来源：http://lo.nicolike.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://jo.szxytkj.cn

[Q67] 设置隔离级别
来源：http://ti.asd995.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://zh.panjiajie.cn

[Q68] 保存点
来源：http://zp.nszjky.cn

SAVEPOINT sp1;
来源：http://li.jianghongdianzi.cn

ROLLBACK TO sp1;
来源：http://pi.nszjky.cn

[Q69] 查看执行计划
来源：http://sb.9csxet.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://xs.haigaiapp.cn

[Q70] 更新统计信息
来源：http://dj.newstarts.cn

ANALYZE TABLE users;
来源：http://et.panjiajie.cn

[Q71] 查看建表语句
来源：http://hv.nicolike.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://sm.bookmarksfly.cn

[Q72] 查看索引
来源：http://uh.haigaiapp.cn

SHOW INDEX FROM users;
来源：http://nn.nicolike.cn

[Q73] 查看表状态
来源：http://pa.shxzukj.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://io.colortex.cn

[Q74] 强制使用索引
来源：http://zc.gzmigu.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ah.chemitech.net.cn

[Q75] 日期格式化
来源：http://uh.hahajie.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://sv.panjiajie.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://cv.jianghongdianzi.cn

[Q76] 按天统计
来源：http://go.521024.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://bv.colortex.cn

[Q77] 时间加减
来源：http://uu.shxzskj.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://vb.nicolike.cn

[Q78] 当前时间
来源：http://pf.shxzskj.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://iv.szsharing.cn

[Q79] 字符串拼接
来源：http://gs.shxzskj.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ii.huixiangedu.cn

[Q80] 字符串截取
来源：http://hj.nicolike.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://kl.gzmigu.cn

[Q81] 字符串替换
来源：http://tn.huixiangedu.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://nw.huanxung.cn

[Q82] 字符长度与字节长度
来源：http://kv.chemitech.net.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://oc.szsharing.cn

[Q83] 大小写转换
来源：http://rv.nszjky.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ay.haigaiapp.cn

[Q84] 去除首尾空格
来源：http://ym.asd995.cn

SELECT TRIM(name) FROM users;
来源：http://za.muxihuayi.cn

[Q85] 数值取整
来源：http://hg.shxzukj.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://pg.yuexingan06.cn

[Q86] 读取 JSON 字段
来源：http://gx.wgjwhj.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://te.szsharing.cn

[Q87] JSON 字段做条件
来源：http://ib.wgjwhj.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hx.nszjky.cn

[Q88] 行转列（条件聚合）
来源：http://nq.hahajie.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ef.muxihuayi.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://fd.huanxung.cn

[Q89] 判断表是否存在
来源：http://uy.muxihuayi.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://yf.jctech888.com.cn

[Q90] 生成序号列
来源：http://kq.asd995.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mm.yuntaijiaju.cn

================================================================================
来源：http://hp.wgjwhj.cn

R. Bash 专题
来源：http://lh.chemitech.net.cn

================================================================================
来源：http://co.szsharing.cn

[R01] shebang 与严格模式
来源：http://if.shxzskj.cn

#!/usr/bin/env bash
来源：http://na.wgjwhj.cn

set -euo pipefail
来源：http://cs.gzmigu.cn

[R02] 变量赋值与使用
来源：http://sp.shxzukj.cn

name="Tom"; echo "$name"
来源：http://yh.shxzukj.cn

[R03] 只读变量
来源：http://za.bjjhwx.cn

readonly PI=3.14
来源：http://qw.szsharing.cn

[R04] 位置参数
来源：http://dv.yuexingan06.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://yi.yuntaijiaju.cn

[R05] 参数默认值
来源：http://mt.bookmarksfly.cn

name="${1:-default}"
来源：http://tp.yuexingan06.cn

[R06] 判断命令是否存在
来源：http://ok.shxzskj.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://in.9csxet.cn

[R07] if 判断文件
来源：http://tj.yuexingan06.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://bm.panjiajie.cn

[R08] 数值比较
来源：http://tl.jctech888.com.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://tj.shtwfgs.cn

[R09] 字符串比较
来源：http://yu.shxzukj.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://st.lnxyls.cn

[R10] 正则匹配
来源：http://ai.jianghongdianzi.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://fs.huanxung.cn

[R11] case 多分支
来源：http://ae.asd995.cn

case "$1" in
来源：http://tp.yuexingan06.cn

start) echo "启动" ;;
来源：http://mp.bookmarksfly.cn

stop)  echo "停止" ;;
来源：http://um.521024.cn

*)     echo "未知命令" ;;
来源：http://yp.chemitech.net.cn

esac
来源：http://tu.szxytkj.cn

[R12] for 遍历文件
来源：http://co.panjiajie.cn

for f in *.txt; do echo "$f"; done
来源：http://yg.wgjwhj.cn

[R13] for 计数循环
来源：http://gf.shxzukj.cn

for i in {1..10}; do echo "$i"; done
来源：http://km.yuexingan06.cn

[R14] C 风格 for
来源：http://ga.panjiajie.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://lh.wgjwhj.cn

[R15] while 逐行读文件
来源：http://dt.szxytkj.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://le.huanxung.cn

[R16] until 等待条件
来源：http://pt.shtwfgs.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ta.wgjwhj.cn

[R17] 数组定义与取值
来源：http://li.panjiajie.cn

arr=(a b c); echo "${arr[0]}"
来源：http://wd.bookmarksfly.cn

[R18] 遍历数组
来源：http://wh.nszjky.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mp.shxzukj.cn

[R19] 数组长度
来源：http://jc.lnxyls.cn

echo "${#arr[@]}"
来源：http://hz.chemitech.net.cn

[R20] 关联数组（字典）
来源：http://uu.yuexingan06.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://qe.newstarts.cn

[R21] 字符串长度
来源：http://qm.gzmigu.cn

echo "${#s}"
来源：http://je.9csxet.cn

[R22] 截取子串
来源：http://xc.yuntaijiaju.cn

echo "${s:0:5}"
来源：http://wq.szsharing.cn

[R23] 字符串替换
来源：http://my.bookmarksfly.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://uh.lnxyls.cn

[R24] 大小写转换
来源：http://rd.bjjhwx.cn

echo "${s^^}"; echo "${s,,}"
来源：http://jf.huixinmuqiang.cn

[R25] 去后缀 / 去前缀
来源：http://gp.colortex.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://lb.hnjuh.cn

[R26] 命令替换
来源：http://ag.wgjwhj.cn

now=$(date +%F); echo "$now"
来源：http://ab.shtwfgs.cn

[R27] 算术展开
来源：http://jd.bookmarksfly.cn

echo $((1 + 2 * 3))
来源：http://an.jctech888.com.cn

[R28] 浮点运算
来源：http://el.bookmarksfly.cn

echo "scale=2; 10/3" | bc
来源：http://jq.nicolike.cn

[R29] 定义函数
来源：http://cp.wgjwhj.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://yi.huixinmuqiang.cn

[R30] 函数返回状态码
来源：http://oo.chemitech.net.cn

f() { return 0; }; f || echo "失败了"
来源：http://wl.nicolike.cn

[R31] 局部变量
来源：http://js.huanxung.cn

f() { local x=1; echo "$x"; }
来源：http://to.yuntaijiaju.cn

[R32] 参数个数校验
来源：http://ty.szsharing.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wb.haigaiapp.cn

[R33] 捕获错误并提示行号
来源：http://fa.shxzukj.cn


<!-- 参考信息 -->