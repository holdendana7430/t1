代发 wailian999

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hp.hahajie.cn

TS:   if (x == null) {}
来源：http://xh.yuntaijiaju.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://tn.panjiajie.cn

Go:   if x == nil {}
来源：http://tq.yuntaijiaju.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.colortex.cn

C#:   if (x is null) {}
来源：http://eb.jianghongdianzi.cn

[P07] 防抖与节流
来源：http://ab.szxytkj.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://tl.muxihuayi.cn

PHP:  // 手写时间戳比较
来源：http://ok.haigaiapp.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://vi.szxytkj.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qs.asd995.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wz.chemitech.net.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ey.yuntaijiaju.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://sz.huanxung.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://rc.huixinmuqiang.cn

[P08] 处理浮点精度问题
来源：http://vd.wgjwhj.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ll.szsharing.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://md.521024.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://yf.hnjuh.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://uf.szsharing.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://lz.panjiajie.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://jg.szxytkj.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://cm.hnjuh.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://gb.jianghongdianzi.cn

================================================================================
来源：http://xe.colortex.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://vu.chemitech.net.cn

================================================================================
来源：http://tq.shxzukj.cn

[Q01] 创建表
来源：http://yc.asd995.cn

CREATE TABLE users (
来源：http://yx.asd995.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ib.yuntaijiaju.cn

name VARCHAR(50) NOT NULL,
来源：http://br.lnxyls.cn

email VARCHAR(100) UNIQUE,
来源：http://ck.huixinmuqiang.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ae.bookmarksfly.cn

);
来源：http://ud.panjiajie.cn

[Q02] 创建带外键的表
来源：http://ps.asd995.cn

CREATE TABLE orders (
来源：http://ab.nszjky.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://lv.wgjwhj.cn

user_id INT NOT NULL,
来源：http://bw.haigaiapp.cn

amount DECIMAL(10, 2),
来源：http://md.szxytkj.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wn.huanxung.cn

);
来源：http://mn.huanxung.cn

[Q03] 增加列
来源：http://em.haigaiapp.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://dt.nicolike.cn

[Q04] 修改列类型
来源：http://ov.asd995.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://yx.bookmarksfly.cn

[Q05] 重命名列
来源：http://tn.newstarts.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://gf.nicolike.cn

[Q06] 删除列
来源：http://ei.szsharing.cn

ALTER TABLE users DROP COLUMN age;
来源：http://qg.asd995.cn

[Q07] 删除表
来源：http://ok.hahajie.cn

DROP TABLE IF EXISTS orders;
来源：http://mk.yuntaijiaju.cn

[Q08] 创建普通索引
来源：http://vv.jianghongdianzi.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://xh.nicolike.cn

[Q09] 创建唯一索引
来源：http://xs.lnxyls.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://pk.newstarts.cn

[Q10] 插入单行
来源：http://hn.nicolike.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://kb.bookmarksfly.cn

[Q11] 一次插入多行
来源：http://nj.huixiangedu.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mf.panjiajie.cn

[Q12] 插入后取自增 ID
来源：http://aw.shxzukj.cn

INSERT INTO users (name) VALUES ('C');
来源：http://oa.9csxet.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://sh.shxzukj.cn

[Q13] 忽略重复插入
来源：http://vf.lnxyls.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://vn.yuntaijiaju.cn

[Q14] 存在则更新（upsert）
来源：http://eh.9csxet.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wc.gzmigu.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://bj.muxihuayi.cn

[Q15] 查询全部
来源：http://ri.colortex.cn

SELECT * FROM users;
来源：http://pw.9csxet.cn

[Q16] 查询指定列
来源：http://gh.szxytkj.cn

SELECT id, name FROM users;
来源：http://zi.huixinmuqiang.cn

[Q17] 条件查询
来源：http://dc.huixiangedu.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://kn.bookmarksfly.cn

[Q18] 模糊匹配
来源：http://zy.szxytkj.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ef.jctech888.com.cn

[Q19] 范围查询
来源：http://jl.jctech888.com.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ur.shxzukj.cn

[Q20] IN 列表
来源：http://cm.lnxyls.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://oy.nszjky.cn

[Q21] 空值判断
来源：http://oe.chemitech.net.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://qv.shxzskj.cn

