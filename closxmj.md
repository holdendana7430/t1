代发 wailian999

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ka.colortex.cn

TS:   if (x == null) {}
来源：http://qs.shxzskj.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://kh.colortex.cn

Go:   if x == nil {}
来源：http://we.lnxyls.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://lk.9csxet.cn

C#:   if (x is null) {}
来源：http://ah.shtwfgs.cn

[P07] 防抖与节流
来源：http://yq.nicolike.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://vc.yuexingan06.cn

PHP:  // 手写时间戳比较
来源：http://rw.lnxyls.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://nl.shxzukj.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://uz.yuexingan06.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hb.jctech888.com.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://fc.lnxyls.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://ga.hnjuh.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://pm.chemitech.net.cn

[P08] 处理浮点精度问题
来源：http://nd.szsharing.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ju.panjiajie.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://dz.nicolike.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://oa.szsharing.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://fh.yuntaijiaju.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://li.muxihuayi.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://yw.gzmigu.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://tx.asd995.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://kk.huanxung.cn

================================================================================
来源：http://xq.yuexingan06.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://zz.nicolike.cn

================================================================================
来源：http://zb.yuexingan06.cn

[Q01] 创建表
来源：http://fe.yuntaijiaju.cn

CREATE TABLE users (
来源：http://ry.hnjuh.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://kt.nszjky.cn

name VARCHAR(50) NOT NULL,
来源：http://tk.521024.cn

email VARCHAR(100) UNIQUE,
来源：http://tu.jctech888.com.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ru.jctech888.com.cn

);
来源：http://yk.jctech888.com.cn

[Q02] 创建带外键的表
来源：http://fp.yuexingan06.cn

CREATE TABLE orders (
来源：http://ue.9csxet.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://na.hahajie.cn

user_id INT NOT NULL,
来源：http://ku.9csxet.cn

amount DECIMAL(10, 2),
来源：http://uh.lnxyls.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wj.huanxung.cn

);
来源：http://iu.szxytkj.cn

[Q03] 增加列
来源：http://hi.hahajie.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://vb.bookmarksfly.cn

[Q04] 修改列类型
来源：http://kr.yuntaijiaju.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ga.521024.cn

[Q05] 重命名列
来源：http://qt.asd995.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://rb.szxytkj.cn

[Q06] 删除列
来源：http://kz.szxytkj.cn

ALTER TABLE users DROP COLUMN age;
来源：http://dx.haigaiapp.cn

[Q07] 删除表
来源：http://bk.jianghongdianzi.cn

DROP TABLE IF EXISTS orders;
来源：http://aa.yuntaijiaju.cn

[Q08] 创建普通索引
来源：http://wu.nicolike.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://rm.huixinmuqiang.cn

[Q09] 创建唯一索引
来源：http://sy.muxihuayi.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://da.521024.cn

[Q10] 插入单行
来源：http://zr.lnxyls.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://xh.jianghongdianzi.cn

[Q11] 一次插入多行
来源：http://wc.colortex.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://cn.yuexingan06.cn

[Q12] 插入后取自增 ID
来源：http://qf.asd995.cn

INSERT INTO users (name) VALUES ('C');
来源：http://bn.bookmarksfly.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://sy.yuexingan06.cn

[Q13] 忽略重复插入
来源：http://it.wgjwhj.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://vv.szxytkj.cn

[Q14] 存在则更新（upsert）
来源：http://kf.shxzukj.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wo.shxzukj.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://gt.shtwfgs.cn

[Q15] 查询全部
来源：http://du.shxzukj.cn

SELECT * FROM users;
来源：http://yz.newstarts.cn

[Q16] 查询指定列
来源：http://vv.hahajie.cn

SELECT id, name FROM users;
来源：http://os.huixiangedu.cn

[Q17] 条件查询
来源：http://pi.nszjky.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://yn.colortex.cn

[Q18] 模糊匹配
来源：http://bi.nszjky.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mt.lnxyls.cn

[Q19] 范围查询
来源：http://ny.yuntaijiaju.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://pn.huixinmuqiang.cn

[Q20] IN 列表
来源：http://fg.hahajie.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://nk.gzmigu.cn

[Q21] 空值判断
来源：http://ua.haigaiapp.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://mm.haigaiapp.cn

