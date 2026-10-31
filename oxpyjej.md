代发 wailian999

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://bz.huanxung.cn

C#:   if (x is null) {}
来源：http://ca.newstarts.cn

[P07] 防抖与节流
来源：http://ld.huixinmuqiang.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://xn.newstarts.cn

PHP:  // 手写时间戳比较
来源：http://gr.bookmarksfly.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hu.jctech888.com.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ev.9csxet.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://tx.szxytkj.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://et.shtwfgs.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://at.muxihuayi.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://yo.muxihuayi.cn

[P08] 处理浮点精度问题
来源：http://ic.szxytkj.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hj.asd995.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://qg.huanxung.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://it.yuntaijiaju.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://fs.9csxet.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://oz.newstarts.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://of.huixinmuqiang.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://zc.nicolike.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://lb.jianghongdianzi.cn

================================================================================
来源：http://dt.shxzukj.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://in.colortex.cn

================================================================================
来源：http://ny.newstarts.cn

[Q01] 创建表
来源：http://lp.hahajie.cn

CREATE TABLE users (
来源：http://ha.panjiajie.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://np.yuntaijiaju.cn

name VARCHAR(50) NOT NULL,
来源：http://va.colortex.cn

email VARCHAR(100) UNIQUE,
来源：http://nw.yuntaijiaju.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://jz.huanxung.cn

);
来源：http://gs.shtwfgs.cn

[Q02] 创建带外键的表
来源：http://of.nicolike.cn

CREATE TABLE orders (
来源：http://vt.muxihuayi.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ae.gzmigu.cn

user_id INT NOT NULL,
来源：http://up.bjjhwx.cn

amount DECIMAL(10, 2),
来源：http://fk.panjiajie.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://zz.521024.cn

);
来源：http://lt.szsharing.cn

[Q03] 增加列
来源：http://di.newstarts.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://gb.hnjuh.cn

[Q04] 修改列类型
来源：http://uo.yuexingan06.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ot.huanxung.cn

[Q05] 重命名列
来源：http://ku.jctech888.com.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://jh.hnjuh.cn

[Q06] 删除列
来源：http://hq.huixinmuqiang.cn

ALTER TABLE users DROP COLUMN age;
来源：http://if.9csxet.cn

[Q07] 删除表
来源：http://vz.huanxung.cn

DROP TABLE IF EXISTS orders;
来源：http://lu.bjjhwx.cn

[Q08] 创建普通索引
来源：http://bg.hnjuh.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://pz.yuntaijiaju.cn

[Q09] 创建唯一索引
来源：http://xz.asd995.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://nq.bookmarksfly.cn

[Q10] 插入单行
来源：http://rw.gzmigu.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://pr.hahajie.cn

[Q11] 一次插入多行
来源：http://of.jianghongdianzi.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ur.szsharing.cn

[Q12] 插入后取自增 ID
来源：http://vg.huixiangedu.cn

INSERT INTO users (name) VALUES ('C');
来源：http://fl.szxytkj.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://zg.shxzukj.cn

[Q13] 忽略重复插入
来源：http://td.yuntaijiaju.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://qi.chemitech.net.cn

[Q14] 存在则更新（upsert）
来源：http://hw.nszjky.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ad.panjiajie.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://go.hnjuh.cn

[Q15] 查询全部
来源：http://yg.9csxet.cn

SELECT * FROM users;
来源：http://th.shtwfgs.cn

[Q16] 查询指定列
来源：http://hi.wgjwhj.cn

SELECT id, name FROM users;
来源：http://pc.shxzukj.cn

[Q17] 条件查询
来源：http://qb.shtwfgs.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mq.gzmigu.cn

[Q18] 模糊匹配
来源：http://mi.huanxung.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://lo.shxzukj.cn

[Q19] 范围查询
来源：http://bm.hnjuh.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://qs.jianghongdianzi.cn

[Q20] IN 列表
来源：http://ip.yuntaijiaju.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://sg.hnjuh.cn

[Q21] 空值判断
来源：http://tp.newstarts.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://je.newstarts.cn

[Q22] 排序
来源：http://kh.521024.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://qw.bookmarksfly.cn

[Q23] 分页
来源：http://tt.shtwfgs.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://gp.chemitech.net.cn

