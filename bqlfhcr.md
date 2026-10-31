代发 wailian999

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://km.yuexingan06.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://fc.gzmigu.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://nz.yuntaijiaju.cn

PHP:  if (empty($x)) {}
来源：http://gf.bookmarksfly.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://lc.9csxet.cn

TS:   if (x == null) {}
来源：http://du.jianghongdianzi.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://mt.colortex.cn

Go:   if x == nil {}
来源：http://nk.huanxung.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://if.bookmarksfly.cn

C#:   if (x is null) {}
来源：http://tm.huanxung.cn

[P07] 防抖与节流
来源：http://np.gzmigu.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://gy.nicolike.cn

PHP:  // 手写时间戳比较
来源：http://dh.haigaiapp.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://nt.jctech888.com.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://rj.huixinmuqiang.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wg.shtwfgs.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ka.bjjhwx.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://tm.9csxet.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ej.wgjwhj.cn

[P08] 处理浮点精度问题
来源：http://jm.hahajie.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://vo.panjiajie.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://bc.wgjwhj.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://pv.nicolike.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wg.nszjky.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://oj.szsharing.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ly.huanxung.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://qb.bookmarksfly.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://oc.colortex.cn

================================================================================
来源：http://wm.wgjwhj.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ge.nszjky.cn

================================================================================
来源：http://yn.wgjwhj.cn

[Q01] 创建表
来源：http://hn.hahajie.cn

CREATE TABLE users (
来源：http://ls.jianghongdianzi.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://lj.bjjhwx.cn

name VARCHAR(50) NOT NULL,
来源：http://pm.hnjuh.cn

email VARCHAR(100) UNIQUE,
来源：http://ep.yuntaijiaju.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://sb.panjiajie.cn

);
来源：http://pg.wgjwhj.cn

[Q02] 创建带外键的表
来源：http://pv.shtwfgs.cn

CREATE TABLE orders (
来源：http://re.hahajie.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wh.shxzukj.cn

user_id INT NOT NULL,
来源：http://jd.shxzukj.cn

amount DECIMAL(10, 2),
来源：http://xl.colortex.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://zw.asd995.cn

);
来源：http://zt.yuntaijiaju.cn

[Q03] 增加列
来源：http://ub.huixinmuqiang.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://fm.jctech888.com.cn

[Q04] 修改列类型
来源：http://zx.asd995.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://vd.huanxung.cn

[Q05] 重命名列
来源：http://rm.huixinmuqiang.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://yg.muxihuayi.cn

[Q06] 删除列
来源：http://fg.asd995.cn

ALTER TABLE users DROP COLUMN age;
来源：http://ip.newstarts.cn

[Q07] 删除表
来源：http://ah.shxzskj.cn

DROP TABLE IF EXISTS orders;
来源：http://uk.wgjwhj.cn

[Q08] 创建普通索引
来源：http://jf.hahajie.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://jk.colortex.cn

[Q09] 创建唯一索引
来源：http://th.szxytkj.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://xd.9csxet.cn

[Q10] 插入单行
来源：http://qc.shxzukj.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://un.huixiangedu.cn

[Q11] 一次插入多行
来源：http://vf.hnjuh.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://to.huixinmuqiang.cn

[Q12] 插入后取自增 ID
来源：http://wf.521024.cn

INSERT INTO users (name) VALUES ('C');
来源：http://ye.yuexingan06.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://gv.gzmigu.cn

[Q13] 忽略重复插入
来源：http://dd.shxzukj.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://fa.nszjky.cn

[Q14] 存在则更新（upsert）
来源：http://rp.bjjhwx.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://zu.hahajie.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ug.newstarts.cn

[Q15] 查询全部
来源：http://be.colortex.cn

SELECT * FROM users;
来源：http://yc.szxytkj.cn

[Q16] 查询指定列
来源：http://uk.9csxet.cn

SELECT id, name FROM users;
来源：http://va.huixinmuqiang.cn

[Q17] 条件查询
来源：http://qa.asd995.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mc.huixiangedu.cn

[Q18] 模糊匹配
来源：http://xq.gzmigu.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://qo.shxzukj.cn

[Q19] 范围查询
来源：http://re.szsharing.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wf.nicolike.cn