[Q22] 排序
来源：http://ad.yuntaijiaju.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://dk.wgjwhj.cn

[Q23] 分页
来源：http://qo.bookmarksfly.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://te.colortex.cn

[Q24] 去重
来源：http://ju.nicolike.cn

SELECT DISTINCT city FROM users;
来源：http://ka.hnjuh.cn

[Q25] 只取前 N 条
来源：http://dn.bjjhwx.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wp.jctech888.com.cn

[Q26] 计数
来源：http://ll.shxzukj.cn

SELECT COUNT(*) FROM users;
来源：http://nc.asd995.cn

[Q27] 条件计数
来源：http://iv.lnxyls.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ff.asd995.cn

[Q28] 求和与平均
来源：http://bh.nicolike.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://pe.gzmigu.cn

[Q29] 最大最小值
来源：http://db.huixiangedu.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://wj.huixiangedu.cn

[Q30] 分组统计
来源：http://he.szsharing.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://iw.shtwfgs.cn

[Q31] 分组后过滤
来源：http://pp.szxytkj.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://gn.szxytkj.cn

[Q32] 分组拼接字符串
来源：http://sg.szxytkj.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://pc.shxzukj.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://fc.yuexingan06.cn

[Q33] 多列分组
来源：http://id.huanxung.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://eh.gzmigu.cn

[Q34] 每组取第一条
来源：http://ap.wgjwhj.cn

SELECT * FROM (
来源：http://xb.huixiangedu.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://rl.nicolike.cn

) t WHERE rn = 1;
来源：http://so.chemitech.net.cn

[Q35] 内连接
来源：http://tq.9csxet.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wv.shxzskj.cn

[Q36] 左连接
来源：http://bo.bjjhwx.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://pj.jctech888.com.cn

[Q37] 右连接
来源：http://tv.hahajie.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://pc.lnxyls.cn

[Q38] 全外连接（PostgreSQL）
来源：http://tn.lnxyls.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://il.9csxet.cn

[Q39] 自连接（查上下级）
来源：http://wc.521024.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://sx.hahajie.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ap.521024.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://cs.shxzskj.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://xm.hahajie.cn

[Q41] 多表连接
来源：http://ru.521024.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://ni.gzmigu.cn

JOIN users u ON u.id = o.user_id
来源：http://jk.bjjhwx.cn

JOIN products p ON p.id = o.product_id;
来源：http://sb.nszjky.cn

[Q42] 连接条件附加过滤
来源：http://bi.huanxung.cn

SELECT u.name, o.amount FROM users u
来源：http://yz.nszjky.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hi.lnxyls.cn

[Q43] 标量子查询
来源：http://fl.bjjhwx.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://zs.lnxyls.cn

[Q44] IN 子查询
来源：http://gc.nicolike.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://nr.bookmarksfly.cn

[Q45] EXISTS 判断存在
来源：http://mi.nszjky.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://nn.shxzukj.cn

[Q46] NOT EXISTS 判断不存在
来源：http://ds.colortex.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://td.nicolike.cn

[Q47] 与平均值比较
来源：http://ol.muxihuayi.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hd.newstarts.cn

[Q48] CTE 公用表表达式
来源：http://cb.panjiajie.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://uk.huixiangedu.cn

SELECT * FROM t WHERE c > 5;
来源：http://la.huixiangedu.cn

[Q49] 更新单行
来源：http://ho.chemitech.net.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ni.newstarts.cn

[Q50] 批量更新
来源：http://bt.szxytkj.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hn.hnjuh.cn

[Q51] 用子查询更新
来源：http://wv.colortex.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://lx.jianghongdianzi.cn

[Q52] 删除指定行
来源：http://bo.jctech888.com.cn

DELETE FROM users WHERE id = 10;
来源：http://gp.colortex.cn

[Q53] 按条件删除
来源：http://lf.lnxyls.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://qb.hahajie.cn

[Q54] 清空表
来源：http://ob.szxytkj.cn

TRUNCATE TABLE logs;
来源：http://bn.bjjhwx.cn

[Q55] 排名（并列占位）
来源：http://yk.asd995.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://iq.chemitech.net.cn