[Q24] 去重
来源：http://ep.jianghongdianzi.cn

SELECT DISTINCT city FROM users;
来源：http://jl.gzmigu.cn

[Q25] 只取前 N 条
来源：http://vq.yuntaijiaju.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://po.shxzskj.cn

[Q26] 计数
来源：http://eg.yuexingan06.cn

SELECT COUNT(*) FROM users;
来源：http://hx.chemitech.net.cn

[Q27] 条件计数
来源：http://uf.huixiangedu.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://tl.muxihuayi.cn

[Q28] 求和与平均
来源：http://ql.szxytkj.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://tm.chemitech.net.cn

[Q29] 最大最小值
来源：http://cs.chemitech.net.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://em.jctech888.com.cn

[Q30] 分组统计
来源：http://ip.shtwfgs.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://jg.lnxyls.cn

[Q31] 分组后过滤
来源：http://ih.panjiajie.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://qm.wgjwhj.cn

[Q32] 分组拼接字符串
来源：http://sr.bjjhwx.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://fl.gzmigu.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ph.asd995.cn

[Q33] 多列分组
来源：http://aj.newstarts.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://fz.szxytkj.cn

[Q34] 每组取第一条
来源：http://hr.colortex.cn

SELECT * FROM (
来源：http://mu.bjjhwx.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hx.haigaiapp.cn

) t WHERE rn = 1;
来源：http://qq.szxytkj.cn

[Q35] 内连接
来源：http://xd.newstarts.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://vb.shtwfgs.cn

[Q36] 左连接
来源：http://mv.shxzukj.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://aj.gzmigu.cn

[Q37] 右连接
来源：http://wf.muxihuayi.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://qo.asd995.cn

[Q38] 全外连接（PostgreSQL）
来源：http://mu.haigaiapp.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://uu.muxihuayi.cn

[Q39] 自连接（查上下级）
来源：http://oc.szxytkj.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://ik.521024.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wa.shxzskj.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://ri.shxzskj.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://qs.colortex.cn

[Q41] 多表连接
来源：http://qt.jctech888.com.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://yx.newstarts.cn

JOIN users u ON u.id = o.user_id
来源：http://nu.521024.cn

JOIN products p ON p.id = o.product_id;
来源：http://tn.haigaiapp.cn

[Q42] 连接条件附加过滤
来源：http://bu.gzmigu.cn

SELECT u.name, o.amount FROM users u
来源：http://lw.huixiangedu.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wc.panjiajie.cn

[Q43] 标量子查询
来源：http://as.lnxyls.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hu.haigaiapp.cn

[Q44] IN 子查询
来源：http://tu.asd995.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://xe.nszjky.cn

[Q45] EXISTS 判断存在
来源：http://ot.panjiajie.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://zm.huanxung.cn

[Q46] NOT EXISTS 判断不存在
来源：http://hv.hnjuh.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://pu.yuntaijiaju.cn

[Q47] 与平均值比较
来源：http://hl.yuntaijiaju.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://lo.newstarts.cn

[Q48] CTE 公用表表达式
来源：http://uc.lnxyls.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ul.jctech888.com.cn

SELECT * FROM t WHERE c > 5;
来源：http://gh.huixinmuqiang.cn

[Q49] 更新单行
来源：http://ww.nszjky.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://kn.wgjwhj.cn

[Q50] 批量更新
来源：http://io.huixinmuqiang.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://yw.chemitech.net.cn

[Q51] 用子查询更新
来源：http://kw.shxzukj.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mm.9csxet.cn

[Q52] 删除指定行
来源：http://ny.huanxung.cn

DELETE FROM users WHERE id = 10;
来源：http://fr.huanxung.cn

[Q53] 按条件删除
来源：http://qi.chemitech.net.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://gr.colortex.cn

[Q54] 清空表
来源：http://yg.9csxet.cn

TRUNCATE TABLE logs;
来源：http://he.asd995.cn

[Q55] 排名（并列占位）
来源：http://pf.wgjwhj.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mc.asd995.cn

[Q56] 密集排名（并列不占位）
来源：http://nw.shxzskj.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://qg.shxzukj.cn

[Q57] 行号
来源：http://rf.newstarts.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://uv.nicolike.cn

[Q58] 累计求和
来源：http://yp.9csxet.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://bj.nszjky.cn

