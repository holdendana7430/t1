代发 wailian999

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://qp.jianghongdianzi.cn

C#:   if (x is null) {}
来源：http://sf.521024.cn

[P07] 防抖与节流
来源：http://il.asd995.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://st.szsharing.cn

PHP:  // 手写时间戳比较
来源：http://bm.yuexingan06.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://iw.yuexingan06.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://co.szxytkj.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://zc.nicolike.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ty.hahajie.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://br.muxihuayi.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://yf.muxihuayi.cn

[P08] 处理浮点精度问题
来源：http://nl.colortex.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://lq.huixinmuqiang.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://yn.hahajie.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://uj.521024.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://vl.shxzskj.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://kr.shxzskj.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://eb.nicolike.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ie.szxytkj.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://cx.chemitech.net.cn

================================================================================
来源：http://du.521024.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://vy.bookmarksfly.cn

================================================================================
来源：http://en.nicolike.cn

[Q01] 创建表
来源：http://gl.nicolike.cn

CREATE TABLE users (
来源：http://gw.huixinmuqiang.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://kb.muxihuayi.cn

name VARCHAR(50) NOT NULL,
来源：http://uy.shxzukj.cn

email VARCHAR(100) UNIQUE,
来源：http://on.bjjhwx.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://qe.521024.cn

);
来源：http://dx.nszjky.cn

[Q02] 创建带外键的表
来源：http://ud.521024.cn

CREATE TABLE orders (
来源：http://mn.yuexingan06.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://jz.szxytkj.cn

user_id INT NOT NULL,
来源：http://vr.szxytkj.cn

amount DECIMAL(10, 2),
来源：http://tj.nicolike.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://bx.yuntaijiaju.cn

);
来源：http://uv.huanxung.cn

[Q03] 增加列
来源：http://dd.szsharing.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://eb.haigaiapp.cn

[Q04] 修改列类型
来源：http://jz.muxihuayi.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ak.wgjwhj.cn

[Q05] 重命名列
来源：http://vi.newstarts.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wy.nicolike.cn

[Q06] 删除列
来源：http://vv.asd995.cn

ALTER TABLE users DROP COLUMN age;
来源：http://mr.chemitech.net.cn

[Q07] 删除表
来源：http://zu.huixiangedu.cn

DROP TABLE IF EXISTS orders;
来源：http://nh.yuexingan06.cn

[Q08] 创建普通索引
来源：http://kp.hahajie.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://xf.nicolike.cn

[Q09] 创建唯一索引
来源：http://zz.bjjhwx.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://lh.wgjwhj.cn

[Q10] 插入单行
来源：http://vy.shxzukj.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ga.shxzskj.cn

[Q11] 一次插入多行
来源：http://rq.hnjuh.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://sp.shxzskj.cn

[Q12] 插入后取自增 ID
来源：http://mv.yuexingan06.cn

INSERT INTO users (name) VALUES ('C');
来源：http://kb.gzmigu.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://me.huanxung.cn

[Q13] 忽略重复插入
来源：http://zf.wgjwhj.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://cz.muxihuayi.cn

[Q14] 存在则更新（upsert）
来源：http://fd.colortex.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://pr.muxihuayi.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://fv.lnxyls.cn

[Q15] 查询全部
来源：http://av.shxzukj.cn

SELECT * FROM users;
来源：http://fj.shxzskj.cn

[Q16] 查询指定列
来源：http://ei.nszjky.cn

SELECT id, name FROM users;
来源：http://wr.colortex.cn

[Q17] 条件查询
来源：http://ht.521024.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ud.jianghongdianzi.cn

[Q18] 模糊匹配
来源：http://kw.shxzskj.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://rr.wgjwhj.cn

[Q19] 范围查询
来源：http://zm.shtwfgs.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://uh.panjiajie.cn

[Q20] IN 列表
来源：http://it.muxihuayi.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://gq.shxzskj.cn

[Q21] 空值判断
来源：http://zw.bjjhwx.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://av.shxzukj.cn

[Q22] 排序
来源：http://en.huixiangedu.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ha.hnjuh.cn

[Q23] 分页
来源：http://jn.hnjuh.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hc.gzmigu.cn

[Q24] 去重
来源：http://wf.hnjuh.cn

