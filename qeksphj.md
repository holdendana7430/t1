代发 wailian999

PHP:  // 手写时间戳比较
来源：http://ss.shxzskj.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://sv.jctech888.com.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://iu.chemitech.net.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://qk.colortex.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://us.jctech888.com.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://vj.9csxet.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://nx.wgjwhj.cn

[P08] 处理浮点精度问题
来源：http://ex.hahajie.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://pv.bookmarksfly.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://zs.jianghongdianzi.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://yl.bjjhwx.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://al.panjiajie.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://iq.lnxyls.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://oi.newstarts.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://kn.yuntaijiaju.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://fz.nicolike.cn

================================================================================
来源：http://po.521024.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://rf.szxytkj.cn

================================================================================
来源：http://xz.521024.cn

[Q01] 创建表
来源：http://yw.shxzskj.cn

CREATE TABLE users (
来源：http://ws.521024.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://as.jianghongdianzi.cn

name VARCHAR(50) NOT NULL,
来源：http://rf.haigaiapp.cn

email VARCHAR(100) UNIQUE,
来源：http://rx.jctech888.com.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://zj.huixiangedu.cn

);
来源：http://br.shxzskj.cn

[Q02] 创建带外键的表
来源：http://wa.lnxyls.cn

CREATE TABLE orders (
来源：http://fl.nicolike.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://li.huanxung.cn

user_id INT NOT NULL,
来源：http://vo.panjiajie.cn

amount DECIMAL(10, 2),
来源：http://rw.nszjky.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://fd.jctech888.com.cn

);
来源：http://rf.521024.cn

[Q03] 增加列
来源：http://uy.haigaiapp.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://pq.bjjhwx.cn

[Q04] 修改列类型
来源：http://zr.gzmigu.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://cs.haigaiapp.cn

[Q05] 重命名列
来源：http://qd.yuntaijiaju.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ug.bjjhwx.cn

[Q06] 删除列
来源：http://jv.huixiangedu.cn

ALTER TABLE users DROP COLUMN age;
来源：http://tk.bookmarksfly.cn

[Q07] 删除表
来源：http://vf.wgjwhj.cn

DROP TABLE IF EXISTS orders;
来源：http://tt.colortex.cn

[Q08] 创建普通索引
来源：http://cx.bookmarksfly.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://kv.hahajie.cn

[Q09] 创建唯一索引
来源：http://pr.wgjwhj.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://tc.jctech888.com.cn

[Q10] 插入单行
来源：http://wb.shxzukj.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://sp.9csxet.cn

[Q11] 一次插入多行
来源：http://oz.9csxet.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://xa.huanxung.cn

[Q12] 插入后取自增 ID
来源：http://gx.huixiangedu.cn

INSERT INTO users (name) VALUES ('C');
来源：http://lu.lnxyls.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://pb.shtwfgs.cn

[Q13] 忽略重复插入
来源：http://dy.nicolike.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://sb.bjjhwx.cn

[Q14] 存在则更新（upsert）
来源：http://cc.huixiangedu.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ph.panjiajie.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://lv.chemitech.net.cn

[Q15] 查询全部
来源：http://zq.hahajie.cn

SELECT * FROM users;
来源：http://jw.bookmarksfly.cn

[Q16] 查询指定列
来源：http://sj.panjiajie.cn

SELECT id, name FROM users;
来源：http://ej.muxihuayi.cn

[Q17] 条件查询
来源：http://mj.huixiangedu.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://cl.huixiangedu.cn

[Q18] 模糊匹配
来源：http://qx.yuntaijiaju.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://iv.hnjuh.cn

[Q19] 范围查询
来源：http://or.gzmigu.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mp.asd995.cn

[Q20] IN 列表
来源：http://wp.muxihuayi.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://eg.muxihuayi.cn

[Q21] 空值判断
来源：http://ge.huixiangedu.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://yw.asd995.cn

[Q22] 排序
来源：http://jf.asd995.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ja.gzmigu.cn

[Q23] 分页
来源：http://yq.wgjwhj.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ap.asd995.cn

[Q24] 去重
来源：http://oz.muxihuayi.cn

SELECT DISTINCT city FROM users;
来源：http://nw.huixinmuqiang.cn