[Q22] 排序
来源：http://gh.wgjwhj.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://sp.huanxung.cn

[Q23] 分页
来源：http://wz.szsharing.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ft.jianghongdianzi.cn

[Q24] 去重
来源：http://ox.huixinmuqiang.cn

SELECT DISTINCT city FROM users;
来源：http://kn.huixiangedu.cn

[Q25] 只取前 N 条
来源：http://lz.newstarts.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://jb.huixinmuqiang.cn

[Q26] 计数
来源：http://hu.hahajie.cn

SELECT COUNT(*) FROM users;
来源：http://ol.huixiangedu.cn

[Q27] 条件计数
来源：http://ib.nicolike.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://or.yuexingan06.cn

[Q28] 求和与平均
来源：http://tu.jctech888.com.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://dg.huanxung.cn

[Q29] 最大最小值
来源：http://pj.asd995.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://lq.huixiangedu.cn

[Q30] 分组统计
来源：http://fr.shxzskj.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://bl.nszjky.cn

[Q31] 分组后过滤
来源：http://io.szsharing.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://sq.newstarts.cn

[Q32] 分组拼接字符串
来源：http://cu.chemitech.net.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://gr.jianghongdianzi.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://le.huixinmuqiang.cn

[Q33] 多列分组
来源：http://go.huanxung.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://kv.asd995.cn

[Q34] 每组取第一条
来源：http://nl.hahajie.cn

SELECT * FROM (
来源：http://pi.jctech888.com.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://zs.521024.cn

) t WHERE rn = 1;
来源：http://gr.colortex.cn

[Q35] 内连接
来源：http://yk.shxzskj.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://br.nszjky.cn

[Q36] 左连接
来源：http://yn.muxihuayi.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://nh.huixinmuqiang.cn

[Q37] 右连接
来源：http://hl.wgjwhj.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://jt.gzmigu.cn

[Q38] 全外连接（PostgreSQL）
来源：http://dt.chemitech.net.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ad.chemitech.net.cn

[Q39] 自连接（查上下级）
来源：http://qk.szxytkj.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://sw.newstarts.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://sy.gzmigu.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://vc.hnjuh.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://rw.hahajie.cn

[Q41] 多表连接
来源：http://gq.nicolike.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://ot.shxzskj.cn

JOIN users u ON u.id = o.user_id
来源：http://us.asd995.cn

JOIN products p ON p.id = o.product_id;
来源：http://ws.wgjwhj.cn

[Q42] 连接条件附加过滤
来源：http://ya.bookmarksfly.cn

SELECT u.name, o.amount FROM users u
来源：http://gd.9csxet.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://km.jianghongdianzi.cn

[Q43] 标量子查询
来源：http://sn.jctech888.com.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://yo.hahajie.cn

[Q44] IN 子查询
来源：http://xp.wgjwhj.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://dk.chemitech.net.cn

[Q45] EXISTS 判断存在
来源：http://rt.shtwfgs.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ji.bjjhwx.cn

[Q46] NOT EXISTS 判断不存在
来源：http://hq.colortex.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://do.jctech888.com.cn

[Q47] 与平均值比较
来源：http://ji.hnjuh.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hg.521024.cn

[Q48] CTE 公用表表达式
来源：http://nj.szsharing.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://fi.colortex.cn

SELECT * FROM t WHERE c > 5;
来源：http://qs.haigaiapp.cn

[Q49] 更新单行
来源：http://do.huanxung.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://cb.bookmarksfly.cn

[Q50] 批量更新
来源：http://ki.shxzukj.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://gs.521024.cn

[Q51] 用子查询更新
来源：http://aq.chemitech.net.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://qg.jctech888.com.cn

[Q52] 删除指定行
来源：http://lx.panjiajie.cn

DELETE FROM users WHERE id = 10;
来源：http://cf.wgjwhj.cn

[Q53] 按条件删除
来源：http://en.hnjuh.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ki.panjiajie.cn

[Q54] 清空表
来源：http://cx.jianghongdianzi.cn

TRUNCATE TABLE logs;
来源：http://xf.huanxung.cn

[Q55] 排名（并列占位）
来源：http://cx.shxzskj.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://sp.521024.cn