[Q59] 分组内累计
来源：http://dy.muxihuayi.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://tc.nszjky.cn

[Q60] 取上一行 / 下一行
来源：http://vn.lnxyls.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://uo.jctech888.com.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ik.huanxung.cn

[Q61] 移动平均
来源：http://yb.shxzskj.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mk.lnxyls.cn

[Q62] 分组占比
来源：http://ix.bjjhwx.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://gs.yuexingan06.cn

[Q63] 开启事务
来源：http://id.jctech888.com.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://dt.asd995.cn

[Q64] 提交事务
来源：http://hu.newstarts.cn

COMMIT;
来源：http://ve.colortex.cn

[Q65] 回滚事务
来源：http://cu.asd995.cn

ROLLBACK;
来源：http://uy.huanxung.cn

[Q66] 行锁查询
来源：http://ga.yuexingan06.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://xg.yuntaijiaju.cn

[Q67] 设置隔离级别
来源：http://ch.jianghongdianzi.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://li.huixiangedu.cn

[Q68] 保存点
来源：http://pb.newstarts.cn

SAVEPOINT sp1;
来源：http://la.yuntaijiaju.cn

ROLLBACK TO sp1;
来源：http://ek.jctech888.com.cn

[Q69] 查看执行计划
来源：http://tx.hnjuh.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wl.yuexingan06.cn

[Q70] 更新统计信息
来源：http://pp.haigaiapp.cn

ANALYZE TABLE users;
来源：http://zg.wgjwhj.cn

[Q71] 查看建表语句
来源：http://ee.gzmigu.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://lg.521024.cn

[Q72] 查看索引
来源：http://go.hnjuh.cn

SHOW INDEX FROM users;
来源：http://be.shtwfgs.cn

[Q73] 查看表状态
来源：http://hu.bjjhwx.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://ra.shxzukj.cn

[Q74] 强制使用索引
来源：http://av.jctech888.com.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://zs.yuexingan06.cn

[Q75] 日期格式化
来源：http://tc.panjiajie.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://jw.szxytkj.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ka.szsharing.cn

[Q76] 按天统计
来源：http://ii.gzmigu.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://od.chemitech.net.cn

[Q77] 时间加减
来源：http://wm.jianghongdianzi.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ct.9csxet.cn

[Q78] 当前时间
来源：http://xi.chemitech.net.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ai.szxytkj.cn

[Q79] 字符串拼接
来源：http://ke.wgjwhj.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ih.huixinmuqiang.cn

[Q80] 字符串截取
来源：http://zm.newstarts.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://kp.jianghongdianzi.cn

[Q81] 字符串替换
来源：http://id.shxzukj.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ic.haigaiapp.cn

[Q82] 字符长度与字节长度
来源：http://pj.panjiajie.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://fc.yuexingan06.cn

[Q83] 大小写转换
来源：http://ia.yuexingan06.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://kf.gzmigu.cn

[Q84] 去除首尾空格
来源：http://cv.bjjhwx.cn

SELECT TRIM(name) FROM users;
来源：http://fo.shxzskj.cn

[Q85] 数值取整
来源：http://nn.yuntaijiaju.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://tw.shxzukj.cn

[Q86] 读取 JSON 字段
来源：http://qq.panjiajie.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://br.haigaiapp.cn

[Q87] JSON 字段做条件
来源：http://xn.shtwfgs.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://pa.shxzskj.cn

[Q88] 行转列（条件聚合）
来源：http://wu.bjjhwx.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ly.colortex.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://fw.wgjwhj.cn

[Q89] 判断表是否存在
来源：http://sk.newstarts.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://da.jctech888.com.cn

[Q90] 生成序号列
来源：http://tl.haigaiapp.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://bg.yuntaijiaju.cn

================================================================================
来源：http://ao.chemitech.net.cn

R. Bash 专题
来源：http://oe.jianghongdianzi.cn

================================================================================
来源：http://sz.bookmarksfly.cn

[R01] shebang 与严格模式
来源：http://br.szxytkj.cn

#!/usr/bin/env bash
来源：http://ht.bookmarksfly.cn

set -euo pipefail
来源：http://gm.jctech888.com.cn

[R02] 变量赋值与使用
来源：http://ks.lnxyls.cn

