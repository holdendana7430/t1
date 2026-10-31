代发 wailian999

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://am.yuntaijiaju.cn

C#:   if (x is null) {}
来源：http://ho.newstarts.cn

[P07] 防抖与节流
来源：http://zz.newstarts.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://re.chemitech.net.cn

PHP:  // 手写时间戳比较
来源：http://mq.panjiajie.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ze.chemitech.net.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://bl.panjiajie.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://uj.chemitech.net.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://is.jctech888.com.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://bp.szsharing.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://fh.chemitech.net.cn

[P08] 处理浮点精度问题
来源：http://bx.hnjuh.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://nx.shxzskj.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://it.haigaiapp.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ku.haigaiapp.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://da.gzmigu.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ns.nszjky.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://dg.gzmigu.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ak.hahajie.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://cm.huanxung.cn

================================================================================
来源：http://ro.gzmigu.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://yt.szxytkj.cn

================================================================================
来源：http://no.shxzskj.cn

[Q01] 创建表
来源：http://cj.huixinmuqiang.cn

CREATE TABLE users (
来源：http://pz.9csxet.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://om.nszjky.cn

name VARCHAR(50) NOT NULL,
来源：http://xu.szxytkj.cn

email VARCHAR(100) UNIQUE,
来源：http://ss.bookmarksfly.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://jr.521024.cn

);
来源：http://wz.newstarts.cn

[Q02] 创建带外键的表
来源：http://gf.nicolike.cn

CREATE TABLE orders (
来源：http://oy.9csxet.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://xl.huixiangedu.cn

user_id INT NOT NULL,
来源：http://yk.nicolike.cn

amount DECIMAL(10, 2),
来源：http://kt.muxihuayi.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://by.bookmarksfly.cn

);
来源：http://xd.521024.cn

[Q03] 增加列
来源：http://az.haigaiapp.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://gh.gzmigu.cn

[Q04] 修改列类型
来源：http://ks.jianghongdianzi.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hn.szxytkj.cn

[Q05] 重命名列
来源：http://kk.wgjwhj.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mp.huanxung.cn

[Q06] 删除列
来源：http://kz.szxytkj.cn

ALTER TABLE users DROP COLUMN age;
来源：http://yt.jctech888.com.cn

[Q07] 删除表
来源：http://ee.wgjwhj.cn

DROP TABLE IF EXISTS orders;
来源：http://kf.nicolike.cn

[Q08] 创建普通索引
来源：http://dc.haigaiapp.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://pj.hnjuh.cn

[Q09] 创建唯一索引
来源：http://ub.hnjuh.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://tq.jianghongdianzi.cn

[Q10] 插入单行
来源：http://js.colortex.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://az.jianghongdianzi.cn

[Q11] 一次插入多行
来源：http://nu.szxytkj.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://iu.jctech888.com.cn

[Q12] 插入后取自增 ID
来源：http://il.9csxet.cn

INSERT INTO users (name) VALUES ('C');
来源：http://lc.yuntaijiaju.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://sg.asd995.cn

[Q13] 忽略重复插入
来源：http://sl.colortex.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://rf.hnjuh.cn

[Q14] 存在则更新（upsert）
来源：http://na.panjiajie.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hk.muxihuayi.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://kd.yuexingan06.cn

[Q15] 查询全部
来源：http://wq.hnjuh.cn

SELECT * FROM users;
来源：http://zi.jianghongdianzi.cn

[Q16] 查询指定列
来源：http://xp.huanxung.cn

SELECT id, name FROM users;
来源：http://mm.jianghongdianzi.cn

[Q17] 条件查询
来源：http://rg.haigaiapp.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://rl.9csxet.cn

[Q18] 模糊匹配
来源：http://eo.hahajie.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://yj.shxzskj.cn

[Q19] 范围查询
来源：http://ss.521024.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://yf.9csxet.cn

[Q20] IN 列表
来源：http://tf.jctech888.com.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wl.wgjwhj.cn

[Q21] 空值判断
来源：http://zm.9csxet.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://oa.bjjhwx.cn

[Q22] 排序
来源：http://tc.asd995.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://xt.hahajie.cn

[Q23] 分页
来源：http://os.szsharing.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://po.jianghongdianzi.cn