[Q56] 密集排名（并列不占位）
来源：http://uj.huanxung.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mq.wgjwhj.cn

[Q57] 行号
来源：http://hr.nszjky.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ki.yuexingan06.cn

[Q58] 累计求和
来源：http://vi.huixinmuqiang.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://up.huixiangedu.cn

[Q59] 分组内累计
来源：http://jk.huixinmuqiang.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://oh.bjjhwx.cn

[Q60] 取上一行 / 下一行
来源：http://re.shxzskj.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hw.9csxet.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://gw.chemitech.net.cn

[Q61] 移动平均
来源：http://lp.nicolike.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://oa.nszjky.cn

[Q62] 分组占比
来源：http://fg.chemitech.net.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://bq.chemitech.net.cn

[Q63] 开启事务
来源：http://kl.szsharing.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://su.panjiajie.cn

[Q64] 提交事务
来源：http://ia.jctech888.com.cn

COMMIT;
来源：http://zx.yuexingan06.cn

[Q65] 回滚事务
来源：http://fe.bjjhwx.cn

ROLLBACK;
来源：http://pm.haigaiapp.cn

[Q66] 行锁查询
来源：http://be.asd995.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://cy.szxytkj.cn

[Q67] 设置隔离级别
来源：http://lt.521024.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mb.huixiangedu.cn

[Q68] 保存点
来源：http://fi.shtwfgs.cn

SAVEPOINT sp1;
来源：http://jw.huixinmuqiang.cn

ROLLBACK TO sp1;
来源：http://pa.9csxet.cn

[Q69] 查看执行计划
来源：http://zs.nszjky.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://je.panjiajie.cn

[Q70] 更新统计信息
来源：http://bw.nicolike.cn

ANALYZE TABLE users;
来源：http://fw.gzmigu.cn

[Q71] 查看建表语句
来源：http://ov.szsharing.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://eo.shxzukj.cn

[Q72] 查看索引
来源：http://hm.panjiajie.cn

SHOW INDEX FROM users;
来源：http://ay.szsharing.cn

[Q73] 查看表状态
来源：http://yc.wgjwhj.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://ws.yuexingan06.cn

[Q74] 强制使用索引
来源：http://yr.panjiajie.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://sh.yuexingan06.cn

[Q75] 日期格式化
来源：http://oi.asd995.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://cs.newstarts.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ae.huanxung.cn

[Q76] 按天统计
来源：http://nc.haigaiapp.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://em.gzmigu.cn

[Q77] 时间加减
来源：http://hr.lnxyls.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://gj.shtwfgs.cn

[Q78] 当前时间
来源：http://od.521024.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ql.yuntaijiaju.cn

[Q79] 字符串拼接
来源：http://bt.muxihuayi.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://gf.bjjhwx.cn

[Q80] 字符串截取
来源：http://em.panjiajie.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://qw.shxzskj.cn

[Q81] 字符串替换
来源：http://pd.haigaiapp.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://pc.hahajie.cn

[Q82] 字符长度与字节长度
来源：http://lz.huanxung.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://dw.huixinmuqiang.cn

[Q83] 大小写转换
来源：http://nf.colortex.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ud.szxytkj.cn

[Q84] 去除首尾空格
来源：http://uq.nicolike.cn

SELECT TRIM(name) FROM users;
来源：http://ml.nszjky.cn

[Q85] 数值取整
来源：http://pu.521024.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://gr.panjiajie.cn

[Q86] 读取 JSON 字段
来源：http://eq.bookmarksfly.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://li.panjiajie.cn

[Q87] JSON 字段做条件
来源：http://jz.huixiangedu.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://la.lnxyls.cn

[Q88] 行转列（条件聚合）
来源：http://hp.nicolike.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wf.9csxet.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ig.nicolike.cn

[Q89] 判断表是否存在
来源：http://fh.jctech888.com.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://tw.521024.cn

[Q90] 生成序号列
来源：http://qv.gzmigu.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ly.jianghongdianzi.cn

================================================================================
来源：http://dh.shxzskj.cn

R. Bash 专题
来源：http://nc.lnxyls.cn

================================================================================
来源：http://lu.yuntaijiaju.cn

[R01] shebang 与严格模式
来源：http://qo.521024.cn

