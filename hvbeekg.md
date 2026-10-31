代发 wailian999

PHP:  // 手写时间戳比较
来源：http://bw.huixiangedu.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://fa.panjiajie.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://sr.huanxung.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://fa.bookmarksfly.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://at.szsharing.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://ux.lnxyls.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://pc.bookmarksfly.cn

[P08] 处理浮点精度问题
来源：http://te.huixiangedu.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://jg.shxzskj.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://bn.chemitech.net.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ae.wgjwhj.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://fk.521024.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ox.huanxung.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://xn.gzmigu.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://iz.newstarts.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://na.521024.cn

================================================================================
来源：http://mm.lnxyls.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ti.hahajie.cn

================================================================================
来源：http://lr.lnxyls.cn

[Q01] 创建表
来源：http://bp.bookmarksfly.cn

CREATE TABLE users (
来源：http://xu.lnxyls.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://vj.haigaiapp.cn

name VARCHAR(50) NOT NULL,
来源：http://jk.shxzukj.cn

email VARCHAR(100) UNIQUE,
来源：http://qq.newstarts.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://rt.nszjky.cn

);
来源：http://pd.nszjky.cn

[Q02] 创建带外键的表
来源：http://pz.yuntaijiaju.cn

CREATE TABLE orders (
来源：http://cy.nicolike.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://my.huanxung.cn

user_id INT NOT NULL,
来源：http://jd.9csxet.cn

amount DECIMAL(10, 2),
来源：http://ab.shtwfgs.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mj.hnjuh.cn

);
来源：http://bp.bookmarksfly.cn

[Q03] 增加列
来源：http://rc.bjjhwx.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mv.asd995.cn

[Q04] 修改列类型
来源：http://qs.9csxet.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://gs.jianghongdianzi.cn

[Q05] 重命名列
来源：http://pe.haigaiapp.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://bd.nszjky.cn

[Q06] 删除列
来源：http://uj.szsharing.cn

ALTER TABLE users DROP COLUMN age;
来源：http://pz.hahajie.cn

[Q07] 删除表
来源：http://hk.newstarts.cn

DROP TABLE IF EXISTS orders;
来源：http://vx.wgjwhj.cn

[Q08] 创建普通索引
来源：http://zk.szsharing.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://uq.bjjhwx.cn

[Q09] 创建唯一索引
来源：http://te.hahajie.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://qq.bookmarksfly.cn

[Q10] 插入单行
来源：http://ls.haigaiapp.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ow.huanxung.cn

[Q11] 一次插入多行
来源：http://mu.521024.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://kr.9csxet.cn

[Q12] 插入后取自增 ID
来源：http://jw.haigaiapp.cn

INSERT INTO users (name) VALUES ('C');
来源：http://gj.hahajie.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://zb.lnxyls.cn

[Q13] 忽略重复插入
来源：http://og.wgjwhj.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://nw.yuexingan06.cn

[Q14] 存在则更新（upsert）
来源：http://rk.shxzskj.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hx.bjjhwx.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ht.nicolike.cn

[Q15] 查询全部
来源：http://yg.shxzukj.cn

SELECT * FROM users;
来源：http://vp.newstarts.cn

[Q16] 查询指定列
来源：http://kk.shxzskj.cn

SELECT id, name FROM users;
来源：http://tq.gzmigu.cn

[Q17] 条件查询
来源：http://sw.haigaiapp.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://nh.jianghongdianzi.cn

[Q18] 模糊匹配
来源：http://ft.nszjky.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://kj.shtwfgs.cn

[Q19] 范围查询
来源：http://pf.nszjky.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ut.9csxet.cn

[Q20] IN 列表
来源：http://nv.huixinmuqiang.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://pu.lnxyls.cn

[Q21] 空值判断
来源：http://hf.lnxyls.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://ak.shxzukj.cn

[Q22] 排序
来源：http://mz.521024.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hn.haigaiapp.cn

[Q23] 分页
来源：http://wb.huanxung.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://gn.haigaiapp.cn

[Q24] 去重
来源：http://po.wgjwhj.cn

SELECT DISTINCT city FROM users;
来源：http://bk.huanxung.cn

[Q25] 只取前 N 条
来源：http://io.muxihuayi.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://nf.nszjky.cn

