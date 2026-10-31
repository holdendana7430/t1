代发 wailian999

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ew.bookmarksfly.cn

C#:   if (x is null) {}
来源：http://iz.nicolike.cn

[P07] 防抖与节流
来源：http://tk.colortex.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://zc.huixinmuqiang.cn

PHP:  // 手写时间戳比较
来源：http://sj.yuntaijiaju.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ue.nicolike.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://er.muxihuayi.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://nr.haigaiapp.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hd.yuexingan06.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://ot.shxzskj.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://sb.gzmigu.cn

[P08] 处理浮点精度问题
来源：http://wa.9csxet.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ng.chemitech.net.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://nc.jianghongdianzi.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://bi.hahajie.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://qk.shtwfgs.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ba.wgjwhj.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ry.colortex.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://je.hahajie.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ta.hnjuh.cn

================================================================================
来源：http://hn.szxytkj.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://qw.shxzukj.cn

================================================================================
来源：http://nl.shxzskj.cn

[Q01] 创建表
来源：http://dh.shxzukj.cn

CREATE TABLE users (
来源：http://qn.yuntaijiaju.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://qh.wgjwhj.cn

name VARCHAR(50) NOT NULL,
来源：http://xs.521024.cn

email VARCHAR(100) UNIQUE,
来源：http://tt.9csxet.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://uy.hnjuh.cn

);
来源：http://qz.panjiajie.cn

[Q02] 创建带外键的表
来源：http://jk.colortex.cn

CREATE TABLE orders (
来源：http://qc.lnxyls.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://vm.bookmarksfly.cn

user_id INT NOT NULL,
来源：http://ur.huixinmuqiang.cn

amount DECIMAL(10, 2),
来源：http://fg.shxzskj.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ke.hahajie.cn

);
来源：http://ko.nszjky.cn

[Q03] 增加列
来源：http://of.lnxyls.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://bs.wgjwhj.cn

[Q04] 修改列类型
来源：http://gg.huixiangedu.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://tc.szxytkj.cn

[Q05] 重命名列
来源：http://mw.521024.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://lx.panjiajie.cn

[Q06] 删除列
来源：http://ei.szsharing.cn

ALTER TABLE users DROP COLUMN age;
来源：http://aa.colortex.cn

[Q07] 删除表
来源：http://tz.colortex.cn

DROP TABLE IF EXISTS orders;
来源：http://gm.nicolike.cn

[Q08] 创建普通索引
来源：http://aj.szsharing.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://db.lnxyls.cn

[Q09] 创建唯一索引
来源：http://ct.nicolike.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://dr.wgjwhj.cn

[Q10] 插入单行
来源：http://od.nszjky.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://sl.hnjuh.cn

[Q11] 一次插入多行
来源：http://ie.szsharing.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://rg.9csxet.cn

[Q12] 插入后取自增 ID
来源：http://bt.shxzskj.cn

INSERT INTO users (name) VALUES ('C');
来源：http://uo.colortex.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://su.jctech888.com.cn

[Q13] 忽略重复插入
来源：http://sn.newstarts.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://aj.521024.cn

[Q14] 存在则更新（upsert）
来源：http://et.gzmigu.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ag.huanxung.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ok.jianghongdianzi.cn

[Q15] 查询全部
来源：http://er.muxihuayi.cn

SELECT * FROM users;
来源：http://or.nicolike.cn

[Q16] 查询指定列
来源：http://lp.shtwfgs.cn

SELECT id, name FROM users;
来源：http://wm.huixiangedu.cn

[Q17] 条件查询
来源：http://yj.521024.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mu.jianghongdianzi.cn

[Q18] 模糊匹配
来源：http://hy.yuexingan06.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://yn.yuexingan06.cn

[Q19] 范围查询
来源：http://ht.shxzskj.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://is.bookmarksfly.cn

[Q20] IN 列表
来源：http://fn.shxzukj.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://zt.hahajie.cn

[Q21] 空值判断
来源：http://wp.nicolike.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://sb.szxytkj.cn

[Q22] 排序
来源：http://ck.nicolike.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://bf.9csxet.cn

[Q23] 分页
来源：http://vl.shxzskj.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://fp.chemitech.net.cn

[Q24] 去重
来源：http://iv.bookmarksfly.cn

