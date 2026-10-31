代发 wailian999

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://nq.yuntaijiaju.cn

C#:   if (x is null) {}
来源：http://sy.9csxet.cn

[P07] 防抖与节流
来源：http://of.nszjky.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://vn.newstarts.cn

PHP:  // 手写时间戳比较
来源：http://ye.szsharing.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://xm.bjjhwx.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ul.yuexingan06.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://al.hahajie.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://uo.hnjuh.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://dj.521024.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://th.gzmigu.cn

[P08] 处理浮点精度问题
来源：http://ld.huixinmuqiang.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://uq.wgjwhj.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ic.gzmigu.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://iz.wgjwhj.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ca.newstarts.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://tm.chemitech.net.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://zn.jianghongdianzi.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://dj.bookmarksfly.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wt.yuntaijiaju.cn

================================================================================
来源：http://ki.yuexingan06.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://fl.hnjuh.cn

================================================================================
来源：http://vb.panjiajie.cn

[Q01] 创建表
来源：http://lp.bookmarksfly.cn

CREATE TABLE users (
来源：http://al.hnjuh.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://nw.bjjhwx.cn

name VARCHAR(50) NOT NULL,
来源：http://or.9csxet.cn

email VARCHAR(100) UNIQUE,
来源：http://gd.huixinmuqiang.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ob.huixiangedu.cn

);
来源：http://xm.shtwfgs.cn

[Q02] 创建带外键的表
来源：http://ka.jctech888.com.cn

CREATE TABLE orders (
来源：http://ui.jianghongdianzi.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hm.szxytkj.cn

user_id INT NOT NULL,
来源：http://uk.muxihuayi.cn

amount DECIMAL(10, 2),
来源：http://fi.lnxyls.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://av.nszjky.cn

);
来源：http://ll.panjiajie.cn

[Q03] 增加列
来源：http://ig.jctech888.com.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ad.huixiangedu.cn

[Q04] 修改列类型
来源：http://ve.colortex.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://so.jianghongdianzi.cn

[Q05] 重命名列
来源：http://nc.nszjky.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mi.shxzukj.cn

[Q06] 删除列
来源：http://vd.haigaiapp.cn

ALTER TABLE users DROP COLUMN age;
来源：http://vi.huixinmuqiang.cn

[Q07] 删除表
来源：http://qa.nszjky.cn

DROP TABLE IF EXISTS orders;
来源：http://vi.nicolike.cn

[Q08] 创建普通索引
来源：http://ea.bookmarksfly.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://hx.jctech888.com.cn

[Q09] 创建唯一索引
来源：http://ug.haigaiapp.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://nw.lnxyls.cn

[Q10] 插入单行
来源：http://cb.gzmigu.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wf.bookmarksfly.cn

[Q11] 一次插入多行
来源：http://om.bjjhwx.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ua.huanxung.cn

[Q12] 插入后取自增 ID
来源：http://ot.nicolike.cn

INSERT INTO users (name) VALUES ('C');
来源：http://xt.shxzukj.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://vr.nszjky.cn

[Q13] 忽略重复插入
来源：http://oh.hahajie.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://uj.huixinmuqiang.cn

[Q14] 存在则更新（upsert）
来源：http://xd.jianghongdianzi.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://be.hahajie.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://er.shxzskj.cn

[Q15] 查询全部
来源：http://ln.lnxyls.cn

SELECT * FROM users;
来源：http://ka.shtwfgs.cn

[Q16] 查询指定列
来源：http://ed.bjjhwx.cn

SELECT id, name FROM users;
来源：http://jm.hnjuh.cn

[Q17] 条件查询
来源：http://si.colortex.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://gd.szsharing.cn

[Q18] 模糊匹配
来源：http://aj.haigaiapp.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://uy.newstarts.cn

[Q19] 范围查询
来源：http://kn.bookmarksfly.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://fw.9csxet.cn

[Q20] IN 列表
来源：http://zu.muxihuayi.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://nm.yuntaijiaju.cn

[Q21] 空值判断
来源：http://jq.asd995.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://na.hnjuh.cn

[Q22] 排序
来源：http://wg.jianghongdianzi.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://an.nszjky.cn

[Q23] 分页
来源：http://fl.hahajie.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://gy.yuexingan06.cn