[Q26] 计数
来源：http://ty.muxihuayi.cn

SELECT COUNT(*) FROM users;
来源：http://ye.shxzukj.cn

[Q27] 条件计数
来源：http://hq.yuexingan06.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://br.9csxet.cn

[Q28] 求和与平均
来源：http://gs.jctech888.com.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://on.hnjuh.cn

[Q29] 最大最小值
来源：http://ef.yuntaijiaju.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://fk.lnxyls.cn

[Q30] 分组统计
来源：http://ba.shxzukj.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hv.huixiangedu.cn

[Q31] 分组后过滤
来源：http://li.bookmarksfly.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://zo.wgjwhj.cn

[Q32] 分组拼接字符串
来源：http://hd.huanxung.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wn.muxihuayi.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wg.bjjhwx.cn

[Q33] 多列分组
来源：http://ch.yuexingan06.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://lz.jianghongdianzi.cn

[Q34] 每组取第一条
来源：http://hz.yuexingan06.cn

SELECT * FROM (
来源：http://vd.hahajie.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ne.lnxyls.cn

) t WHERE rn = 1;
来源：http://rf.521024.cn

[Q35] 内连接
来源：http://jp.muxihuayi.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mi.hnjuh.cn

[Q36] 左连接
来源：http://op.jianghongdianzi.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ob.9csxet.cn

[Q37] 右连接
来源：http://kq.asd995.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mr.jctech888.com.cn

[Q38] 全外连接（PostgreSQL）
来源：http://is.hnjuh.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://tc.panjiajie.cn

[Q39] 自连接（查上下级）
来源：http://qp.szxytkj.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://rb.panjiajie.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://qq.szsharing.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://ad.hahajie.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://tc.jctech888.com.cn

[Q41] 多表连接
来源：http://gs.szxytkj.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://ko.bookmarksfly.cn

JOIN users u ON u.id = o.user_id
来源：http://ol.nszjky.cn

JOIN products p ON p.id = o.product_id;
来源：http://vm.wgjwhj.cn

[Q42] 连接条件附加过滤
来源：http://al.colortex.cn

SELECT u.name, o.amount FROM users u
来源：http://da.bjjhwx.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://gq.gzmigu.cn

[Q43] 标量子查询
来源：http://jl.jianghongdianzi.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://en.wgjwhj.cn

[Q44] IN 子查询
来源：http://gi.newstarts.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://fh.9csxet.cn

[Q45] EXISTS 判断存在
来源：http://sg.muxihuayi.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://er.gzmigu.cn

[Q46] NOT EXISTS 判断不存在
来源：http://ii.szsharing.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://gb.shxzskj.cn

[Q47] 与平均值比较
来源：http://mf.wgjwhj.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mx.jctech888.com.cn

[Q48] CTE 公用表表达式
来源：http://tj.panjiajie.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://yc.hahajie.cn

SELECT * FROM t WHERE c > 5;
来源：http://na.521024.cn

[Q49] 更新单行
来源：http://zp.newstarts.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://jh.huixinmuqiang.cn

[Q50] 批量更新
来源：http://cn.szxytkj.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://xf.panjiajie.cn

[Q51] 用子查询更新
来源：http://qn.huixinmuqiang.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://vg.hnjuh.cn

[Q52] 删除指定行
来源：http://ve.shxzskj.cn

DELETE FROM users WHERE id = 10;
来源：http://am.newstarts.cn

[Q53] 按条件删除
来源：http://ji.hnjuh.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://fo.huanxung.cn

[Q54] 清空表
来源：http://ld.szxytkj.cn

TRUNCATE TABLE logs;
来源：http://cc.521024.cn

[Q55] 排名（并列占位）
来源：http://eb.hahajie.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ov.bjjhwx.cn

[Q56] 密集排名（并列不占位）
来源：http://po.bjjhwx.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://rr.nicolike.cn

[Q57] 行号
来源：http://yb.huixiangedu.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://um.haigaiapp.cn

[Q58] 累计求和
来源：http://yl.gzmigu.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://tl.521024.cn

[Q59] 分组内累计
来源：http://ih.lnxyls.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://kk.wgjwhj.cn