[Q25] 只取前 N 条
来源：http://fe.shxzskj.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://un.huanxung.cn

[Q26] 计数
来源：http://za.szsharing.cn

SELECT COUNT(*) FROM users;
来源：http://pc.jctech888.com.cn

[Q27] 条件计数
来源：http://iz.huixiangedu.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://zd.asd995.cn

[Q28] 求和与平均
来源：http://nu.hahajie.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://lw.nicolike.cn

[Q29] 最大最小值
来源：http://gm.shxzukj.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://op.bookmarksfly.cn

[Q30] 分组统计
来源：http://vh.haigaiapp.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wn.szsharing.cn

[Q31] 分组后过滤
来源：http://oy.9csxet.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://py.szsharing.cn

[Q32] 分组拼接字符串
来源：http://kb.muxihuayi.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ht.huixiangedu.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://bz.jianghongdianzi.cn

[Q33] 多列分组
来源：http://gy.bjjhwx.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ul.hnjuh.cn

[Q34] 每组取第一条
来源：http://vm.huixiangedu.cn

SELECT * FROM (
来源：http://dw.szsharing.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ra.jctech888.com.cn

) t WHERE rn = 1;
来源：http://ea.shxzskj.cn

[Q35] 内连接
来源：http://ix.haigaiapp.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://uj.jianghongdianzi.cn

[Q36] 左连接
来源：http://ho.colortex.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://pc.newstarts.cn

[Q37] 右连接
来源：http://sz.muxihuayi.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://jc.wgjwhj.cn

[Q38] 全外连接（PostgreSQL）
来源：http://jw.asd995.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://il.panjiajie.cn

[Q39] 自连接（查上下级）
来源：http://xh.huixinmuqiang.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://wf.huixiangedu.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://zh.colortex.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://qu.shxzskj.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://gl.huanxung.cn

[Q41] 多表连接
来源：http://pu.jianghongdianzi.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://pe.huixinmuqiang.cn

JOIN users u ON u.id = o.user_id
来源：http://pr.521024.cn

JOIN products p ON p.id = o.product_id;
来源：http://jo.huanxung.cn

[Q42] 连接条件附加过滤
来源：http://ms.jianghongdianzi.cn

SELECT u.name, o.amount FROM users u
来源：http://wk.huanxung.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://sp.9csxet.cn

[Q43] 标量子查询
来源：http://cs.muxihuayi.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://rg.wgjwhj.cn

[Q44] IN 子查询
来源：http://gh.gzmigu.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://bk.wgjwhj.cn

[Q45] EXISTS 判断存在
来源：http://kg.hnjuh.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://yf.yuntaijiaju.cn

[Q46] NOT EXISTS 判断不存在
来源：http://gl.muxihuayi.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://my.hahajie.cn

[Q47] 与平均值比较
来源：http://fr.huanxung.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ti.panjiajie.cn

[Q48] CTE 公用表表达式
来源：http://kd.wgjwhj.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ix.jctech888.com.cn

SELECT * FROM t WHERE c > 5;
来源：http://vu.chemitech.net.cn

[Q49] 更新单行
来源：http://gu.shtwfgs.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ta.huixiangedu.cn

[Q50] 批量更新
来源：http://zi.bjjhwx.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wd.hahajie.cn

[Q51] 用子查询更新
来源：http://wp.yuntaijiaju.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://pz.hahajie.cn

[Q52] 删除指定行
来源：http://ir.nszjky.cn

DELETE FROM users WHERE id = 10;
来源：http://tq.huixiangedu.cn

[Q53] 按条件删除
来源：http://pz.shtwfgs.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ts.yuexingan06.cn

[Q54] 清空表
来源：http://kn.shxzskj.cn

TRUNCATE TABLE logs;
来源：http://ai.huixiangedu.cn

[Q55] 排名（并列占位）
来源：http://rk.szxytkj.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ul.szsharing.cn

[Q56] 密集排名（并列不占位）
来源：http://na.lnxyls.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://fk.chemitech.net.cn

[Q57] 行号
来源：http://bc.huixiangedu.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://vz.nszjky.cn

[Q58] 累计求和
来源：http://xj.9csxet.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hr.szxytkj.cn

[Q59] 分组内累计
来源：http://cf.wgjwhj.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://yi.521024.cn