SELECT DISTINCT city FROM users;
来源：http://mg.hahajie.cn

[Q25] 只取前 N 条
来源：http://ik.nicolike.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://cb.jctech888.com.cn

[Q26] 计数
来源：http://kx.nszjky.cn

SELECT COUNT(*) FROM users;
来源：http://iv.panjiajie.cn

[Q27] 条件计数
来源：http://sx.hnjuh.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://uw.huixiangedu.cn

[Q28] 求和与平均
来源：http://na.huixinmuqiang.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://ab.muxihuayi.cn

[Q29] 最大最小值
来源：http://ao.huixiangedu.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://sz.szxytkj.cn

[Q30] 分组统计
来源：http://ux.huixinmuqiang.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ik.muxihuayi.cn

[Q31] 分组后过滤
来源：http://ev.huixiangedu.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wm.nicolike.cn

[Q32] 分组拼接字符串
来源：http://yu.yuntaijiaju.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://lc.colortex.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://bu.shxzskj.cn

[Q33] 多列分组
来源：http://fg.shxzukj.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://xl.huanxung.cn

[Q34] 每组取第一条
来源：http://sq.chemitech.net.cn

SELECT * FROM (
来源：http://fq.muxihuayi.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://lc.nicolike.cn

) t WHERE rn = 1;
来源：http://ff.9csxet.cn

[Q35] 内连接
来源：http://ri.jctech888.com.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://fw.9csxet.cn

[Q36] 左连接
来源：http://wr.bookmarksfly.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ds.szxytkj.cn

[Q37] 右连接
来源：http://fc.huixinmuqiang.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ir.bjjhwx.cn

[Q38] 全外连接（PostgreSQL）
来源：http://mg.szsharing.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hy.shxzukj.cn

[Q39] 自连接（查上下级）
来源：http://qc.lnxyls.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://vj.shxzukj.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://iz.huixiangedu.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://xc.yuexingan06.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://og.lnxyls.cn

[Q41] 多表连接
来源：http://bj.haigaiapp.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://yq.bookmarksfly.cn

JOIN users u ON u.id = o.user_id
来源：http://cq.9csxet.cn

JOIN products p ON p.id = o.product_id;
来源：http://jx.lnxyls.cn

[Q42] 连接条件附加过滤
来源：http://ye.nszjky.cn

SELECT u.name, o.amount FROM users u
来源：http://kn.shxzskj.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://rh.yuexingan06.cn

[Q43] 标量子查询
来源：http://wz.jctech888.com.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://bs.muxihuayi.cn

[Q44] IN 子查询
来源：http://wg.muxihuayi.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ou.gzmigu.cn

[Q45] EXISTS 判断存在
来源：http://hj.bookmarksfly.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://jj.muxihuayi.cn

[Q46] NOT EXISTS 判断不存在
来源：http://gw.huixiangedu.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://sl.chemitech.net.cn

[Q47] 与平均值比较
来源：http://ln.haigaiapp.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://xi.huanxung.cn

[Q48] CTE 公用表表达式
来源：http://tl.huixinmuqiang.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ji.szsharing.cn

SELECT * FROM t WHERE c > 5;
来源：http://ee.hahajie.cn

[Q49] 更新单行
来源：http://gx.szxytkj.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.nszjky.cn

[Q50] 批量更新
来源：http://di.bjjhwx.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://de.521024.cn

[Q51] 用子查询更新
来源：http://ik.lnxyls.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://xn.bjjhwx.cn

[Q52] 删除指定行
来源：http://rg.huixinmuqiang.cn

DELETE FROM users WHERE id = 10;
来源：http://ex.huixinmuqiang.cn

[Q53] 按条件删除
来源：http://zf.lnxyls.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ox.chemitech.net.cn

[Q54] 清空表
来源：http://lt.nszjky.cn

TRUNCATE TABLE logs;
来源：http://rr.shxzukj.cn

[Q55] 排名（并列占位）
来源：http://we.521024.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://qe.newstarts.cn

[Q56] 密集排名（并列不占位）
来源：http://dc.huixinmuqiang.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hv.shxzskj.cn

[Q57] 行号
来源：http://bj.yuexingan06.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mc.jianghongdianzi.cn