[Q60] 取上一行 / 下一行
来源：http://hd.asd995.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://rs.bjjhwx.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://iz.nicolike.cn

[Q61] 移动平均
来源：http://an.jianghongdianzi.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://cy.huixiangedu.cn

[Q62] 分组占比
来源：http://kt.shtwfgs.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hn.colortex.cn

[Q63] 开启事务
来源：http://jg.colortex.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://aw.nszjky.cn

[Q64] 提交事务
来源：http://sq.asd995.cn

COMMIT;
来源：http://jm.bjjhwx.cn

[Q65] 回滚事务
来源：http://bs.huixiangedu.cn

ROLLBACK;
来源：http://nk.colortex.cn

[Q66] 行锁查询
来源：http://po.gzmigu.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ms.asd995.cn

[Q67] 设置隔离级别
来源：http://mg.wgjwhj.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hm.yuexingan06.cn

[Q68] 保存点
来源：http://yq.colortex.cn

SAVEPOINT sp1;
来源：http://dc.asd995.cn

ROLLBACK TO sp1;
来源：http://ur.colortex.cn

[Q69] 查看执行计划
来源：http://jc.huanxung.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hv.szsharing.cn

[Q70] 更新统计信息
来源：http://hu.521024.cn

ANALYZE TABLE users;
来源：http://np.szsharing.cn

[Q71] 查看建表语句
来源：http://iz.shxzskj.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://sg.bjjhwx.cn

[Q72] 查看索引
来源：http://bk.jianghongdianzi.cn

SHOW INDEX FROM users;
来源：http://fv.newstarts.cn

[Q73] 查看表状态
来源：http://zv.hnjuh.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://ws.newstarts.cn

[Q74] 强制使用索引
来源：http://mz.colortex.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://gl.asd995.cn

[Q75] 日期格式化
来源：http://zi.lnxyls.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://gs.9csxet.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://uy.szxytkj.cn

[Q76] 按天统计
来源：http://fd.521024.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://qg.shxzskj.cn

[Q77] 时间加减
来源：http://fc.szxytkj.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://rq.jianghongdianzi.cn

[Q78] 当前时间
来源：http://om.shtwfgs.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://qp.shxzskj.cn

[Q79] 字符串拼接
来源：http://it.muxihuayi.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ny.huixiangedu.cn

[Q80] 字符串截取
来源：http://jc.colortex.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://st.nicolike.cn

[Q81] 字符串替换
来源：http://fy.jianghongdianzi.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ck.szsharing.cn

[Q82] 字符长度与字节长度
来源：http://vf.hahajie.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://qd.hahajie.cn

[Q83] 大小写转换
来源：http://sm.szsharing.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wv.huanxung.cn

[Q84] 去除首尾空格
来源：http://gq.chemitech.net.cn

SELECT TRIM(name) FROM users;
来源：http://cl.wgjwhj.cn

[Q85] 数值取整
来源：http://cy.jianghongdianzi.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://rt.wgjwhj.cn

[Q86] 读取 JSON 字段
来源：http://rb.nicolike.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://es.colortex.cn

[Q87] JSON 字段做条件
来源：http://kk.szxytkj.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://iu.shtwfgs.cn

[Q88] 行转列（条件聚合）
来源：http://jo.jctech888.com.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wj.huanxung.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ze.wgjwhj.cn

[Q89] 判断表是否存在
来源：http://cv.hahajie.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://oy.hahajie.cn

[Q90] 生成序号列
来源：http://hm.nszjky.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://aj.521024.cn

================================================================================
来源：http://an.jctech888.com.cn

R. Bash 专题
来源：http://le.szxytkj.cn

================================================================================
来源：http://qq.newstarts.cn

[R01] shebang 与严格模式
来源：http://kw.szsharing.cn

#!/usr/bin/env bash
来源：http://rt.haigaiapp.cn

set -euo pipefail
来源：http://tg.jianghongdianzi.cn

[R02] 变量赋值与使用
来源：http://mk.huixiangedu.cn

name="Tom"; echo "$name"
来源：http://ds.hahajie.cn

[R03] 只读变量
来源：http://gh.newstarts.cn

readonly PI=3.14
来源：http://hi.hahajie.cn

[R04] 位置参数
来源：http://di.wgjwhj.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://dr.muxihuayi.cn