[Q60] 取上一行 / 下一行
来源：http://yy.nszjky.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://vp.panjiajie.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://zb.hnjuh.cn

[Q61] 移动平均
来源：http://lp.lnxyls.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ky.huixiangedu.cn

[Q62] 分组占比
来源：http://es.huixiangedu.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://pf.yuntaijiaju.cn

[Q63] 开启事务
来源：http://cx.huixinmuqiang.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://lx.asd995.cn

[Q64] 提交事务
来源：http://jn.nszjky.cn

COMMIT;
来源：http://eu.newstarts.cn

[Q65] 回滚事务
来源：http://ej.bookmarksfly.cn

ROLLBACK;
来源：http://co.521024.cn

[Q66] 行锁查询
来源：http://lj.szsharing.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://fh.jctech888.com.cn

[Q67] 设置隔离级别
来源：http://lf.jctech888.com.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://sy.yuexingan06.cn

[Q68] 保存点
来源：http://ul.yuntaijiaju.cn

SAVEPOINT sp1;
来源：http://gg.colortex.cn

ROLLBACK TO sp1;
来源：http://oy.jianghongdianzi.cn

[Q69] 查看执行计划
来源：http://wk.nicolike.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://zp.jctech888.com.cn

[Q70] 更新统计信息
来源：http://mz.nicolike.cn

ANALYZE TABLE users;
来源：http://sc.bookmarksfly.cn

[Q71] 查看建表语句
来源：http://yg.szsharing.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://yv.jctech888.com.cn

[Q72] 查看索引
来源：http://jn.shxzukj.cn

SHOW INDEX FROM users;
来源：http://cc.huixiangedu.cn

[Q73] 查看表状态
来源：http://sz.shxzukj.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://pc.shxzskj.cn

[Q74] 强制使用索引
来源：http://rf.huixiangedu.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ct.szxytkj.cn

[Q75] 日期格式化
来源：http://po.szxytkj.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wf.hahajie.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ff.nszjky.cn

[Q76] 按天统计
来源：http://gz.szsharing.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://vo.newstarts.cn

[Q77] 时间加减
来源：http://qg.haigaiapp.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ws.shxzukj.cn

[Q78] 当前时间
来源：http://cj.shxzukj.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ip.shxzskj.cn

[Q79] 字符串拼接
来源：http://ff.newstarts.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ka.colortex.cn

[Q80] 字符串截取
来源：http://vk.szxytkj.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://pl.shxzukj.cn

[Q81] 字符串替换
来源：http://vq.newstarts.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mo.szsharing.cn

[Q82] 字符长度与字节长度
来源：http://gu.asd995.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://fi.shxzukj.cn

[Q83] 大小写转换
来源：http://lr.huixiangedu.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://pi.huixiangedu.cn

[Q84] 去除首尾空格
来源：http://xj.nszjky.cn

SELECT TRIM(name) FROM users;
来源：http://xi.nszjky.cn

[Q85] 数值取整
来源：http://hv.szxytkj.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://iv.asd995.cn

[Q86] 读取 JSON 字段
来源：http://so.wgjwhj.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://lc.yuntaijiaju.cn

[Q87] JSON 字段做条件
来源：http://yp.hnjuh.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://pw.hahajie.cn

[Q88] 行转列（条件聚合）
来源：http://ks.lnxyls.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://tv.yuexingan06.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://vb.chemitech.net.cn

[Q89] 判断表是否存在
来源：http://kk.521024.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://aj.bjjhwx.cn

[Q90] 生成序号列
来源：http://th.chemitech.net.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ye.shxzskj.cn

================================================================================
来源：http://ym.nicolike.cn

R. Bash 专题
来源：http://xb.haigaiapp.cn

================================================================================
来源：http://bq.bookmarksfly.cn

[R01] shebang 与严格模式
来源：http://dk.huixinmuqiang.cn

#!/usr/bin/env bash
来源：http://mv.asd995.cn

set -euo pipefail
来源：http://ox.szsharing.cn

[R02] 变量赋值与使用
来源：http://vi.bjjhwx.cn

name="Tom"; echo "$name"
来源：http://ci.asd995.cn

[R03] 只读变量
来源：http://rf.chemitech.net.cn

readonly PI=3.14
来源：http://tn.huixiangedu.cn

