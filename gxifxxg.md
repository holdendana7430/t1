代发 wailian999

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://zw.nicolike.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wh.panjiajie.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ss.panjiajie.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://fb.lnxyls.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://id.chemitech.net.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://jf.jianghongdianzi.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://gl.521024.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ar.huixinmuqiang.cn

================================================================================
来源：http://zj.szsharing.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wv.yuexingan06.cn

================================================================================
来源：http://tp.szxytkj.cn

[Q01] 创建表
来源：http://uw.jianghongdianzi.cn

CREATE TABLE users (
来源：http://xc.bookmarksfly.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hy.colortex.cn

name VARCHAR(50) NOT NULL,
来源：http://ry.huixinmuqiang.cn

email VARCHAR(100) UNIQUE,
来源：http://lw.wgjwhj.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://yg.jianghongdianzi.cn

);
来源：http://xb.9csxet.cn

[Q02] 创建带外键的表
来源：http://nk.jctech888.com.cn

CREATE TABLE orders (
来源：http://iz.nszjky.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://eh.huanxung.cn

user_id INT NOT NULL,
来源：http://uv.9csxet.cn

amount DECIMAL(10, 2),
来源：http://uu.lnxyls.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://gi.asd995.cn

);
来源：http://hu.chemitech.net.cn

[Q03] 增加列
来源：http://bf.huanxung.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://bp.521024.cn

[Q04] 修改列类型
来源：http://ms.panjiajie.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ev.asd995.cn

[Q05] 重命名列
来源：http://lk.haigaiapp.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://xw.colortex.cn

[Q06] 删除列
来源：http://cw.asd995.cn

ALTER TABLE users DROP COLUMN age;
来源：http://cs.haigaiapp.cn

[Q07] 删除表
来源：http://ww.yuexingan06.cn

DROP TABLE IF EXISTS orders;
来源：http://md.bjjhwx.cn

[Q08] 创建普通索引
来源：http://vh.yuexingan06.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://yn.gzmigu.cn

[Q09] 创建唯一索引
来源：http://me.newstarts.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mp.newstarts.cn

[Q10] 插入单行
来源：http://gl.muxihuayi.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ua.9csxet.cn

[Q11] 一次插入多行
来源：http://py.nicolike.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://cv.wgjwhj.cn

[Q12] 插入后取自增 ID
来源：http://jq.panjiajie.cn

INSERT INTO users (name) VALUES ('C');
来源：http://pd.muxihuayi.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://jb.521024.cn

[Q13] 忽略重复插入
来源：http://gz.shxzskj.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ot.szsharing.cn

[Q14] 存在则更新（upsert）
来源：http://oe.newstarts.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://di.9csxet.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ag.colortex.cn

[Q15] 查询全部
来源：http://xy.wgjwhj.cn

SELECT * FROM users;
来源：http://qo.gzmigu.cn

[Q16] 查询指定列
来源：http://mi.9csxet.cn

SELECT id, name FROM users;
来源：http://bs.huixiangedu.cn

[Q17] 条件查询
来源：http://mr.chemitech.net.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mc.asd995.cn

[Q18] 模糊匹配
来源：http://kf.muxihuayi.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hk.jianghongdianzi.cn

[Q19] 范围查询
来源：http://ci.panjiajie.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ht.lnxyls.cn

[Q20] IN 列表
来源：http://tt.bjjhwx.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://pg.nszjky.cn

[Q21] 空值判断
来源：http://dz.huixiangedu.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://wn.nszjky.cn

[Q22] 排序
来源：http://cw.colortex.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://df.muxihuayi.cn

[Q23] 分页
来源：http://fn.bookmarksfly.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://rn.lnxyls.cn

[Q24] 去重
来源：http://tl.panjiajie.cn

SELECT DISTINCT city FROM users;
来源：http://zf.lnxyls.cn

[Q25] 只取前 N 条
来源：http://xd.gzmigu.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://jl.szsharing.cn

[Q26] 计数
来源：http://zo.chemitech.net.cn

SELECT COUNT(*) FROM users;
来源：http://tv.nicolike.cn

[Q27] 条件计数
来源：http://cg.jctech888.com.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wp.yuntaijiaju.cn

[Q28] 求和与平均
来源：http://zi.szxytkj.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://pp.shxzskj.cn

