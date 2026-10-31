代发 wailian999

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://oo.wgjwhj.cn

TS:   if (x == null) {}
来源：http://an.shxzskj.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://kw.newstarts.cn

Go:   if x == nil {}
来源：http://pz.nszjky.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hl.nicolike.cn

C#:   if (x is null) {}
来源：http://zv.shtwfgs.cn

[P07] 防抖与节流
来源：http://pw.panjiajie.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://iu.nicolike.cn

PHP:  // 手写时间戳比较
来源：http://av.521024.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://yy.huixinmuqiang.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://cd.newstarts.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://vs.hahajie.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://pa.yuntaijiaju.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://wk.shtwfgs.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wi.nszjky.cn

[P08] 处理浮点精度问题
来源：http://tr.nicolike.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://rt.huixinmuqiang.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://vk.szsharing.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://yk.bookmarksfly.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://qw.asd995.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ls.huixiangedu.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://jr.yuntaijiaju.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ry.newstarts.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://cf.shxzskj.cn

================================================================================
来源：http://uv.shxzskj.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://xs.lnxyls.cn

================================================================================
来源：http://tl.huixiangedu.cn

[Q01] 创建表
来源：http://yk.shxzukj.cn

CREATE TABLE users (
来源：http://mj.hahajie.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://zu.gzmigu.cn

name VARCHAR(50) NOT NULL,
来源：http://um.newstarts.cn

email VARCHAR(100) UNIQUE,
来源：http://qp.panjiajie.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://br.huanxung.cn

);
来源：http://pf.huixiangedu.cn

[Q02] 创建带外键的表
来源：http://vj.huanxung.cn

CREATE TABLE orders (
来源：http://qb.521024.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ug.jctech888.com.cn

user_id INT NOT NULL,
来源：http://ws.huixiangedu.cn

amount DECIMAL(10, 2),
来源：http://du.gzmigu.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://rv.nszjky.cn

);
来源：http://fz.huanxung.cn

[Q03] 增加列
来源：http://xp.wgjwhj.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://he.szxytkj.cn

[Q04] 修改列类型
来源：http://gj.panjiajie.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://kr.colortex.cn

[Q05] 重命名列
来源：http://kf.yuntaijiaju.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ja.lnxyls.cn

[Q06] 删除列
来源：http://bc.gzmigu.cn

ALTER TABLE users DROP COLUMN age;
来源：http://yp.shtwfgs.cn

[Q07] 删除表
来源：http://ok.shxzskj.cn

DROP TABLE IF EXISTS orders;
来源：http://hv.hahajie.cn

[Q08] 创建普通索引
来源：http://go.haigaiapp.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://fm.colortex.cn

[Q09] 创建唯一索引
来源：http://pl.lnxyls.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wi.bjjhwx.cn

[Q10] 插入单行
来源：http://ok.haigaiapp.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://uz.nicolike.cn

[Q11] 一次插入多行
来源：http://kx.huixinmuqiang.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ld.bjjhwx.cn

[Q12] 插入后取自增 ID
来源：http://me.521024.cn

INSERT INTO users (name) VALUES ('C');
来源：http://ca.wgjwhj.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://bd.bjjhwx.cn

[Q13] 忽略重复插入
来源：http://tr.muxihuayi.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://tx.colortex.cn

[Q14] 存在则更新（upsert）
来源：http://tm.haigaiapp.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://nu.muxihuayi.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://nv.bjjhwx.cn

[Q15] 查询全部
来源：http://dl.lnxyls.cn

SELECT * FROM users;
来源：http://go.shxzukj.cn

[Q16] 查询指定列
来源：http://nb.szsharing.cn

SELECT id, name FROM users;
来源：http://vf.nszjky.cn

[Q17] 条件查询
来源：http://wm.bookmarksfly.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wb.chemitech.net.cn

[Q18] 模糊匹配
来源：http://hx.jianghongdianzi.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://rz.nicolike.cn

[Q19] 范围查询
来源：http://ej.huanxung.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://cf.yuexingan06.cn

[Q20] IN 列表
来源：http://tt.asd995.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ya.nszjky.cn

[Q21] 空值判断
来源：http://fr.jianghongdianzi.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://jk.nszjky.cn