[Q58] 累计求和
来源：http://rw.colortex.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://js.chemitech.net.cn

[Q59] 分组内累计
来源：http://bk.yuexingan06.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://kh.gzmigu.cn

[Q60] 取上一行 / 下一行
来源：http://fa.szsharing.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://lt.huanxung.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://rd.jctech888.com.cn

[Q61] 移动平均
来源：http://xg.hahajie.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://sh.shxzukj.cn

[Q62] 分组占比
来源：http://cd.yuntaijiaju.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wy.huanxung.cn

[Q63] 开启事务
来源：http://mq.shxzskj.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://dq.wgjwhj.cn

[Q64] 提交事务
来源：http://am.bookmarksfly.cn

COMMIT;
来源：http://le.hahajie.cn

[Q65] 回滚事务
来源：http://nv.9csxet.cn

ROLLBACK;
来源：http://rs.lnxyls.cn

[Q66] 行锁查询
来源：http://ul.huixiangedu.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://vj.nszjky.cn

[Q67] 设置隔离级别
来源：http://ay.9csxet.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://cy.chemitech.net.cn

[Q68] 保存点
来源：http://kr.jctech888.com.cn

SAVEPOINT sp1;
来源：http://cv.szsharing.cn

ROLLBACK TO sp1;
来源：http://zv.huixiangedu.cn

[Q69] 查看执行计划
来源：http://cp.bjjhwx.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://qg.hnjuh.cn

[Q70] 更新统计信息
来源：http://nh.shxzukj.cn

ANALYZE TABLE users;
来源：http://zv.haigaiapp.cn

[Q71] 查看建表语句
来源：http://jw.bjjhwx.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://lv.lnxyls.cn

[Q72] 查看索引
来源：http://zf.szxytkj.cn

SHOW INDEX FROM users;
来源：http://xy.shxzukj.cn

[Q73] 查看表状态
来源：http://vr.huixinmuqiang.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://nr.haigaiapp.cn

[Q74] 强制使用索引
来源：http://ad.asd995.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://zd.lnxyls.cn

[Q75] 日期格式化
来源：http://yo.yuntaijiaju.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://zc.hahajie.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://cj.hahajie.cn

[Q76] 按天统计
来源：http://yr.szsharing.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://zf.panjiajie.cn

[Q77] 时间加减
来源：http://hd.asd995.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://tt.huanxung.cn

[Q78] 当前时间
来源：http://jh.shxzskj.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ut.panjiajie.cn

[Q79] 字符串拼接
来源：http://zr.shxzukj.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ru.jianghongdianzi.cn

[Q80] 字符串截取
来源：http://bi.521024.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://lr.huixiangedu.cn

[Q81] 字符串替换
来源：http://mn.newstarts.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://nl.nszjky.cn

[Q82] 字符长度与字节长度
来源：http://dc.newstarts.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ba.jctech888.com.cn

[Q83] 大小写转换
来源：http://ao.lnxyls.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ox.szxytkj.cn

[Q84] 去除首尾空格
来源：http://dn.shtwfgs.cn

SELECT TRIM(name) FROM users;
来源：http://xe.hnjuh.cn

[Q85] 数值取整
来源：http://lp.chemitech.net.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://yz.szxytkj.cn

[Q86] 读取 JSON 字段
来源：http://os.szsharing.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ml.lnxyls.cn

[Q87] JSON 字段做条件
来源：http://sc.bjjhwx.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://xt.lnxyls.cn

[Q88] 行转列（条件聚合）
来源：http://kd.lnxyls.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://dq.panjiajie.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://tc.colortex.cn

[Q89] 判断表是否存在
来源：http://ch.9csxet.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mc.haigaiapp.cn

[Q90] 生成序号列
来源：http://kr.shxzukj.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wy.yuexingan06.cn

================================================================================
来源：http://rk.huixiangedu.cn

R. Bash 专题
来源：http://qk.nicolike.cn

================================================================================
来源：http://nk.panjiajie.cn

[R01] shebang 与严格模式
来源：http://fc.shxzskj.cn

#!/usr/bin/env bash
来源：http://sp.chemitech.net.cn

set -euo pipefail
来源：http://jd.yuntaijiaju.cn

[R02] 变量赋值与使用
来源：http://iz.shxzskj.cn