[Q29] 最大最小值
来源：http://eb.jctech888.com.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://wy.jctech888.com.cn

[Q30] 分组统计
来源：http://mv.szsharing.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ro.panjiajie.cn

[Q31] 分组后过滤
来源：http://fy.huanxung.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://gc.szsharing.cn

[Q32] 分组拼接字符串
来源：http://qf.521024.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://vm.jianghongdianzi.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://gv.9csxet.cn

[Q33] 多列分组
来源：http://zn.yuntaijiaju.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://pa.muxihuayi.cn

[Q34] 每组取第一条
来源：http://ut.chemitech.net.cn

SELECT * FROM (
来源：http://pl.shxzskj.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://vi.jianghongdianzi.cn

) t WHERE rn = 1;
来源：http://ph.nicolike.cn

[Q35] 内连接
来源：http://gb.shxzskj.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://jq.jctech888.com.cn

[Q36] 左连接
来源：http://gk.shtwfgs.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://he.colortex.cn

[Q37] 右连接
来源：http://ld.colortex.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://tf.colortex.cn

[Q38] 全外连接（PostgreSQL）
来源：http://nt.hnjuh.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mt.asd995.cn

[Q39] 自连接（查上下级）
来源：http://pp.yuntaijiaju.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://fh.panjiajie.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wh.szsharing.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://iu.yuexingan06.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ug.shxzukj.cn

[Q41] 多表连接
来源：http://tl.nszjky.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://no.bjjhwx.cn

JOIN users u ON u.id = o.user_id
来源：http://uh.gzmigu.cn

JOIN products p ON p.id = o.product_id;
来源：http://rp.nicolike.cn

[Q42] 连接条件附加过滤
来源：http://dc.bookmarksfly.cn

SELECT u.name, o.amount FROM users u
来源：http://jl.shxzskj.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://vy.9csxet.cn

[Q43] 标量子查询
来源：http://bi.bjjhwx.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://bt.haigaiapp.cn

[Q44] IN 子查询
来源：http://mk.hnjuh.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://fe.wgjwhj.cn

[Q45] EXISTS 判断存在
来源：http://et.huixiangedu.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mt.szxytkj.cn

[Q46] NOT EXISTS 判断不存在
来源：http://kj.huixinmuqiang.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://kq.huixinmuqiang.cn

[Q47] 与平均值比较
来源：http://ce.szsharing.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ko.chemitech.net.cn

[Q48] CTE 公用表表达式
来源：http://dg.szxytkj.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://bw.asd995.cn

SELECT * FROM t WHERE c > 5;
来源：http://mx.shxzukj.cn

[Q49] 更新单行
来源：http://zf.newstarts.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://an.bookmarksfly.cn

[Q50] 批量更新
来源：http://rb.huixinmuqiang.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://ra.nicolike.cn

[Q51] 用子查询更新
来源：http://ij.huanxung.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://kv.hnjuh.cn

[Q52] 删除指定行
来源：http://zh.huanxung.cn

DELETE FROM users WHERE id = 10;
来源：http://db.chemitech.net.cn

[Q53] 按条件删除
来源：http://br.shxzukj.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://aa.bjjhwx.cn

[Q54] 清空表
来源：http://dt.gzmigu.cn

TRUNCATE TABLE logs;
来源：http://np.nszjky.cn

[Q55] 排名（并列占位）
来源：http://yt.colortex.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://tp.yuexingan06.cn

[Q56] 密集排名（并列不占位）
来源：http://cv.szsharing.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://zs.bookmarksfly.cn

[Q57] 行号
来源：http://xn.newstarts.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://tb.hahajie.cn

[Q58] 累计求和
来源：http://zh.9csxet.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://cb.gzmigu.cn

[Q59] 分组内累计
来源：http://zn.wgjwhj.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://lx.gzmigu.cn

[Q60] 取上一行 / 下一行
来源：http://os.yuexingan06.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://nu.gzmigu.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://sh.szsharing.cn

[Q61] 移动平均
来源：http://dv.muxihuayi.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://cc.muxihuayi.cn

[Q62] 分组占比
来源：http://du.chemitech.net.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://rn.panjiajie.cn

[Q63] 开启事务
来源：http://vr.lnxyls.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://vu.yuexingan06.cn

[Q64] 提交事务
来源：http://uj.hahajie.cn