[Q22] 排序
来源：http://oz.haigaiapp.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://zz.bookmarksfly.cn

[Q23] 分页
来源：http://gg.hahajie.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://qs.szsharing.cn

[Q24] 去重
来源：http://hm.jctech888.com.cn

SELECT DISTINCT city FROM users;
来源：http://xe.szsharing.cn

[Q25] 只取前 N 条
来源：http://bz.chemitech.net.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://fu.haigaiapp.cn

[Q26] 计数
来源：http://gk.asd995.cn

SELECT COUNT(*) FROM users;
来源：http://qz.panjiajie.cn

[Q27] 条件计数
来源：http://me.huixiangedu.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://rw.jianghongdianzi.cn

[Q28] 求和与平均
来源：http://hr.huixinmuqiang.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://ii.huixinmuqiang.cn

[Q29] 最大最小值
来源：http://ns.yuexingan06.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://zs.jctech888.com.cn

[Q30] 分组统计
来源：http://ex.szsharing.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://er.colortex.cn

[Q31] 分组后过滤
来源：http://di.asd995.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://dm.szxytkj.cn

[Q32] 分组拼接字符串
来源：http://ek.muxihuayi.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hb.huanxung.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://rt.szxytkj.cn

[Q33] 多列分组
来源：http://wu.yuntaijiaju.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hi.gzmigu.cn

[Q34] 每组取第一条
来源：http://hc.asd995.cn

SELECT * FROM (
来源：http://yt.szxytkj.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://pg.szxytkj.cn

) t WHERE rn = 1;
来源：http://jx.bookmarksfly.cn

[Q35] 内连接
来源：http://fk.nicolike.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://yq.521024.cn

[Q36] 左连接
来源：http://bw.jctech888.com.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://as.9csxet.cn

[Q37] 右连接
来源：http://yr.muxihuayi.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://vi.jianghongdianzi.cn

[Q38] 全外连接（PostgreSQL）
来源：http://dn.lnxyls.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://bk.newstarts.cn

[Q39] 自连接（查上下级）
来源：http://qn.huixinmuqiang.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://ay.gzmigu.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://lh.muxihuayi.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://ah.szxytkj.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://pt.shxzukj.cn

[Q41] 多表连接
来源：http://hn.hahajie.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://gk.newstarts.cn

JOIN users u ON u.id = o.user_id
来源：http://ys.huixinmuqiang.cn

JOIN products p ON p.id = o.product_id;
来源：http://ur.szxytkj.cn

[Q42] 连接条件附加过滤
来源：http://ez.bookmarksfly.cn

SELECT u.name, o.amount FROM users u
来源：http://jt.hahajie.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://fc.bjjhwx.cn

[Q43] 标量子查询
来源：http://ht.nicolike.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://bf.huixiangedu.cn

[Q44] IN 子查询
来源：http://uh.haigaiapp.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wo.muxihuayi.cn

[Q45] EXISTS 判断存在
来源：http://on.jctech888.com.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://qw.hnjuh.cn

[Q46] NOT EXISTS 判断不存在
来源：http://mg.asd995.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://dh.hnjuh.cn

[Q47] 与平均值比较
来源：http://mm.chemitech.net.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://nx.huixinmuqiang.cn

[Q48] CTE 公用表表达式
来源：http://ut.huanxung.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://po.nicolike.cn

SELECT * FROM t WHERE c > 5;
来源：http://ld.521024.cn

[Q49] 更新单行
来源：http://xv.haigaiapp.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mi.hahajie.cn

[Q50] 批量更新
来源：http://zd.nicolike.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://up.yuexingan06.cn

[Q51] 用子查询更新
来源：http://rt.colortex.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://lv.hnjuh.cn

[Q52] 删除指定行
来源：http://zv.yuexingan06.cn

DELETE FROM users WHERE id = 10;
来源：http://yd.lnxyls.cn

[Q53] 按条件删除
来源：http://iz.nszjky.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://cz.bookmarksfly.cn

[Q54] 清空表
来源：http://rz.szxytkj.cn

TRUNCATE TABLE logs;
来源：http://ys.nicolike.cn

[Q55] 排名（并列占位）
来源：http://fw.asd995.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://fk.521024.cn