SELECT DISTINCT city FROM users;
来源：http://so.bjjhwx.cn

[Q25] 只取前 N 条
来源：http://cf.asd995.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://vi.jctech888.com.cn

[Q26] 计数
来源：http://zb.hahajie.cn

SELECT COUNT(*) FROM users;
来源：http://td.huanxung.cn

[Q27] 条件计数
来源：http://eu.panjiajie.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://qs.huixinmuqiang.cn

[Q28] 求和与平均
来源：http://sy.jctech888.com.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://xz.bookmarksfly.cn

[Q29] 最大最小值
来源：http://mo.yuexingan06.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://qa.panjiajie.cn

[Q30] 分组统计
来源：http://ma.panjiajie.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://tm.huixinmuqiang.cn

[Q31] 分组后过滤
来源：http://fd.colortex.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://jl.9csxet.cn

[Q32] 分组拼接字符串
来源：http://gu.szsharing.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://xu.lnxyls.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://cm.huanxung.cn

[Q33] 多列分组
来源：http://sw.gzmigu.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wn.szxytkj.cn

[Q34] 每组取第一条
来源：http://hw.hnjuh.cn

SELECT * FROM (
来源：http://ke.chemitech.net.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://nc.szxytkj.cn

) t WHERE rn = 1;
来源：http://sm.haigaiapp.cn

[Q35] 内连接
来源：http://dr.jctech888.com.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://rm.lnxyls.cn

[Q36] 左连接
来源：http://cc.shtwfgs.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://bj.shtwfgs.cn

[Q37] 右连接
来源：http://tv.hnjuh.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://uz.huixiangedu.cn

[Q38] 全外连接（PostgreSQL）
来源：http://lh.yuntaijiaju.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://bu.asd995.cn

[Q39] 自连接（查上下级）
来源：http://pk.nicolike.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://et.521024.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wg.szxytkj.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://mh.521024.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://tf.gzmigu.cn

[Q41] 多表连接
来源：http://tr.asd995.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://ay.szsharing.cn

JOIN users u ON u.id = o.user_id
来源：http://ps.muxihuayi.cn

JOIN products p ON p.id = o.product_id;
来源：http://bn.521024.cn

[Q42] 连接条件附加过滤
来源：http://pk.panjiajie.cn

SELECT u.name, o.amount FROM users u
来源：http://ia.nicolike.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ac.haigaiapp.cn

[Q43] 标量子查询
来源：http://iw.huixinmuqiang.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://tp.muxihuayi.cn

[Q44] IN 子查询
来源：http://fd.muxihuayi.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://qi.huanxung.cn

[Q45] EXISTS 判断存在
来源：http://uj.chemitech.net.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ss.huanxung.cn

[Q46] NOT EXISTS 判断不存在
来源：http://bw.shxzukj.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://un.huixiangedu.cn

[Q47] 与平均值比较
来源：http://ox.shxzskj.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://oh.szxytkj.cn

[Q48] CTE 公用表表达式
来源：http://mf.shtwfgs.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://of.521024.cn

SELECT * FROM t WHERE c > 5;
来源：http://st.nicolike.cn

[Q49] 更新单行
来源：http://zf.huixiangedu.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://oq.gzmigu.cn

[Q50] 批量更新
来源：http://ua.newstarts.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mv.hnjuh.cn

[Q51] 用子查询更新
来源：http://sh.szsharing.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://xw.bjjhwx.cn

[Q52] 删除指定行
来源：http://xx.hahajie.cn

DELETE FROM users WHERE id = 10;
来源：http://ap.shxzukj.cn

[Q53] 按条件删除
来源：http://tu.jctech888.com.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://il.bookmarksfly.cn

[Q54] 清空表
来源：http://rr.shxzukj.cn

TRUNCATE TABLE logs;
来源：http://qp.colortex.cn

[Q55] 排名（并列占位）
来源：http://lr.shtwfgs.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://lt.chemitech.net.cn

[Q56] 密集排名（并列不占位）
来源：http://qd.shxzukj.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mo.lnxyls.cn

[Q57] 行号
来源：http://pa.shtwfgs.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://na.gzmigu.cn