COMMIT;
来源：http://wl.gzmigu.cn

[Q65] 回滚事务
来源：http://em.haigaiapp.cn

ROLLBACK;
来源：http://zf.panjiajie.cn

[Q66] 行锁查询
来源：http://rl.wgjwhj.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://qq.521024.cn

[Q67] 设置隔离级别
来源：http://ad.9csxet.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://bp.nszjky.cn

[Q68] 保存点
来源：http://jy.colortex.cn

SAVEPOINT sp1;
来源：http://pz.nicolike.cn

ROLLBACK TO sp1;
来源：http://hf.521024.cn

[Q69] 查看执行计划
来源：http://qg.jctech888.com.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://xh.huanxung.cn

[Q70] 更新统计信息
来源：http://kf.shxzskj.cn

ANALYZE TABLE users;
来源：http://sk.bookmarksfly.cn

[Q71] 查看建表语句
来源：http://fe.bookmarksfly.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://uz.shxzukj.cn

[Q72] 查看索引
来源：http://yy.gzmigu.cn

SHOW INDEX FROM users;
来源：http://un.nicolike.cn

[Q73] 查看表状态
来源：http://jk.huixiangedu.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://or.gzmigu.cn

[Q74] 强制使用索引
来源：http://rq.panjiajie.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://cc.lnxyls.cn

[Q75] 日期格式化
来源：http://im.lnxyls.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://bi.gzmigu.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ni.szxytkj.cn

[Q76] 按天统计
来源：http://hx.huanxung.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://yn.colortex.cn

[Q77] 时间加减
来源：http://ic.huixinmuqiang.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://kk.gzmigu.cn

[Q78] 当前时间
来源：http://av.hahajie.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://zo.chemitech.net.cn

[Q79] 字符串拼接
来源：http://wm.hnjuh.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ox.yuexingan06.cn

[Q80] 字符串截取
来源：http://rh.wgjwhj.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://xc.9csxet.cn

[Q81] 字符串替换
来源：http://eg.hahajie.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://vl.huanxung.cn

[Q82] 字符长度与字节长度
来源：http://vy.9csxet.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://uk.jianghongdianzi.cn

[Q83] 大小写转换
来源：http://uu.lnxyls.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://qu.huanxung.cn

[Q84] 去除首尾空格
来源：http://cw.jianghongdianzi.cn

SELECT TRIM(name) FROM users;
来源：http://lk.huanxung.cn

[Q85] 数值取整
来源：http://lc.huixiangedu.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://cm.panjiajie.cn

[Q86] 读取 JSON 字段
来源：http://fk.hahajie.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://gy.yuntaijiaju.cn

[Q87] JSON 字段做条件
来源：http://va.haigaiapp.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://tj.colortex.cn

[Q88] 行转列（条件聚合）
来源：http://xs.nszjky.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://no.gzmigu.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://gp.newstarts.cn

[Q89] 判断表是否存在
来源：http://ga.muxihuayi.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ai.yuntaijiaju.cn

[Q90] 生成序号列
来源：http://oi.panjiajie.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://jk.asd995.cn

================================================================================
来源：http://ln.shxzskj.cn

R. Bash 专题
来源：http://po.hahajie.cn

================================================================================
来源：http://wl.huanxung.cn

[R01] shebang 与严格模式
来源：http://ym.nszjky.cn

#!/usr/bin/env bash
来源：http://ld.gzmigu.cn

set -euo pipefail
来源：http://mn.panjiajie.cn

[R02] 变量赋值与使用
来源：http://kf.jctech888.com.cn

name="Tom"; echo "$name"
来源：http://sw.huanxung.cn

[R03] 只读变量
来源：http://og.jctech888.com.cn

readonly PI=3.14
来源：http://je.gzmigu.cn

[R04] 位置参数
来源：http://tm.jianghongdianzi.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://lk.yuexingan06.cn

[R05] 参数默认值
来源：http://eo.szsharing.cn

name="${1:-default}"
来源：http://wk.huanxung.cn

[R06] 判断命令是否存在
来源：http://yu.chemitech.net.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://jw.huanxung.cn

[R07] if 判断文件
来源：http://uh.yuexingan06.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://re.szxytkj.cn

[R08] 数值比较
来源：http://od.bookmarksfly.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://ac.shxzukj.cn