[Q24] 去重
来源：http://wu.jctech888.com.cn

SELECT DISTINCT city FROM users;
来源：http://lr.colortex.cn

[Q25] 只取前 N 条
来源：http://uy.colortex.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mf.hnjuh.cn

[Q26] 计数
来源：http://qs.521024.cn

SELECT COUNT(*) FROM users;
来源：http://zn.wgjwhj.cn

[Q27] 条件计数
来源：http://kq.huixiangedu.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://am.panjiajie.cn

[Q28] 求和与平均
来源：http://nq.gzmigu.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://to.gzmigu.cn

[Q29] 最大最小值
来源：http://dn.wgjwhj.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://oy.jctech888.com.cn

[Q30] 分组统计
来源：http://on.521024.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mm.newstarts.cn

[Q31] 分组后过滤
来源：http://yc.nszjky.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://vz.muxihuayi.cn

[Q32] 分组拼接字符串
来源：http://ka.jianghongdianzi.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://zv.jctech888.com.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://eh.9csxet.cn

[Q33] 多列分组
来源：http://jn.9csxet.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ez.shtwfgs.cn

[Q34] 每组取第一条
来源：http://lb.lnxyls.cn

SELECT * FROM (
来源：http://aq.huixinmuqiang.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hl.nicolike.cn

) t WHERE rn = 1;
来源：http://id.hnjuh.cn

[Q35] 内连接
来源：http://db.shxzukj.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://bk.colortex.cn

[Q36] 左连接
来源：http://ws.bjjhwx.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://rz.yuntaijiaju.cn

[Q37] 右连接
来源：http://oe.shtwfgs.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://vo.9csxet.cn

[Q38] 全外连接（PostgreSQL）
来源：http://vo.huixiangedu.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://nl.szxytkj.cn

[Q39] 自连接（查上下级）
来源：http://ra.chemitech.net.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://eo.jctech888.com.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://nf.huixinmuqiang.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://bg.szsharing.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://lp.shxzukj.cn

[Q41] 多表连接
来源：http://ke.huixiangedu.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://gp.jianghongdianzi.cn

JOIN users u ON u.id = o.user_id
来源：http://mq.hnjuh.cn

JOIN products p ON p.id = o.product_id;
来源：http://bs.nszjky.cn

[Q42] 连接条件附加过滤
来源：http://ri.shtwfgs.cn

SELECT u.name, o.amount FROM users u
来源：http://ul.huixiangedu.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ww.shxzukj.cn

[Q43] 标量子查询
来源：http://lv.muxihuayi.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://cs.shtwfgs.cn

[Q44] IN 子查询
来源：http://eg.gzmigu.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://np.hahajie.cn

[Q45] EXISTS 判断存在
来源：http://sn.newstarts.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://tu.szsharing.cn

[Q46] NOT EXISTS 判断不存在
来源：http://zl.jianghongdianzi.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://vg.hnjuh.cn

[Q47] 与平均值比较
来源：http://md.asd995.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://il.chemitech.net.cn

[Q48] CTE 公用表表达式
来源：http://lu.huanxung.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://sc.wgjwhj.cn

SELECT * FROM t WHERE c > 5;
来源：http://is.huixinmuqiang.cn

[Q49] 更新单行
来源：http://rj.bookmarksfly.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://jm.gzmigu.cn

[Q50] 批量更新
来源：http://jg.521024.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://el.muxihuayi.cn

[Q51] 用子查询更新
来源：http://yu.shxzukj.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wy.shxzskj.cn

[Q52] 删除指定行
来源：http://lr.hnjuh.cn

DELETE FROM users WHERE id = 10;
来源：http://zq.wgjwhj.cn

[Q53] 按条件删除
来源：http://cd.newstarts.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mz.shxzukj.cn

[Q54] 清空表
来源：http://hl.asd995.cn

TRUNCATE TABLE logs;
来源：http://ko.jianghongdianzi.cn

[Q55] 排名（并列占位）
来源：http://bm.chemitech.net.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://rn.yuexingan06.cn

[Q56] 密集排名（并列不占位）
来源：http://iw.yuntaijiaju.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://vb.bookmarksfly.cn

[Q57] 行号
来源：http://tl.lnxyls.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://bc.huixiangedu.cn