name="Tom"; echo "$name"
来源：http://gq.muxihuayi.cn

[R03] 只读变量
来源：http://qw.newstarts.cn

readonly PI=3.14
来源：http://kv.yuntaijiaju.cn

[R04] 位置参数
来源：http://kb.gzmigu.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://gv.huanxung.cn

[R05] 参数默认值
来源：http://yt.jctech888.com.cn

name="${1:-default}"
来源：http://je.panjiajie.cn

[R06] 判断命令是否存在
来源：http://it.shxzskj.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://kp.huixiangedu.cn

[R07] if 判断文件
来源：http://gm.panjiajie.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://qn.colortex.cn

[R08] 数值比较
来源：http://sn.asd995.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://xm.shtwfgs.cn

[R09] 字符串比较
来源：http://xr.9csxet.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://aq.hnjuh.cn

[R10] 正则匹配
来源：http://uy.bjjhwx.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ej.521024.cn

[R11] case 多分支
来源：http://wn.gzmigu.cn

case "$1" in
来源：http://nh.szxytkj.cn

start) echo "启动" ;;
来源：http://bp.bookmarksfly.cn

stop)  echo "停止" ;;
来源：http://aq.shxzukj.cn

*)     echo "未知命令" ;;
来源：http://uu.shxzskj.cn

esac
来源：http://zc.huixinmuqiang.cn

[R12] for 遍历文件
来源：http://yx.szxytkj.cn

for f in *.txt; do echo "$f"; done
来源：http://hx.521024.cn

[R13] for 计数循环
来源：http://iq.chemitech.net.cn

for i in {1..10}; do echo "$i"; done
来源：http://jl.yuntaijiaju.cn

[R14] C 风格 for
来源：http://hm.szsharing.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://bn.hnjuh.cn

[R15] while 逐行读文件
来源：http://uk.yuntaijiaju.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://xz.nszjky.cn

[R16] until 等待条件
来源：http://qr.panjiajie.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mf.shxzukj.cn

[R17] 数组定义与取值
来源：http://uq.jctech888.com.cn

arr=(a b c); echo "${arr[0]}"
来源：http://rh.hahajie.cn

[R18] 遍历数组
来源：http://ct.huanxung.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ja.szxytkj.cn

[R19] 数组长度
来源：http://up.lnxyls.cn

echo "${#arr[@]}"
来源：http://rx.shxzukj.cn

[R20] 关联数组（字典）
来源：http://np.shtwfgs.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://es.haigaiapp.cn

[R21] 字符串长度
来源：http://gy.521024.cn

echo "${#s}"
来源：http://ux.jianghongdianzi.cn

[R22] 截取子串
来源：http://jk.lnxyls.cn

echo "${s:0:5}"
来源：http://yz.lnxyls.cn

[R23] 字符串替换
来源：http://bm.chemitech.net.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://vd.bookmarksfly.cn

[R24] 大小写转换
来源：http://qs.lnxyls.cn

echo "${s^^}"; echo "${s,,}"
来源：http://ux.szsharing.cn

[R25] 去后缀 / 去前缀
来源：http://cp.colortex.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://wg.colortex.cn

[R26] 命令替换
来源：http://zg.muxihuayi.cn

now=$(date +%F); echo "$now"
来源：http://om.shxzskj.cn

[R27] 算术展开
来源：http://wl.chemitech.net.cn

echo $((1 + 2 * 3))
来源：http://mn.colortex.cn

[R28] 浮点运算
来源：http://ds.yuntaijiaju.cn

echo "scale=2; 10/3" | bc
来源：http://zg.huixinmuqiang.cn

[R29] 定义函数
来源：http://ys.huixinmuqiang.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://pk.panjiajie.cn

[R30] 函数返回状态码
来源：http://yc.lnxyls.cn

f() { return 0; }; f || echo "失败了"
来源：http://ex.panjiajie.cn

[R31] 局部变量
来源：http://yi.lnxyls.cn

f() { local x=1; echo "$x"; }
来源：http://rp.colortex.cn

[R32] 参数个数校验
来源：http://bp.nszjky.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://rs.shxzukj.cn

[R33] 捕获错误并提示行号
来源：http://mj.521024.cn


<!-- 参考信息 -->