[R05] 参数默认值
来源：http://vt.bookmarksfly.cn

name="${1:-default}"
来源：http://dh.hnjuh.cn

[R06] 判断命令是否存在
来源：http://cg.nszjky.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://gr.hahajie.cn

[R07] if 判断文件
来源：http://rf.lnxyls.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://jw.jianghongdianzi.cn

[R08] 数值比较
来源：http://vo.muxihuayi.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://lo.shxzukj.cn

[R09] 字符串比较
来源：http://be.chemitech.net.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ye.szxytkj.cn

[R10] 正则匹配
来源：http://bi.jianghongdianzi.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://uf.nszjky.cn

[R11] case 多分支
来源：http://er.shxzskj.cn

case "$1" in
来源：http://te.gzmigu.cn

start) echo "启动" ;;
来源：http://sk.huixinmuqiang.cn

stop)  echo "停止" ;;
来源：http://if.wgjwhj.cn

*)     echo "未知命令" ;;
来源：http://km.shxzukj.cn

esac
来源：http://rm.shtwfgs.cn

[R12] for 遍历文件
来源：http://sy.szsharing.cn

for f in *.txt; do echo "$f"; done
来源：http://ys.wgjwhj.cn

[R13] for 计数循环
来源：http://da.9csxet.cn

for i in {1..10}; do echo "$i"; done
来源：http://aa.nicolike.cn

[R14] C 风格 for
来源：http://tb.szsharing.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ub.huixinmuqiang.cn

[R15] while 逐行读文件
来源：http://bn.jctech888.com.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://dm.shtwfgs.cn

[R16] until 等待条件
来源：http://bp.asd995.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://bm.szsharing.cn

[R17] 数组定义与取值
来源：http://bd.huanxung.cn

arr=(a b c); echo "${arr[0]}"
来源：http://yp.muxihuayi.cn

[R18] 遍历数组
来源：http://sa.shxzukj.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://vk.asd995.cn

[R19] 数组长度
来源：http://ho.haigaiapp.cn

echo "${#arr[@]}"
来源：http://hb.lnxyls.cn

[R20] 关联数组（字典）
来源：http://zd.521024.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://lx.huixiangedu.cn

[R21] 字符串长度
来源：http://gw.hnjuh.cn

echo "${#s}"
来源：http://zc.521024.cn

[R22] 截取子串
来源：http://py.yuexingan06.cn

echo "${s:0:5}"
来源：http://ym.muxihuayi.cn

[R23] 字符串替换
来源：http://qa.nicolike.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mi.shxzskj.cn

[R24] 大小写转换
来源：http://dk.jctech888.com.cn

echo "${s^^}"; echo "${s,,}"
来源：http://bb.huixinmuqiang.cn

[R25] 去后缀 / 去前缀
来源：http://wn.9csxet.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://mw.shxzskj.cn

[R26] 命令替换
来源：http://dk.bookmarksfly.cn

now=$(date +%F); echo "$now"
来源：http://fs.huixiangedu.cn

[R27] 算术展开
来源：http://yw.bookmarksfly.cn

echo $((1 + 2 * 3))
来源：http://co.huanxung.cn

[R28] 浮点运算
来源：http://qg.chemitech.net.cn

echo "scale=2; 10/3" | bc
来源：http://of.huixiangedu.cn

[R29] 定义函数
来源：http://br.panjiajie.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://gj.hahajie.cn

[R30] 函数返回状态码
来源：http://ye.haigaiapp.cn

f() { return 0; }; f || echo "失败了"
来源：http://iz.muxihuayi.cn

[R31] 局部变量
来源：http://cr.yuexingan06.cn

f() { local x=1; echo "$x"; }
来源：http://je.gzmigu.cn

[R32] 参数个数校验
来源：http://ka.huanxung.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://kd.521024.cn

[R33] 捕获错误并提示行号
来源：http://vs.nszjky.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ot.shxzskj.cn

[R34] 退出时清理
来源：http://tx.jianghongdianzi.cn

trap 'rm -f "$tmp"' EXIT
来源：http://ph.szsharing.cn

[R35] 后台执行并等待
来源：http://bq.hnjuh.cn


<!-- 参考信息 -->