name="Tom"; echo "$name"
来源：http://ge.hnjuh.cn

[R03] 只读变量
来源：http://el.asd995.cn

readonly PI=3.14
来源：http://ja.yuntaijiaju.cn

[R04] 位置参数
来源：http://tt.lnxyls.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://qj.nszjky.cn

[R05] 参数默认值
来源：http://ev.huixinmuqiang.cn

name="${1:-default}"
来源：http://ad.shxzukj.cn

[R06] 判断命令是否存在
来源：http://zm.colortex.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://un.colortex.cn

[R07] if 判断文件
来源：http://jy.szxytkj.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://fe.hahajie.cn

[R08] 数值比较
来源：http://gr.shxzukj.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.gzmigu.cn

[R09] 字符串比较
来源：http://ts.huanxung.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://rl.asd995.cn

[R10] 正则匹配
来源：http://cs.panjiajie.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://yt.asd995.cn

[R11] case 多分支
来源：http://qu.haigaiapp.cn

case "$1" in
来源：http://ak.huixinmuqiang.cn

start) echo "启动" ;;
来源：http://kd.shxzskj.cn

stop)  echo "停止" ;;
来源：http://gk.gzmigu.cn

*)     echo "未知命令" ;;
来源：http://lo.huixiangedu.cn

esac
来源：http://nd.yuntaijiaju.cn

[R12] for 遍历文件
来源：http://li.jianghongdianzi.cn

for f in *.txt; do echo "$f"; done
来源：http://nj.shxzukj.cn

[R13] for 计数循环
来源：http://nz.szxytkj.cn

for i in {1..10}; do echo "$i"; done
来源：http://po.shtwfgs.cn

[R14] C 风格 for
来源：http://zf.yuexingan06.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ev.muxihuayi.cn

[R15] while 逐行读文件
来源：http://bd.lnxyls.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ig.shtwfgs.cn

[R16] until 等待条件
来源：http://qh.chemitech.net.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://lf.huixiangedu.cn

[R17] 数组定义与取值
来源：http://xw.hnjuh.cn

arr=(a b c); echo "${arr[0]}"
来源：http://qr.hahajie.cn

[R18] 遍历数组
来源：http://os.jianghongdianzi.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://nu.hnjuh.cn

[R19] 数组长度
来源：http://js.bookmarksfly.cn

echo "${#arr[@]}"
来源：http://nf.hnjuh.cn

[R20] 关联数组（字典）
来源：http://cr.nszjky.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://sa.chemitech.net.cn

[R21] 字符串长度
来源：http://ir.jctech888.com.cn

echo "${#s}"
来源：http://br.wgjwhj.cn

[R22] 截取子串
来源：http://uo.szxytkj.cn

echo "${s:0:5}"
来源：http://fi.hahajie.cn

[R23] 字符串替换
来源：http://zv.muxihuayi.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://jo.newstarts.cn

[R24] 大小写转换
来源：http://hb.bjjhwx.cn

echo "${s^^}"; echo "${s,,}"
来源：http://ws.hnjuh.cn

[R25] 去后缀 / 去前缀
来源：http://xs.chemitech.net.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://yx.shtwfgs.cn

[R26] 命令替换
来源：http://rx.asd995.cn

now=$(date +%F); echo "$now"
来源：http://nt.shtwfgs.cn

[R27] 算术展开
来源：http://kv.haigaiapp.cn

echo $((1 + 2 * 3))
来源：http://ok.yuntaijiaju.cn

[R28] 浮点运算
来源：http://fu.huixiangedu.cn

echo "scale=2; 10/3" | bc
来源：http://ar.521024.cn

[R29] 定义函数
来源：http://vg.panjiajie.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://uz.wgjwhj.cn

[R30] 函数返回状态码
来源：http://vh.jctech888.com.cn

f() { return 0; }; f || echo "失败了"
来源：http://mo.jctech888.com.cn

[R31] 局部变量
来源：http://gc.asd995.cn

f() { local x=1; echo "$x"; }
来源：http://ae.gzmigu.cn

[R32] 参数个数校验
来源：http://ge.shxzskj.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hg.gzmigu.cn

[R33] 捕获错误并提示行号
来源：http://at.shxzukj.cn


<!-- 参考信息 -->