[Q20] IN 列表
来源：http://gc.huanxung.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://kc.yuexingan06.cn

[Q21] 空值判断
来源：http://di.muxihuayi.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://qy.nicolike.cn

[Q22] 排序
来源：http://jo.nicolike.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://of.jctech888.com.cn

[Q23] 分页
来源：http://ft.shxzskj.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mu.gzmigu.cn

[Q24] 去重
来源：http://tc.bookmarksfly.cn

SELECT DISTINCT city FROM users;
来源：http://bc.hnjuh.cn

[Q25] 只取前 N 条
来源：http://tj.hnjuh.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ul.muxihuayi.cn

[Q26] 计数
来源：http://ng.panjiajie.cn

SELECT COUNT(*) FROM users;
来源：http://me.colortex.cn

[Q27] 条件计数
来源：http://ka.nicolike.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wv.bookmarksfly.cn

[Q28] 求和与平均
来源：http://sg.huixinmuqiang.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://vz.521024.cn

[Q29] 最大最小值
来源：http://bi.lnxyls.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://vw.szxytkj.cn

[Q30] 分组统计
来源：http://di.bjjhwx.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ts.huanxung.cn

[Q31] 分组后过滤
来源：http://ad.gzmigu.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://qk.newstarts.cn

[Q32] 分组拼接字符串
来源：http://zx.jianghongdianzi.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ns.colortex.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://eo.bookmarksfly.cn

[Q33] 多列分组
来源：http://sm.newstarts.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://rp.shtwfgs.cn

[Q34] 每组取第一条
来源：http://jg.hahajie.cn

SELECT * FROM (
来源：http://jw.bookmarksfly.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wq.yuntaijiaju.cn

) t WHERE rn = 1;
来源：http://ub.asd995.cn

[Q35] 内连接
来源：http://wh.lnxyls.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://fv.huanxung.cn

[Q36] 左连接
来源：http://en.huanxung.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ao.yuntaijiaju.cn

[Q37] 右连接
来源：http://fr.hnjuh.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ru.gzmigu.cn

[Q38] 全外连接（PostgreSQL）
来源：http://rz.colortex.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wp.huixinmuqiang.cn

[Q39] 自连接（查上下级）
来源：http://eo.nicolike.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://wh.szxytkj.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://qk.hahajie.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://rg.huixiangedu.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://qz.muxihuayi.cn

[Q41] 多表连接
来源：http://eg.shtwfgs.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://cm.bjjhwx.cn

JOIN users u ON u.id = o.user_id
来源：http://yl.hahajie.cn

JOIN products p ON p.id = o.product_id;
来源：http://oz.nszjky.cn

[Q42] 连接条件附加过滤
来源：http://mb.shxzskj.cn

SELECT u.name, o.amount FROM users u
来源：http://wb.huanxung.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wu.gzmigu.cn

[Q43] 标量子查询
来源：http://tv.yuexingan06.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://fj.asd995.cn

[Q44] IN 子查询
来源：http://ye.szsharing.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://nz.panjiajie.cn

[Q45] EXISTS 判断存在
来源：http://fo.huanxung.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://lh.jctech888.com.cn

[Q46] NOT EXISTS 判断不存在
来源：http://fg.gzmigu.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hb.huanxung.cn

[Q47] 与平均值比较
来源：http://du.bookmarksfly.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://av.huixiangedu.cn

[Q48] CTE 公用表表达式
来源：http://in.wgjwhj.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ya.yuntaijiaju.cn

SELECT * FROM t WHERE c > 5;
来源：http://sg.chemitech.net.cn

[Q49] 更新单行
来源：http://ma.jianghongdianzi.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wz.bjjhwx.cn

[Q50] 批量更新
来源：http://lq.hnjuh.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://co.lnxyls.cn

[Q51] 用子查询更新
来源：http://ud.hahajie.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wb.shtwfgs.cn

[Q52] 删除指定行
来源：http://ei.huixinmuqiang.cn

DELETE FROM users WHERE id = 10;
来源：http://dg.yuexingan06.cn

[Q53] 按条件删除
来源：http://eu.huanxung.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://im.shtwfgs.cn

[Q54] 清空表
来源：http://du.bookmarksfly.cn