[Q56] 密集排名（并列不占位）
来源：http://tj.shtwfgs.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://fl.bookmarksfly.cn

[Q57] 行号
来源：http://jl.szxytkj.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://tc.chemitech.net.cn

[Q58] 累计求和
来源：http://sw.shxzukj.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://qx.huixiangedu.cn

[Q59] 分组内累计
来源：http://gq.jctech888.com.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://lg.hahajie.cn

[Q60] 取上一行 / 下一行
来源：http://ai.bjjhwx.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://jj.9csxet.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://bl.huixiangedu.cn

[Q61] 移动平均
来源：http://dk.jctech888.com.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://xp.panjiajie.cn

[Q62] 分组占比
来源：http://wg.szxytkj.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hb.szxytkj.cn

[Q63] 开启事务
来源：http://bl.chemitech.net.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://gd.huixinmuqiang.cn

[Q64] 提交事务
来源：http://gl.jianghongdianzi.cn

COMMIT;
来源：http://va.huixinmuqiang.cn

[Q65] 回滚事务
来源：http://by.nszjky.cn

ROLLBACK;
来源：http://dw.asd995.cn

[Q66] 行锁查询
来源：http://sx.nicolike.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://by.colortex.cn

[Q67] 设置隔离级别
来源：http://tb.newstarts.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://rp.nicolike.cn

[Q68] 保存点
来源：http://cg.szxytkj.cn

SAVEPOINT sp1;
来源：http://uu.haigaiapp.cn

ROLLBACK TO sp1;
来源：http://is.hnjuh.cn

[Q69] 查看执行计划
来源：http://qw.jctech888.com.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://xl.huixinmuqiang.cn

[Q70] 更新统计信息
来源：http://dh.newstarts.cn

ANALYZE TABLE users;
来源：http://tj.colortex.cn

[Q71] 查看建表语句
来源：http://uf.hahajie.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://lq.chemitech.net.cn

[Q72] 查看索引
来源：http://av.gzmigu.cn

SHOW INDEX FROM users;
来源：http://im.muxihuayi.cn

[Q73] 查看表状态
来源：http://cr.haigaiapp.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://by.hahajie.cn

[Q74] 强制使用索引
来源：http://nn.asd995.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ja.huixinmuqiang.cn

[Q75] 日期格式化
来源：http://rz.haigaiapp.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ii.bookmarksfly.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://bs.huanxung.cn

[Q76] 按天统计
来源：http://ec.hnjuh.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://fl.wgjwhj.cn

[Q77] 时间加减
来源：http://ex.521024.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://dl.9csxet.cn

[Q78] 当前时间
来源：http://tj.colortex.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://sg.9csxet.cn

[Q79] 字符串拼接
来源：http://gx.haigaiapp.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mr.shtwfgs.cn

[Q80] 字符串截取
来源：http://ki.jctech888.com.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://vn.bjjhwx.cn

[Q81] 字符串替换
来源：http://cu.bjjhwx.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ks.nszjky.cn

[Q82] 字符长度与字节长度
来源：http://nh.gzmigu.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://zu.yuntaijiaju.cn

[Q83] 大小写转换
来源：http://ay.muxihuayi.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://lw.lnxyls.cn

[Q84] 去除首尾空格
来源：http://tm.521024.cn

SELECT TRIM(name) FROM users;
来源：http://dy.shxzskj.cn

[Q85] 数值取整
来源：http://oq.huixiangedu.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://xd.shxzukj.cn

[Q86] 读取 JSON 字段
来源：http://nn.newstarts.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ur.muxihuayi.cn

[Q87] JSON 字段做条件
来源：http://bq.gzmigu.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://rp.hnjuh.cn

[Q88] 行转列（条件聚合）
来源：http://iz.lnxyls.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mu.colortex.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://kp.yuntaijiaju.cn

[Q89] 判断表是否存在
来源：http://rc.shxzskj.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://dz.shxzukj.cn

[Q90] 生成序号列
来源：http://oa.521024.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://fb.shtwfgs.cn

================================================================================
来源：http://zl.hnjuh.cn

R. Bash 专题
来源：http://so.chemitech.net.cn

================================================================================
来源：http://yx.gzmigu.cn