#!/usr/bin/env bash
来源：http://er.shtwfgs.cn

set -euo pipefail
来源：http://zq.jctech888.com.cn

[R02] 变量赋值与使用
来源：http://qo.gzmigu.cn

name="Tom"; echo "$name"
来源：http://az.huixinmuqiang.cn

[R03] 只读变量
来源：http://li.chemitech.net.cn

readonly PI=3.14
来源：http://un.9csxet.cn

[R04] 位置参数
来源：http://vg.haigaiapp.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hl.shtwfgs.cn

[R05] 参数默认值
来源：http://lq.chemitech.net.cn

name="${1:-default}"
来源：http://qq.haigaiapp.cn

[R06] 判断命令是否存在
来源：http://yo.hnjuh.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://yx.haigaiapp.cn

[R07] if 判断文件
来源：http://jc.shxzskj.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://rg.szxytkj.cn

[R08] 数值比较
来源：http://rs.szxytkj.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://lz.wgjwhj.cn

[R09] 字符串比较
来源：http://ki.shtwfgs.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://rg.haigaiapp.cn

[R10] 正则匹配
来源：http://fw.huanxung.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ct.hahajie.cn

[R11] case 多分支
来源：http://xd.huixiangedu.cn

case "$1" in
来源：http://mq.hnjuh.cn

start) echo "启动" ;;
来源：http://lx.szxytkj.cn

stop)  echo "停止" ;;
来源：http://fj.haigaiapp.cn

*)     echo "未知命令" ;;
来源：http://ur.szsharing.cn

esac
来源：http://yx.newstarts.cn

[R12] for 遍历文件
来源：http://fz.haigaiapp.cn

for f in *.txt; do echo "$f"; done
来源：http://yi.hahajie.cn

[R13] for 计数循环
来源：http://qo.yuexingan06.cn

for i in {1..10}; do echo "$i"; done
来源：http://st.muxihuayi.cn

[R14] C 风格 for
来源：http://dt.muxihuayi.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://pr.yuntaijiaju.cn

[R15] while 逐行读文件
来源：http://aj.haigaiapp.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ks.lnxyls.cn

[R16] until 等待条件
来源：http://kr.chemitech.net.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hn.huixinmuqiang.cn

[R17] 数组定义与取值
来源：http://uc.shxzskj.cn

arr=(a b c); echo "${arr[0]}"
来源：http://cc.nszjky.cn

[R18] 遍历数组
来源：http://to.muxihuayi.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://kn.521024.cn

[R19] 数组长度
来源：http://kq.shtwfgs.cn

echo "${#arr[@]}"
来源：http://lb.szsharing.cn

[R20] 关联数组（字典）
来源：http://dw.panjiajie.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mx.szsharing.cn

[R21] 字符串长度
来源：http://uv.asd995.cn

echo "${#s}"
来源：http://tu.asd995.cn

[R22] 截取子串
来源：http://sl.nicolike.cn

echo "${s:0:5}"
来源：http://ms.shxzskj.cn

[R23] 字符串替换
来源：http://dg.jctech888.com.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://cj.huanxung.cn

[R24] 大小写转换
来源：http://tq.huixinmuqiang.cn

echo "${s^^}"; echo "${s,,}"
来源：http://sb.newstarts.cn

[R25] 去后缀 / 去前缀
来源：http://jy.hahajie.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://nb.bjjhwx.cn

[R26] 命令替换
来源：http://uz.gzmigu.cn

now=$(date +%F); echo "$now"
来源：http://wb.huixinmuqiang.cn

[R27] 算术展开
来源：http://jo.huixiangedu.cn

echo $((1 + 2 * 3))
来源：http://ta.521024.cn

[R28] 浮点运算
来源：http://lp.lnxyls.cn

echo "scale=2; 10/3" | bc
来源：http://ox.yuntaijiaju.cn

[R29] 定义函数
来源：http://dw.hahajie.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://we.shtwfgs.cn

[R30] 函数返回状态码
来源：http://kc.bjjhwx.cn

f() { return 0; }; f || echo "失败了"
来源：http://lb.yuntaijiaju.cn

[R31] 局部变量
来源：http://dm.shtwfgs.cn


<!-- 参考信息 -->