[R09] 字符串比较
来源：http://pr.panjiajie.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ze.bjjhwx.cn

[R10] 正则匹配
来源：http://yt.huixinmuqiang.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://fe.szxytkj.cn

[R11] case 多分支
来源：http://tf.yuexingan06.cn

case "$1" in
来源：http://kb.shtwfgs.cn

start) echo "启动" ;;
来源：http://ec.shxzukj.cn

stop)  echo "停止" ;;
来源：http://uv.yuexingan06.cn

*)     echo "未知命令" ;;
来源：http://ta.gzmigu.cn

esac
来源：http://ar.jctech888.com.cn

[R12] for 遍历文件
来源：http://tz.wgjwhj.cn

for f in *.txt; do echo "$f"; done
来源：http://nx.bjjhwx.cn

[R13] for 计数循环
来源：http://ve.shxzskj.cn

for i in {1..10}; do echo "$i"; done
来源：http://wf.521024.cn

[R14] C 风格 for
来源：http://wc.shxzukj.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://lz.yuntaijiaju.cn

[R15] while 逐行读文件
来源：http://vm.521024.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://yd.huixiangedu.cn

[R16] until 等待条件
来源：http://eh.yuntaijiaju.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://af.nszjky.cn

[R17] 数组定义与取值
来源：http://ee.szsharing.cn

arr=(a b c); echo "${arr[0]}"
来源：http://cx.huixinmuqiang.cn

[R18] 遍历数组
来源：http://ey.huanxung.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://fm.huixiangedu.cn

[R19] 数组长度
来源：http://pn.muxihuayi.cn

echo "${#arr[@]}"
来源：http://kv.nszjky.cn

[R20] 关联数组（字典）
来源：http://fe.shtwfgs.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://dt.jianghongdianzi.cn

[R21] 字符串长度
来源：http://xg.szsharing.cn

echo "${#s}"
来源：http://ac.yuexingan06.cn

[R22] 截取子串
来源：http://aa.chemitech.net.cn

echo "${s:0:5}"
来源：http://wi.szxytkj.cn

[R23] 字符串替换
来源：http://zr.asd995.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ef.nicolike.cn

[R24] 大小写转换
来源：http://ui.shtwfgs.cn

echo "${s^^}"; echo "${s,,}"
来源：http://ua.hnjuh.cn

[R25] 去后缀 / 去前缀
来源：http://oo.jianghongdianzi.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://wj.newstarts.cn

[R26] 命令替换
来源：http://vb.hahajie.cn

now=$(date +%F); echo "$now"
来源：http://ym.bookmarksfly.cn

[R27] 算术展开
来源：http://sz.szxytkj.cn

echo $((1 + 2 * 3))
来源：http://gz.haigaiapp.cn

[R28] 浮点运算
来源：http://ay.jctech888.com.cn

echo "scale=2; 10/3" | bc
来源：http://gl.wgjwhj.cn

[R29] 定义函数
来源：http://vn.nicolike.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://qw.huixiangedu.cn

[R30] 函数返回状态码
来源：http://cs.jianghongdianzi.cn

f() { return 0; }; f || echo "失败了"
来源：http://sg.jianghongdianzi.cn

[R31] 局部变量
来源：http://nq.jctech888.com.cn

f() { local x=1; echo "$x"; }
来源：http://st.szsharing.cn

[R32] 参数个数校验
来源：http://zh.shxzukj.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://vu.szsharing.cn

[R33] 捕获错误并提示行号
来源：http://su.wgjwhj.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://au.szsharing.cn

[R34] 退出时清理
来源：http://pe.colortex.cn

trap 'rm -f "$tmp"' EXIT
来源：http://py.hahajie.cn

[R35] 后台执行并等待
来源：http://dc.colortex.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://nw.haigaiapp.cn

[R36] 并发执行多个任务
来源：http://nz.yuexingan06.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://rf.haigaiapp.cn

[R37] 把输出赋给变量
来源：http://ge.lnxyls.cn

files=$(ls -1)
来源：http://ki.hnjuh.cn

[R38] 管道串联
来源：http://ij.yuexingan06.cn

cat a.txt | grep -i error | wc -l
来源：http://yp.newstarts.cn

[R39] 重定向标准输出与错误
来源：http://ty.colortex.cn


<!-- 参考信息 -->