[Q56] 密集排名（并列不占位）
来源：http://jd.bjjhwx.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://xy.lnxyls.cn

[Q57] 行号
来源：http://ud.newstarts.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ci.nicolike.cn

[Q58] 累计求和
来源：http://fm.hnjuh.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://iq.yuexingan06.cn

[Q59] 分组内累计
来源：http://lb.shxzukj.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://rd.9csxet.cn

[Q60] 取上一行 / 下一行
来源：http://yp.haigaiapp.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://jv.muxihuayi.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://fi.hnjuh.cn

[Q61] 移动平均
来源：http://fo.haigaiapp.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://qr.chemitech.net.cn

[Q62] 分组占比
来源：http://ui.huanxung.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ok.panjiajie.cn

[Q63] 开启事务
来源：http://wd.shxzskj.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://xs.yuntaijiaju.cn

[Q64] 提交事务
来源：http://hq.521024.cn

COMMIT;
来源：http://iq.szsharing.cn

[Q65] 回滚事务
来源：http://kz.colortex.cn

ROLLBACK;
来源：http://qf.panjiajie.cn

[Q66] 行锁查询
来源：http://dl.hnjuh.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wl.gzmigu.cn

[Q67] 设置隔离级别
来源：http://pz.haigaiapp.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://yj.huixiangedu.cn

[Q68] 保存点
来源：http://qe.yuexingan06.cn

SAVEPOINT sp1;
来源：http://jg.szsharing.cn

ROLLBACK TO sp1;
来源：http://gb.colortex.cn

[Q69] 查看执行计划
来源：http://og.bjjhwx.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://si.hnjuh.cn

[Q70] 更新统计信息
来源：http://be.szxytkj.cn

ANALYZE TABLE users;
来源：http://xk.jctech888.com.cn

[Q71] 查看建表语句
来源：http://eq.muxihuayi.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://je.asd995.cn

[Q72] 查看索引
来源：http://nr.hnjuh.cn

SHOW INDEX FROM users;
来源：http://uy.lnxyls.cn

[Q73] 查看表状态
来源：http://ut.huixinmuqiang.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://am.gzmigu.cn

[Q74] 强制使用索引
来源：http://tz.szxytkj.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://zu.yuexingan06.cn

[Q75] 日期格式化
来源：http://bt.huixiangedu.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ys.9csxet.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://nj.colortex.cn

[Q76] 按天统计
来源：http://tn.521024.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://zo.asd995.cn

[Q77] 时间加减
来源：http://oh.lnxyls.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://oz.hahajie.cn

[Q78] 当前时间
来源：http://fu.nszjky.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://vl.nszjky.cn

[Q79] 字符串拼接
来源：http://rv.asd995.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ov.colortex.cn

[Q80] 字符串截取
来源：http://uu.asd995.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://cw.haigaiapp.cn

[Q81] 字符串替换
来源：http://rg.lnxyls.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://oh.yuexingan06.cn

[Q82] 字符长度与字节长度
来源：http://uq.asd995.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://sc.szxytkj.cn

[Q83] 大小写转换
来源：http://gj.bjjhwx.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://nq.9csxet.cn

[Q84] 去除首尾空格
来源：http://ij.jianghongdianzi.cn

SELECT TRIM(name) FROM users;
来源：http://zb.nicolike.cn

[Q85] 数值取整
来源：http://dh.yuexingan06.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://kf.bookmarksfly.cn

[Q86] 读取 JSON 字段
来源：http://sv.newstarts.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mx.lnxyls.cn

[Q87] JSON 字段做条件
来源：http://ac.yuntaijiaju.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://cm.hahajie.cn

[Q88] 行转列（条件聚合）
来源：http://lb.asd995.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://li.gzmigu.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://gx.jianghongdianzi.cn

[Q89] 判断表是否存在
来源：http://kz.nicolike.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://di.jctech888.com.cn

[Q90] 生成序号列
来源：http://ai.bookmarksfly.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wu.shxzskj.cn

================================================================================
来源：http://ow.jctech888.com.cn

R. Bash 专题
来源：http://li.colortex.cn

================================================================================
来源：http://lh.shxzukj.cn

[R01] shebang 与严格模式
来源：http://cb.nszjky.cn