TRUNCATE TABLE logs;
来源：http://vq.chemitech.net.cn

[Q55] 排名（并列占位）
来源：http://oh.haigaiapp.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://pl.colortex.cn

[Q56] 密集排名（并列不占位）
来源：http://qy.shxzukj.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ah.huixinmuqiang.cn

[Q57] 行号
来源：http://ii.huanxung.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://sw.521024.cn

[Q58] 累计求和
来源：http://qj.shxzukj.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://xm.bookmarksfly.cn

[Q59] 分组内累计
来源：http://bu.hahajie.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://qv.colortex.cn

[Q60] 取上一行 / 下一行
来源：http://ar.szxytkj.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hi.asd995.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://kr.colortex.cn

[Q61] 移动平均
来源：http://gq.huixinmuqiang.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://uu.szsharing.cn

[Q62] 分组占比
来源：http://nb.lnxyls.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://up.huanxung.cn

[Q63] 开启事务
来源：http://zf.521024.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://av.chemitech.net.cn

[Q64] 提交事务
来源：http://vz.shxzukj.cn

COMMIT;
来源：http://kp.huanxung.cn

[Q65] 回滚事务
来源：http://lf.nszjky.cn

ROLLBACK;
来源：http://lb.lnxyls.cn

[Q66] 行锁查询
来源：http://lt.bjjhwx.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://pt.muxihuayi.cn

[Q67] 设置隔离级别
来源：http://yj.9csxet.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://xp.panjiajie.cn

[Q68] 保存点
来源：http://xf.chemitech.net.cn

SAVEPOINT sp1;
来源：http://sh.jctech888.com.cn

ROLLBACK TO sp1;
来源：http://xd.bjjhwx.cn

[Q69] 查看执行计划
来源：http://fq.szxytkj.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://sy.colortex.cn

[Q70] 更新统计信息
来源：http://rv.wgjwhj.cn

ANALYZE TABLE users;
来源：http://hc.nicolike.cn

[Q71] 查看建表语句
来源：http://ri.wgjwhj.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://cn.haigaiapp.cn

[Q72] 查看索引
来源：http://fh.nicolike.cn

SHOW INDEX FROM users;
来源：http://no.shtwfgs.cn

[Q73] 查看表状态
来源：http://uv.nicolike.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://cc.bookmarksfly.cn

[Q74] 强制使用索引
来源：http://zv.hnjuh.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://uv.jctech888.com.cn

[Q75] 日期格式化
来源：http://rd.haigaiapp.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ca.chemitech.net.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://oj.muxihuayi.cn

[Q76] 按天统计
来源：http://pp.lnxyls.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ss.wgjwhj.cn

[Q77] 时间加减
来源：http://fz.bjjhwx.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://pm.asd995.cn

[Q78] 当前时间
来源：http://by.shtwfgs.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ku.hahajie.cn

[Q79] 字符串拼接
来源：http://qh.nicolike.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://oj.9csxet.cn

[Q80] 字符串截取
来源：http://yu.gzmigu.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://lf.jianghongdianzi.cn

[Q81] 字符串替换
来源：http://mv.szsharing.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ak.hnjuh.cn

[Q82] 字符长度与字节长度
来源：http://wt.shxzukj.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://la.muxihuayi.cn

[Q83] 大小写转换
来源：http://bz.chemitech.net.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://pd.panjiajie.cn

[Q84] 去除首尾空格
来源：http://qg.bookmarksfly.cn

SELECT TRIM(name) FROM users;
来源：http://mh.panjiajie.cn

[Q85] 数值取整
来源：http://hg.panjiajie.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ew.521024.cn

[Q86] 读取 JSON 字段
来源：http://ee.panjiajie.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://li.nicolike.cn

[Q87] JSON 字段做条件
来源：http://dn.haigaiapp.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://rg.szxytkj.cn

[Q88] 行转列（条件聚合）
来源：http://ps.nicolike.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ha.huixinmuqiang.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ss.shxzskj.cn

[Q89] 判断表是否存在
来源：http://sv.nszjky.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://yh.huanxung.cn

[Q90] 生成序号列
来源：http://an.hnjuh.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ja.jianghongdianzi.cn