[Q58] 累计求和
来源：http://em.shxzukj.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://rq.szxytkj.cn

[Q59] 分组内累计
来源：http://be.yuexingan06.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ve.jctech888.com.cn

[Q60] 取上一行 / 下一行
来源：http://ww.jctech888.com.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://li.lnxyls.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://kc.nszjky.cn

[Q61] 移动平均
来源：http://ar.shxzskj.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://eb.szsharing.cn

[Q62] 分组占比
来源：http://ux.hnjuh.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mw.muxihuayi.cn

[Q63] 开启事务
来源：http://vs.lnxyls.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://rq.jianghongdianzi.cn

[Q64] 提交事务
来源：http://fz.lnxyls.cn

COMMIT;
来源：http://mo.huixinmuqiang.cn

[Q65] 回滚事务
来源：http://dd.jctech888.com.cn

ROLLBACK;
来源：http://jk.lnxyls.cn

[Q66] 行锁查询
来源：http://wh.newstarts.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://al.9csxet.cn

[Q67] 设置隔离级别
来源：http://or.yuntaijiaju.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://tc.shtwfgs.cn

[Q68] 保存点
来源：http://yz.bookmarksfly.cn

SAVEPOINT sp1;
来源：http://lj.shxzukj.cn

ROLLBACK TO sp1;
来源：http://kr.szsharing.cn

[Q69] 查看执行计划
来源：http://bg.huanxung.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://en.szxytkj.cn

[Q70] 更新统计信息
来源：http://gr.lnxyls.cn

ANALYZE TABLE users;
来源：http://if.521024.cn

[Q71] 查看建表语句
来源：http://md.muxihuayi.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://oo.jctech888.com.cn

[Q72] 查看索引
来源：http://tp.muxihuayi.cn

SHOW INDEX FROM users;
来源：http://re.huixiangedu.cn

[Q73] 查看表状态
来源：http://hb.jianghongdianzi.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://bw.huixiangedu.cn

[Q74] 强制使用索引
来源：http://yj.chemitech.net.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://it.jctech888.com.cn

[Q75] 日期格式化
来源：http://jy.muxihuayi.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://go.bjjhwx.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://pw.huixiangedu.cn

[Q76] 按天统计
来源：http://ed.jctech888.com.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wq.bookmarksfly.cn

[Q77] 时间加减
来源：http://fc.bjjhwx.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://uw.chemitech.net.cn

[Q78] 当前时间
来源：http://dh.hahajie.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hx.huanxung.cn

[Q79] 字符串拼接
来源：http://rb.bjjhwx.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://sm.9csxet.cn

[Q80] 字符串截取
来源：http://dd.haigaiapp.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://od.huixinmuqiang.cn

[Q81] 字符串替换
来源：http://pl.huixiangedu.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hf.colortex.cn

[Q82] 字符长度与字节长度
来源：http://vh.yuexingan06.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://bp.huixiangedu.cn

[Q83] 大小写转换
来源：http://dp.hahajie.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://tg.huixiangedu.cn

[Q84] 去除首尾空格
来源：http://mf.yuntaijiaju.cn

SELECT TRIM(name) FROM users;
来源：http://av.wgjwhj.cn

[Q85] 数值取整
来源：http://vx.shtwfgs.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wu.shxzukj.cn

[Q86] 读取 JSON 字段
来源：http://sb.bookmarksfly.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://uf.huixiangedu.cn

[Q87] JSON 字段做条件
来源：http://iz.chemitech.net.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://fv.lnxyls.cn

[Q88] 行转列（条件聚合）
来源：http://vv.szxytkj.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://br.huixiangedu.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://en.nszjky.cn

[Q89] 判断表是否存在
来源：http://fc.yuntaijiaju.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ru.panjiajie.cn

[Q90] 生成序号列
来源：http://ne.hnjuh.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://yy.shxzskj.cn

================================================================================
来源：http://tu.bjjhwx.cn

R. Bash 专题
来源：http://cr.bjjhwx.cn

================================================================================
来源：http://lr.jianghongdianzi.cn

[R01] shebang 与严格模式
来源：http://go.9csxet.cn

#!/usr/bin/env bash
来源：http://dd.hnjuh.cn

set -euo pipefail
来源：http://zg.gzmigu.cn

[R02] 变量赋值与使用
来源：http://um.nicolike.cn