[Q24] 去重
来源：http://cv.hahajie.cn

SELECT DISTINCT city FROM users;
来源：http://yv.huixinmuqiang.cn

[Q25] 只取前 N 条
来源：http://bp.newstarts.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://po.wgjwhj.cn

[Q26] 计数
来源：http://td.jctech888.com.cn

SELECT COUNT(*) FROM users;
来源：http://do.bjjhwx.cn

[Q27] 条件计数
来源：http://iy.szsharing.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ru.chemitech.net.cn

[Q28] 求和与平均
来源：http://pm.haigaiapp.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://il.nicolike.cn

[Q29] 最大最小值
来源：http://aq.huanxung.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://gt.muxihuayi.cn

[Q30] 分组统计
来源：http://ad.panjiajie.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://tt.yuexingan06.cn

[Q31] 分组后过滤
来源：http://ge.9csxet.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ho.hnjuh.cn

[Q32] 分组拼接字符串
来源：http://ny.lnxyls.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://cl.shxzukj.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://vy.wgjwhj.cn

[Q33] 多列分组
来源：http://ge.wgjwhj.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hm.9csxet.cn

[Q34] 每组取第一条
来源：http://jx.wgjwhj.cn

SELECT * FROM (
来源：http://zt.yuexingan06.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://jh.chemitech.net.cn

) t WHERE rn = 1;
来源：http://zu.colortex.cn

[Q35] 内连接
来源：http://yw.huixiangedu.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://rw.nszjky.cn

[Q36] 左连接
来源：http://eg.gzmigu.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://sy.panjiajie.cn

[Q37] 右连接
来源：http://rz.shxzukj.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://gn.hnjuh.cn

[Q38] 全外连接（PostgreSQL）
来源：http://fo.newstarts.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://xl.hnjuh.cn

[Q39] 自连接（查上下级）
来源：http://os.521024.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://hh.bjjhwx.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ni.shxzukj.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://xg.521024.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wu.nicolike.cn

[Q41] 多表连接
来源：http://xh.asd995.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://lp.hnjuh.cn

JOIN users u ON u.id = o.user_id
来源：http://vm.huixinmuqiang.cn

JOIN products p ON p.id = o.product_id;
来源：http://sj.chemitech.net.cn

[Q42] 连接条件附加过滤
来源：http://em.nicolike.cn

SELECT u.name, o.amount FROM users u
来源：http://fe.wgjwhj.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://bi.yuntaijiaju.cn

[Q43] 标量子查询
来源：http://hh.szxytkj.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://yx.szxytkj.cn

[Q44] IN 子查询
来源：http://cx.shtwfgs.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ia.wgjwhj.cn

[Q45] EXISTS 判断存在
来源：http://qo.jianghongdianzi.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://zq.muxihuayi.cn

[Q46] NOT EXISTS 判断不存在
来源：http://sa.jianghongdianzi.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://nu.yuntaijiaju.cn

[Q47] 与平均值比较
来源：http://kx.shxzukj.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://tx.shxzukj.cn

[Q48] CTE 公用表表达式
来源：http://ge.hnjuh.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://xg.hnjuh.cn

SELECT * FROM t WHERE c > 5;
来源：http://kw.jctech888.com.cn

[Q49] 更新单行
来源：http://qk.bjjhwx.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wf.yuntaijiaju.cn

[Q50] 批量更新
来源：http://om.yuexingan06.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://nu.yuexingan06.cn

[Q51] 用子查询更新
来源：http://hd.9csxet.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://qk.hahajie.cn

[Q52] 删除指定行
来源：http://ra.asd995.cn

DELETE FROM users WHERE id = 10;
来源：http://fl.asd995.cn

[Q53] 按条件删除
来源：http://nk.huixinmuqiang.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://im.muxihuayi.cn

[Q54] 清空表
来源：http://qg.hahajie.cn

TRUNCATE TABLE logs;
来源：http://rx.nicolike.cn

[Q55] 排名（并列占位）
来源：http://dn.huixiangedu.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://vx.wgjwhj.cn

[Q56] 密集排名（并列不占位）
来源：http://mc.huixinmuqiang.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://kq.haigaiapp.cn

[Q57] 行号
来源：http://gt.huixinmuqiang.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://qc.colortex.cn