================================================================================
来源：http://yg.hnjuh.cn

R. Bash 专题
来源：http://pp.nicolike.cn

================================================================================
来源：http://mv.szsharing.cn

[R01] shebang 与严格模式
来源：http://ai.jctech888.com.cn

#!/usr/bin/env bash
来源：http://mo.muxihuayi.cn

set -euo pipefail
来源：http://tl.nicolike.cn

[R02] 变量赋值与使用
来源：http://qa.yuntaijiaju.cn

name="Tom"; echo "$name"
来源：http://lz.shxzskj.cn

[R03] 只读变量
来源：http://pb.panjiajie.cn

readonly PI=3.14
来源：http://ba.yuexingan06.cn

[R04] 位置参数
来源：http://mu.huixiangedu.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://nt.huanxung.cn

[R05] 参数默认值
来源：http://zx.nszjky.cn

name="${1:-default}"
来源：http://wh.gzmigu.cn

[R06] 判断命令是否存在
来源：http://we.yuntaijiaju.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://vz.szxytkj.cn

[R07] if 判断文件
来源：http://nd.asd995.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://fi.yuntaijiaju.cn

[R08] 数值比较
来源：http://bp.nicolike.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://oy.bookmarksfly.cn

[R09] 字符串比较
来源：http://qf.haigaiapp.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://nm.9csxet.cn

[R10] 正则匹配
来源：http://jc.huixiangedu.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://th.9csxet.cn

[R11] case 多分支
来源：http://ep.szsharing.cn

case "$1" in
来源：http://hc.jianghongdianzi.cn

start) echo "启动" ;;
来源：http://lz.yuntaijiaju.cn

stop)  echo "停止" ;;
来源：http://yq.shxzskj.cn

*)     echo "未知命令" ;;
来源：http://wf.huixinmuqiang.cn

esac
来源：http://pn.jctech888.com.cn

[R12] for 遍历文件
来源：http://jl.wgjwhj.cn

for f in *.txt; do echo "$f"; done
来源：http://iq.9csxet.cn

[R13] for 计数循环
来源：http://eo.521024.cn

for i in {1..10}; do echo "$i"; done
来源：http://qd.szsharing.cn

[R14] C 风格 for
来源：http://jg.shtwfgs.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ry.shxzskj.cn

[R15] while 逐行读文件
来源：http://em.hahajie.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://sm.colortex.cn

[R16] until 等待条件
来源：http://pk.lnxyls.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://jx.jctech888.com.cn

[R17] 数组定义与取值
来源：http://zq.panjiajie.cn

arr=(a b c); echo "${arr[0]}"
来源：http://ha.wgjwhj.cn

[R18] 遍历数组
来源：http://wu.huixiangedu.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://tk.shtwfgs.cn

[R19] 数组长度
来源：http://hb.wgjwhj.cn

echo "${#arr[@]}"
来源：http://qf.colortex.cn

[R20] 关联数组（字典）
来源：http://iw.haigaiapp.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://rf.colortex.cn

[R21] 字符串长度
来源：http://ow.muxihuayi.cn

echo "${#s}"
来源：http://aa.huanxung.cn

[R22] 截取子串
来源：http://iw.hnjuh.cn

echo "${s:0:5}"
来源：http://lk.521024.cn

[R23] 字符串替换
来源：http://dr.9csxet.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://jt.wgjwhj.cn

[R24] 大小写转换
来源：http://or.bookmarksfly.cn

echo "${s^^}"; echo "${s,,}"
来源：http://ao.hahajie.cn

[R25] 去后缀 / 去前缀
来源：http://tl.shxzukj.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://ju.newstarts.cn

[R26] 命令替换
来源：http://lt.nszjky.cn

now=$(date +%F); echo "$now"
来源：http://kx.jctech888.com.cn

[R27] 算术展开
来源：http://cd.newstarts.cn

echo $((1 + 2 * 3))
来源：http://kp.9csxet.cn

[R28] 浮点运算
来源：http://ca.huixiangedu.cn

echo "scale=2; 10/3" | bc
来源：http://er.bookmarksfly.cn

[R29] 定义函数
来源：http://ft.shxzukj.cn


<!-- 参考信息 -->