name="Tom"; echo "$name"
来源：http://ic.colortex.cn

[R03] 只读变量
来源：http://jr.nszjky.cn

readonly PI=3.14
来源：http://ck.huixiangedu.cn

[R04] 位置参数
来源：http://fp.shxzskj.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://rv.bjjhwx.cn

[R05] 参数默认值
来源：http://pe.jctech888.com.cn

name="${1:-default}"
来源：http://vg.colortex.cn

[R06] 判断命令是否存在
来源：http://tr.nicolike.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://sm.wgjwhj.cn

[R07] if 判断文件
来源：http://qg.newstarts.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://bz.yuntaijiaju.cn

[R08] 数值比较
来源：http://fu.wgjwhj.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://zq.colortex.cn

[R09] 字符串比较
来源：http://bh.huanxung.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://cc.nicolike.cn

[R10] 正则匹配
来源：http://hy.shtwfgs.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://gj.asd995.cn

[R11] case 多分支
来源：http://qf.jianghongdianzi.cn

case "$1" in
来源：http://hj.gzmigu.cn

start) echo "启动" ;;
来源：http://es.521024.cn

stop)  echo "停止" ;;
来源：http://ti.bookmarksfly.cn

*)     echo "未知命令" ;;
来源：http://pl.wgjwhj.cn

esac
来源：http://ij.lnxyls.cn

[R12] for 遍历文件
来源：http://wc.haigaiapp.cn

for f in *.txt; do echo "$f"; done
来源：http://zj.shxzskj.cn

[R13] for 计数循环
来源：http://qe.szxytkj.cn

for i in {1..10}; do echo "$i"; done
来源：http://aq.yuexingan06.cn

[R14] C 风格 for
来源：http://od.wgjwhj.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://cs.hahajie.cn

[R15] while 逐行读文件
来源：http://ou.nszjky.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ra.newstarts.cn

[R16] until 等待条件
来源：http://ph.hnjuh.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://cw.jctech888.com.cn

[R17] 数组定义与取值
来源：http://gg.bjjhwx.cn

arr=(a b c); echo "${arr[0]}"
来源：http://cp.haigaiapp.cn

[R18] 遍历数组
来源：http://bi.colortex.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ms.bjjhwx.cn

[R19] 数组长度
来源：http://xl.bookmarksfly.cn

echo "${#arr[@]}"
来源：http://hx.asd995.cn

[R20] 关联数组（字典）
来源：http://el.szxytkj.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ph.jctech888.com.cn

[R21] 字符串长度
来源：http://nr.jianghongdianzi.cn

echo "${#s}"
来源：http://rk.huixinmuqiang.cn

[R22] 截取子串
来源：http://ot.jianghongdianzi.cn

echo "${s:0:5}"
来源：http://og.colortex.cn

[R23] 字符串替换
来源：http://hm.panjiajie.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ok.jctech888.com.cn

[R24] 大小写转换
来源：http://uv.szsharing.cn

echo "${s^^}"; echo "${s,,}"
来源：http://yn.huixinmuqiang.cn

[R25] 去后缀 / 去前缀
来源：http://pu.nicolike.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://eq.wgjwhj.cn

[R26] 命令替换
来源：http://ei.newstarts.cn

now=$(date +%F); echo "$now"
来源：http://sv.huixinmuqiang.cn

[R27] 算术展开
来源：http://iq.hahajie.cn

echo $((1 + 2 * 3))
来源：http://lg.shtwfgs.cn

[R28] 浮点运算
来源：http://pc.chemitech.net.cn

echo "scale=2; 10/3" | bc
来源：http://je.colortex.cn

[R29] 定义函数
来源：http://tz.bjjhwx.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://tz.nicolike.cn

[R30] 函数返回状态码
来源：http://or.yuexingan06.cn

f() { return 0; }; f || echo "失败了"
来源：http://re.newstarts.cn

[R31] 局部变量
来源：http://sx.9csxet.cn

f() { local x=1; echo "$x"; }
来源：http://nz.jctech888.com.cn

[R32] 参数个数校验
来源：http://sk.colortex.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://dv.shxzukj.cn

[R33] 捕获错误并提示行号
来源：http://rw.huixinmuqiang.cn


<!-- 参考信息 -->