[Q58] 累计求和
来源：http://sg.9csxet.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://tm.szxytkj.cn

[Q59] 分组内累计
来源：http://xn.huixinmuqiang.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://bw.chemitech.net.cn

[Q60] 取上一行 / 下一行
来源：http://ux.wgjwhj.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wn.521024.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://vv.newstarts.cn

[Q61] 移动平均
来源：http://wp.bookmarksfly.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://tw.asd995.cn

[Q62] 分组占比
来源：http://bj.huanxung.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://gr.szxytkj.cn

[Q63] 开启事务
来源：http://wd.jctech888.com.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://bc.nicolike.cn

[Q64] 提交事务
来源：http://tj.9csxet.cn

COMMIT;
来源：http://xg.521024.cn

[Q65] 回滚事务
来源：http://wt.shxzskj.cn

ROLLBACK;
来源：http://ii.huanxung.cn

[Q66] 行锁查询
来源：http://so.panjiajie.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://qy.newstarts.cn

[Q67] 设置隔离级别
来源：http://yb.muxihuayi.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://xh.bookmarksfly.cn

[Q68] 保存点
来源：http://yj.yuexingan06.cn

SAVEPOINT sp1;
来源：http://mx.hnjuh.cn

ROLLBACK TO sp1;
来源：http://lq.521024.cn

[Q69] 查看执行计划
来源：http://to.chemitech.net.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://qb.chemitech.net.cn

[Q70] 更新统计信息
来源：http://sm.wgjwhj.cn

ANALYZE TABLE users;
来源：http://ea.szsharing.cn

[Q71] 查看建表语句
来源：http://xg.wgjwhj.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://uu.lnxyls.cn

[Q72] 查看索引
来源：http://mw.shxzskj.cn

SHOW INDEX FROM users;
来源：http://xo.huixinmuqiang.cn

[Q73] 查看表状态
来源：http://wz.shxzukj.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://rp.bjjhwx.cn

[Q74] 强制使用索引
来源：http://mq.szsharing.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wy.wgjwhj.cn

[Q75] 日期格式化
来源：http://cm.panjiajie.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://fq.nszjky.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://tn.gzmigu.cn

[Q76] 按天统计
来源：http://vk.yuntaijiaju.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wg.szsharing.cn

[Q77] 时间加减
来源：http://yx.nszjky.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://fy.muxihuayi.cn

[Q78] 当前时间
来源：http://ws.szsharing.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://sl.521024.cn

[Q79] 字符串拼接
来源：http://ni.szxytkj.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://sb.jctech888.com.cn

[Q80] 字符串截取
来源：http://eu.huixinmuqiang.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ei.521024.cn

[Q81] 字符串替换
来源：http://uz.haigaiapp.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://lc.jianghongdianzi.cn

[Q82] 字符长度与字节长度
来源：http://ve.asd995.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://qw.shxzskj.cn

[Q83] 大小写转换
来源：http://ja.haigaiapp.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hu.yuntaijiaju.cn

[Q84] 去除首尾空格
来源：http://au.shxzukj.cn

SELECT TRIM(name) FROM users;
来源：http://hx.newstarts.cn

[Q85] 数值取整
来源：http://pb.yuexingan06.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://jb.szsharing.cn

[Q86] 读取 JSON 字段
来源：http://ob.yuntaijiaju.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ip.jctech888.com.cn

[Q87] JSON 字段做条件
来源：http://tv.colortex.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ae.wgjwhj.cn

[Q88] 行转列（条件聚合）
来源：http://rf.colortex.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://xf.jctech888.com.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://cs.shxzskj.cn

[Q89] 判断表是否存在
来源：http://qc.shxzukj.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://cd.gzmigu.cn

[Q90] 生成序号列
来源：http://cs.nicolike.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://dj.jianghongdianzi.cn

================================================================================
来源：http://so.hnjuh.cn

R. Bash 专题
来源：http://ut.bjjhwx.cn

================================================================================
来源：http://cx.nszjky.cn

[R01] shebang 与严格模式
来源：http://lq.jctech888.com.cn

#!/usr/bin/env bash
来源：http://xq.yuntaijiaju.cn

set -euo pipefail
来源：http://km.gzmigu.cn

[R02] 变量赋值与使用
来源：http://yg.shxzskj.cn