[Q58] 累计求和
来源：http://rm.yuexingan06.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://dq.shtwfgs.cn

[Q59] 分组内累计
来源：http://vd.colortex.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hy.panjiajie.cn

[Q60] 取上一行 / 下一行
来源：http://gc.colortex.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://oj.lnxyls.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://sm.colortex.cn

[Q61] 移动平均
来源：http://ip.huanxung.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mm.nszjky.cn

[Q62] 分组占比
来源：http://hg.haigaiapp.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ad.bookmarksfly.cn

[Q63] 开启事务
来源：http://cf.nszjky.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://ku.chemitech.net.cn

[Q64] 提交事务
来源：http://ji.huixiangedu.cn

COMMIT;
来源：http://as.yuntaijiaju.cn

[Q65] 回滚事务
来源：http://gh.bookmarksfly.cn

ROLLBACK;
来源：http://gq.521024.cn

[Q66] 行锁查询
来源：http://cs.huixiangedu.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ro.haigaiapp.cn

[Q67] 设置隔离级别
来源：http://vn.huixinmuqiang.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://fu.lnxyls.cn

[Q68] 保存点
来源：http://yy.hnjuh.cn

SAVEPOINT sp1;
来源：http://ko.nicolike.cn

ROLLBACK TO sp1;
来源：http://lr.muxihuayi.cn

[Q69] 查看执行计划
来源：http://le.newstarts.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://yg.hnjuh.cn

[Q70] 更新统计信息
来源：http://cg.huixiangedu.cn

ANALYZE TABLE users;
来源：http://ua.hnjuh.cn

[Q71] 查看建表语句
来源：http://um.521024.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://vv.jctech888.com.cn

[Q72] 查看索引
来源：http://ok.newstarts.cn

SHOW INDEX FROM users;
来源：http://gs.szsharing.cn

[Q73] 查看表状态
来源：http://nt.shxzskj.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://fr.nszjky.cn

[Q74] 强制使用索引
来源：http://wf.panjiajie.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wy.521024.cn

[Q75] 日期格式化
来源：http://ye.shxzukj.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://rc.nszjky.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://oc.yuexingan06.cn

[Q76] 按天统计
来源：http://we.shxzskj.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://zv.szsharing.cn

[Q77] 时间加减
来源：http://uq.huanxung.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://zz.asd995.cn

[Q78] 当前时间
来源：http://oq.bookmarksfly.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://xs.huixinmuqiang.cn

[Q79] 字符串拼接
来源：http://pz.lnxyls.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://sp.yuntaijiaju.cn

[Q80] 字符串截取
来源：http://vp.szxytkj.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ra.lnxyls.cn

[Q81] 字符串替换
来源：http://iq.haigaiapp.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://jw.nicolike.cn

[Q82] 字符长度与字节长度
来源：http://hq.newstarts.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://jl.nszjky.cn

[Q83] 大小写转换
来源：http://ui.asd995.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://vq.shxzskj.cn

[Q84] 去除首尾空格
来源：http://bp.haigaiapp.cn

SELECT TRIM(name) FROM users;
来源：http://un.muxihuayi.cn

[Q85] 数值取整
来源：http://ig.szsharing.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://dq.bookmarksfly.cn

[Q86] 读取 JSON 字段
来源：http://pp.shxzukj.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://qu.nszjky.cn

[Q87] JSON 字段做条件
来源：http://pn.yuexingan06.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://lp.szxytkj.cn

[Q88] 行转列（条件聚合）
来源：http://xm.bookmarksfly.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ue.haigaiapp.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://qk.shxzskj.cn

[Q89] 判断表是否存在
来源：http://rm.lnxyls.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ta.shtwfgs.cn

[Q90] 生成序号列
来源：http://rx.jianghongdianzi.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ie.hnjuh.cn

================================================================================
来源：http://go.shxzskj.cn

R. Bash 专题
来源：http://or.jctech888.com.cn

================================================================================
来源：http://oz.huixinmuqiang.cn

[R01] shebang 与严格模式
来源：http://rk.hahajie.cn

#!/usr/bin/env bash
来源：http://pz.hahajie.cn

set -euo pipefail
来源：http://of.hahajie.cn

[R02] 变量赋值与使用
来源：http://ts.shtwfgs.cn