[R01] shebang 与严格模式
来源：http://gj.lnxyls.cn

#!/usr/bin/env bash
来源：http://cp.gzmigu.cn

set -euo pipefail
来源：http://fi.panjiajie.cn

[R02] 变量赋值与使用
来源：http://vl.nszjky.cn

name="Tom"; echo "$name"
来源：http://ih.gzmigu.cn

[R03] 只读变量
来源：http://rc.szxytkj.cn

readonly PI=3.14
来源：http://je.nicolike.cn

[R04] 位置参数
来源：http://af.asd995.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ag.szsharing.cn

[R05] 参数默认值
来源：http://kz.lnxyls.cn

name="${1:-default}"
来源：http://zg.jianghongdianzi.cn

[R06] 判断命令是否存在
来源：http://zq.szxytkj.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://pj.bookmarksfly.cn

[R07] if 判断文件
来源：http://ee.wgjwhj.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://jm.bjjhwx.cn

[R08] 数值比较
来源：http://bs.9csxet.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://nz.szsharing.cn

[R09] 字符串比较
来源：http://yo.huixinmuqiang.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ia.bjjhwx.cn

[R10] 正则匹配
来源：http://js.yuntaijiaju.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ue.nszjky.cn

[R11] case 多分支
来源：http://to.huanxung.cn

case "$1" in
来源：http://qp.huixinmuqiang.cn

start) echo "启动" ;;
来源：http://cp.hahajie.cn

stop)  echo "停止" ;;
来源：http://jo.jianghongdianzi.cn

*)     echo "未知命令" ;;
来源：http://gh.asd995.cn

esac
来源：http://no.bookmarksfly.cn

[R12] for 遍历文件
来源：http://kb.yuntaijiaju.cn

for f in *.txt; do echo "$f"; done
来源：http://tg.panjiajie.cn

[R13] for 计数循环
来源：http://ny.hahajie.cn

for i in {1..10}; do echo "$i"; done
来源：http://hc.szsharing.cn

[R14] C 风格 for
来源：http://qq.colortex.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://to.chemitech.net.cn

[R15] while 逐行读文件
来源：http://ez.newstarts.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://rh.wgjwhj.cn

[R16] until 等待条件
来源：http://jk.haigaiapp.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://om.colortex.cn

[R17] 数组定义与取值
来源：http://bd.szxytkj.cn

arr=(a b c); echo "${arr[0]}"
来源：http://sz.yuexingan06.cn

[R18] 遍历数组
来源：http://sj.gzmigu.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://aw.bjjhwx.cn

[R19] 数组长度
来源：http://nj.nicolike.cn

echo "${#arr[@]}"
来源：http://us.asd995.cn

[R20] 关联数组（字典）
来源：http://eh.shtwfgs.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://um.jianghongdianzi.cn

[R21] 字符串长度
来源：http://zs.bjjhwx.cn

echo "${#s}"
来源：http://ls.panjiajie.cn

[R22] 截取子串
来源：http://fy.newstarts.cn

echo "${s:0:5}"
来源：http://qj.jianghongdianzi.cn

[R23] 字符串替换
来源：http://fk.newstarts.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://iv.521024.cn

[R24] 大小写转换
来源：http://yz.wgjwhj.cn

echo "${s^^}"; echo "${s,,}"
来源：http://bt.colortex.cn

[R25] 去后缀 / 去前缀
来源：http://nl.nszjky.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://ca.yuexingan06.cn

[R26] 命令替换
来源：http://va.wgjwhj.cn

now=$(date +%F); echo "$now"
来源：http://we.chemitech.net.cn

[R27] 算术展开
来源：http://im.panjiajie.cn

echo $((1 + 2 * 3))
来源：http://ah.szsharing.cn

[R28] 浮点运算
来源：http://yz.chemitech.net.cn

echo "scale=2; 10/3" | bc
来源：http://jk.newstarts.cn

[R29] 定义函数
来源：http://jl.szsharing.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wz.asd995.cn

[R30] 函数返回状态码
来源：http://su.jianghongdianzi.cn

f() { return 0; }; f || echo "失败了"
来源：http://lj.bjjhwx.cn

[R31] 局部变量
来源：http://jr.shxzskj.cn


<!-- 参考信息 -->