name="Tom"; echo "$name"
来源：http://wh.szxytkj.cn

[R03] 只读变量
来源：http://yi.shxzskj.cn

readonly PI=3.14
来源：http://ct.gzmigu.cn

[R04] 位置参数
来源：http://hn.szxytkj.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://un.gzmigu.cn

[R05] 参数默认值
来源：http://gl.hahajie.cn

name="${1:-default}"
来源：http://eg.shxzskj.cn

[R06] 判断命令是否存在
来源：http://hy.nicolike.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://po.muxihuayi.cn

[R07] if 判断文件
来源：http://kl.nicolike.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://lz.lnxyls.cn

[R08] 数值比较
来源：http://hz.9csxet.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://qi.huanxung.cn

[R09] 字符串比较
来源：http://lv.huixinmuqiang.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://nc.nicolike.cn

[R10] 正则匹配
来源：http://sm.colortex.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://zt.shxzukj.cn

[R11] case 多分支
来源：http://vv.lnxyls.cn

case "$1" in
来源：http://rz.nszjky.cn

start) echo "启动" ;;
来源：http://ja.jctech888.com.cn

stop)  echo "停止" ;;
来源：http://at.yuntaijiaju.cn

*)     echo "未知命令" ;;
来源：http://wf.haigaiapp.cn

esac
来源：http://hb.szxytkj.cn

[R12] for 遍历文件
来源：http://rd.asd995.cn

for f in *.txt; do echo "$f"; done
来源：http://eq.gzmigu.cn

[R13] for 计数循环
来源：http://bs.muxihuayi.cn

for i in {1..10}; do echo "$i"; done
来源：http://iy.huixinmuqiang.cn

[R14] C 风格 for
来源：http://wg.nszjky.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://qb.nicolike.cn

[R15] while 逐行读文件
来源：http://hf.wgjwhj.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ke.jianghongdianzi.cn

[R16] until 等待条件
来源：http://rb.colortex.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://iq.haigaiapp.cn

[R17] 数组定义与取值
来源：http://jd.asd995.cn

arr=(a b c); echo "${arr[0]}"
来源：http://qw.shtwfgs.cn

[R18] 遍历数组
来源：http://ko.panjiajie.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://kz.wgjwhj.cn

[R19] 数组长度
来源：http://nv.newstarts.cn

echo "${#arr[@]}"
来源：http://ka.shxzukj.cn

[R20] 关联数组（字典）
来源：http://rn.wgjwhj.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://nm.newstarts.cn

[R21] 字符串长度
来源：http://zp.panjiajie.cn

echo "${#s}"
来源：http://gh.hahajie.cn

[R22] 截取子串
来源：http://kq.jianghongdianzi.cn

echo "${s:0:5}"
来源：http://dl.lnxyls.cn

[R23] 字符串替换
来源：http://ap.yuntaijiaju.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://gd.nicolike.cn

[R24] 大小写转换
来源：http://wb.hahajie.cn

echo "${s^^}"; echo "${s,,}"
来源：http://sk.lnxyls.cn

[R25] 去后缀 / 去前缀
来源：http://rf.huanxung.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://ae.lnxyls.cn

[R26] 命令替换
来源：http://ti.9csxet.cn

now=$(date +%F); echo "$now"
来源：http://nt.521024.cn

[R27] 算术展开
来源：http://kk.haigaiapp.cn

echo $((1 + 2 * 3))
来源：http://hl.521024.cn

[R28] 浮点运算
来源：http://aj.szxytkj.cn

echo "scale=2; 10/3" | bc
来源：http://la.hahajie.cn

[R29] 定义函数
来源：http://al.bookmarksfly.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://gk.yuexingan06.cn

[R30] 函数返回状态码
来源：http://mj.chemitech.net.cn

f() { return 0; }; f || echo "失败了"
来源：http://aw.hahajie.cn

[R31] 局部变量
来源：http://ge.jctech888.com.cn

f() { local x=1; echo "$x"; }
来源：http://lg.nszjky.cn

[R32] 参数个数校验
来源：http://hp.shxzukj.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://zq.nicolike.cn

[R33] 捕获错误并提示行号
来源：http://dc.hahajie.cn


<!-- 参考信息 -->