name="Tom"; echo "$name"
来源：http://uj.szxytkj.cn

[R03] 只读变量
来源：http://rw.jianghongdianzi.cn

readonly PI=3.14
来源：http://nq.yuntaijiaju.cn

[R04] 位置参数
来源：http://km.muxihuayi.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://dr.lnxyls.cn

[R05] 参数默认值
来源：http://fp.yuntaijiaju.cn

name="${1:-default}"
来源：http://zb.panjiajie.cn

[R06] 判断命令是否存在
来源：http://af.9csxet.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://cc.gzmigu.cn

[R07] if 判断文件
来源：http://ou.haigaiapp.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ou.yuntaijiaju.cn

[R08] 数值比较
来源：http://lw.shtwfgs.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://wi.yuexingan06.cn

[R09] 字符串比较
来源：http://cg.9csxet.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://so.shtwfgs.cn

[R10] 正则匹配
来源：http://tu.shtwfgs.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://dd.huixiangedu.cn

[R11] case 多分支
来源：http://ij.shxzskj.cn

case "$1" in
来源：http://zi.nszjky.cn

start) echo "启动" ;;
来源：http://of.shxzukj.cn

stop)  echo "停止" ;;
来源：http://dt.nszjky.cn

*)     echo "未知命令" ;;
来源：http://ro.asd995.cn

esac
来源：http://vc.muxihuayi.cn

[R12] for 遍历文件
来源：http://xd.hahajie.cn

for f in *.txt; do echo "$f"; done
来源：http://ll.huixiangedu.cn

[R13] for 计数循环
来源：http://do.szxytkj.cn

for i in {1..10}; do echo "$i"; done
来源：http://an.szxytkj.cn

[R14] C 风格 for
来源：http://gm.yuntaijiaju.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://xd.gzmigu.cn

[R15] while 逐行读文件
来源：http://dw.shxzskj.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://in.panjiajie.cn

[R16] until 等待条件
来源：http://mh.nicolike.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://fw.newstarts.cn

[R17] 数组定义与取值
来源：http://dg.yuntaijiaju.cn

arr=(a b c); echo "${arr[0]}"
来源：http://rt.panjiajie.cn

[R18] 遍历数组
来源：http://lu.haigaiapp.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://cj.bjjhwx.cn

[R19] 数组长度
来源：http://yl.panjiajie.cn

echo "${#arr[@]}"
来源：http://lj.nicolike.cn

[R20] 关联数组（字典）
来源：http://ur.newstarts.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://jd.muxihuayi.cn

[R21] 字符串长度
来源：http://ak.szsharing.cn

echo "${#s}"
来源：http://zf.huanxung.cn

[R22] 截取子串
来源：http://pl.szsharing.cn

echo "${s:0:5}"
来源：http://js.shxzskj.cn

[R23] 字符串替换
来源：http://oa.jianghongdianzi.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hh.lnxyls.cn

[R24] 大小写转换
来源：http://dr.colortex.cn

echo "${s^^}"; echo "${s,,}"
来源：http://vv.newstarts.cn

[R25] 去后缀 / 去前缀
来源：http://rd.muxihuayi.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://ce.colortex.cn

[R26] 命令替换
来源：http://lj.colortex.cn

now=$(date +%F); echo "$now"
来源：http://eb.huixiangedu.cn

[R27] 算术展开
来源：http://il.9csxet.cn

echo $((1 + 2 * 3))
来源：http://qk.wgjwhj.cn

[R28] 浮点运算
来源：http://yh.asd995.cn

echo "scale=2; 10/3" | bc
来源：http://wb.huixiangedu.cn

[R29] 定义函数
来源：http://hf.szxytkj.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://dl.huixiangedu.cn

[R30] 函数返回状态码
来源：http://kf.521024.cn

f() { return 0; }; f || echo "失败了"
来源：http://lx.asd995.cn

[R31] 局部变量
来源：http://ft.asd995.cn

f() { local x=1; echo "$x"; }
来源：http://wq.panjiajie.cn

[R32] 参数个数校验
来源：http://yv.colortex.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://lh.hahajie.cn

[R33] 捕获错误并提示行号
来源：http://vz.huixiangedu.cn


<!-- 参考信息 -->