[R04] 位置参数
来源：http://ks.hahajie.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://oi.colortex.cn

[R05] 参数默认值
来源：http://ss.muxihuayi.cn

name="${1:-default}"
来源：http://co.colortex.cn

[R06] 判断命令是否存在
来源：http://pi.shxzukj.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://di.szxytkj.cn

[R07] if 判断文件
来源：http://of.jctech888.com.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ao.newstarts.cn

[R08] 数值比较
来源：http://sq.chemitech.net.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://lz.haigaiapp.cn

[R09] 字符串比较
来源：http://lz.shtwfgs.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://gw.jctech888.com.cn

[R10] 正则匹配
来源：http://uk.asd995.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://fs.521024.cn

[R11] case 多分支
来源：http://tn.jianghongdianzi.cn

case "$1" in
来源：http://hs.bookmarksfly.cn

start) echo "启动" ;;
来源：http://ee.nicolike.cn

stop)  echo "停止" ;;
来源：http://bp.lnxyls.cn

*)     echo "未知命令" ;;
来源：http://ce.shxzskj.cn

esac
来源：http://qg.wgjwhj.cn

[R12] for 遍历文件
来源：http://eq.asd995.cn

for f in *.txt; do echo "$f"; done
来源：http://re.9csxet.cn

[R13] for 计数循环
来源：http://sa.szxytkj.cn

for i in {1..10}; do echo "$i"; done
来源：http://et.gzmigu.cn

[R14] C 风格 for
来源：http://ew.nicolike.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://yk.muxihuayi.cn

[R15] while 逐行读文件
来源：http://su.haigaiapp.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ab.panjiajie.cn

[R16] until 等待条件
来源：http://ky.jctech888.com.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://qu.colortex.cn

[R17] 数组定义与取值
来源：http://gn.nicolike.cn

arr=(a b c); echo "${arr[0]}"
来源：http://wj.panjiajie.cn

[R18] 遍历数组
来源：http://ih.521024.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://yv.bjjhwx.cn

[R19] 数组长度
来源：http://kj.9csxet.cn

echo "${#arr[@]}"
来源：http://rq.nicolike.cn

[R20] 关联数组（字典）
来源：http://dn.shtwfgs.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://sh.jctech888.com.cn

[R21] 字符串长度
来源：http://gp.huixinmuqiang.cn

echo "${#s}"
来源：http://hn.huanxung.cn

[R22] 截取子串
来源：http://im.szxytkj.cn

echo "${s:0:5}"
来源：http://qn.9csxet.cn

[R23] 字符串替换
来源：http://da.colortex.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://qf.huixiangedu.cn

[R24] 大小写转换
来源：http://aq.gzmigu.cn

echo "${s^^}"; echo "${s,,}"
来源：http://cz.lnxyls.cn

[R25] 去后缀 / 去前缀
来源：http://hu.bookmarksfly.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://jw.chemitech.net.cn

[R26] 命令替换
来源：http://eu.colortex.cn

now=$(date +%F); echo "$now"
来源：http://pt.lnxyls.cn

[R27] 算术展开
来源：http://xy.nszjky.cn

echo $((1 + 2 * 3))
来源：http://fw.shxzukj.cn

[R28] 浮点运算
来源：http://mf.newstarts.cn

echo "scale=2; 10/3" | bc
来源：http://sk.nicolike.cn

[R29] 定义函数
来源：http://sa.hahajie.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ci.haigaiapp.cn

[R30] 函数返回状态码
来源：http://eo.gzmigu.cn

f() { return 0; }; f || echo "失败了"
来源：http://fg.jianghongdianzi.cn

[R31] 局部变量
来源：http://ta.shxzukj.cn

f() { local x=1; echo "$x"; }
来源：http://jw.huanxung.cn

[R32] 参数个数校验
来源：http://tl.jctech888.com.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://oq.yuntaijiaju.cn

[R33] 捕获错误并提示行号
来源：http://dv.huixiangedu.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://vp.hnjuh.cn

[R34] 退出时清理
来源：http://if.shxzukj.cn

trap 'rm -f "$tmp"' EXIT
来源：http://mh.521024.cn

[R35] 后台执行并等待
来源：http://xa.nicolike.cn


<!-- 参考信息 -->