#!/usr/bin/env bash
来源：http://vb.hnjuh.cn

set -euo pipefail
来源：http://am.jianghongdianzi.cn

[R02] 变量赋值与使用
来源：http://ym.chemitech.net.cn

name="Tom"; echo "$name"
来源：http://gi.jctech888.com.cn

[R03] 只读变量
来源：http://qg.huixiangedu.cn

readonly PI=3.14
来源：http://uv.nicolike.cn

[R04] 位置参数
来源：http://yd.yuexingan06.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mw.bookmarksfly.cn

[R05] 参数默认值
来源：http://yf.gzmigu.cn

name="${1:-default}"
来源：http://ri.9csxet.cn

[R06] 判断命令是否存在
来源：http://pf.hahajie.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://uq.szxytkj.cn

[R07] if 判断文件
来源：http://oi.gzmigu.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wd.muxihuayi.cn

[R08] 数值比较
来源：http://ey.nicolike.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://we.szsharing.cn

[R09] 字符串比较
来源：http://wo.gzmigu.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wv.muxihuayi.cn

[R10] 正则匹配
来源：http://bl.asd995.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://zn.gzmigu.cn

[R11] case 多分支
来源：http://lu.jianghongdianzi.cn

case "$1" in
来源：http://nw.gzmigu.cn

start) echo "启动" ;;
来源：http://xx.bookmarksfly.cn

stop)  echo "停止" ;;
来源：http://pw.bookmarksfly.cn

*)     echo "未知命令" ;;
来源：http://jn.newstarts.cn

esac
来源：http://rh.haigaiapp.cn

[R12] for 遍历文件
来源：http://iq.asd995.cn

for f in *.txt; do echo "$f"; done
来源：http://dx.lnxyls.cn

[R13] for 计数循环
来源：http://at.yuexingan06.cn

for i in {1..10}; do echo "$i"; done
来源：http://zx.yuntaijiaju.cn

[R14] C 风格 for
来源：http://ln.huanxung.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://qc.bjjhwx.cn

[R15] while 逐行读文件
来源：http://uk.9csxet.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://bg.yuexingan06.cn

[R16] until 等待条件
来源：http://ep.huanxung.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://oc.bookmarksfly.cn

[R17] 数组定义与取值
来源：http://vk.yuntaijiaju.cn

arr=(a b c); echo "${arr[0]}"
来源：http://pl.bjjhwx.cn

[R18] 遍历数组
来源：http://qa.yuntaijiaju.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mz.huixiangedu.cn

[R19] 数组长度
来源：http://vw.muxihuayi.cn

echo "${#arr[@]}"
来源：http://ym.gzmigu.cn

[R20] 关联数组（字典）
来源：http://no.521024.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://fe.colortex.cn

[R21] 字符串长度
来源：http://lp.huixinmuqiang.cn

echo "${#s}"
来源：http://gl.shxzskj.cn

[R22] 截取子串
来源：http://jm.hahajie.cn

echo "${s:0:5}"
来源：http://ei.chemitech.net.cn

[R23] 字符串替换
来源：http://dm.9csxet.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://lv.szxytkj.cn

[R24] 大小写转换
来源：http://mk.521024.cn

echo "${s^^}"; echo "${s,,}"
来源：http://gr.asd995.cn

[R25] 去后缀 / 去前缀
来源：http://vh.haigaiapp.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://zi.yuexingan06.cn

[R26] 命令替换
来源：http://rg.shxzukj.cn

now=$(date +%F); echo "$now"
来源：http://ug.shtwfgs.cn

[R27] 算术展开
来源：http://id.muxihuayi.cn

echo $((1 + 2 * 3))
来源：http://dz.muxihuayi.cn

[R28] 浮点运算
来源：http://hv.newstarts.cn

echo "scale=2; 10/3" | bc
来源：http://sj.shtwfgs.cn

[R29] 定义函数
来源：http://se.lnxyls.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://vb.521024.cn

[R30] 函数返回状态码
来源：http://qu.colortex.cn

f() { return 0; }; f || echo "失败了"
来源：http://bz.wgjwhj.cn

[R31] 局部变量
来源：http://vj.asd995.cn


<!-- 参考信息 -->