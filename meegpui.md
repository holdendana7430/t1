代发 wailian999

================================================================================
来源：http://tj.jctech888.com.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wg.panjiajie.cn

================================================================================
来源：http://ow.521024.cn

[Q01] 创建表
来源：http://hq.gzmigu.cn

CREATE TABLE users (
来源：http://zc.jctech888.com.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://pc.hahajie.cn

name VARCHAR(50) NOT NULL,
来源：http://vo.jctech888.com.cn

email VARCHAR(100) UNIQUE,
来源：http://bj.bookmarksfly.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://aa.panjiajie.cn

);
来源：http://kw.muxihuayi.cn

[Q02] 创建带外键的表
来源：http://as.bjjhwx.cn

CREATE TABLE orders (
来源：http://pq.bookmarksfly.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ap.shxzskj.cn

user_id INT NOT NULL,
来源：http://gm.shtwfgs.cn

amount DECIMAL(10, 2),
来源：http://uj.huanxung.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ed.shxzskj.cn

);
来源：http://cl.szsharing.cn

[Q03] 增加列
来源：http://in.shtwfgs.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://dd.muxihuayi.cn

[Q04] 修改列类型
来源：http://ps.colortex.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://bx.hnjuh.cn

[Q05] 重命名列
来源：http://pm.colortex.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ve.hahajie.cn

[Q06] 删除列
来源：http://tw.szsharing.cn

ALTER TABLE users DROP COLUMN age;
来源：http://aw.nszjky.cn

[Q07] 删除表
来源：http://ts.szsharing.cn

DROP TABLE IF EXISTS orders;
来源：http://vq.shtwfgs.cn

[Q08] 创建普通索引
来源：http://nd.huanxung.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://hw.nszjky.cn

[Q09] 创建唯一索引
来源：http://dd.shxzukj.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://gi.chemitech.net.cn

[Q10] 插入单行
来源：http://oy.panjiajie.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://jg.bjjhwx.cn

[Q11] 一次插入多行
来源：http://gp.nicolike.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://vl.shxzukj.cn

[Q12] 插入后取自增 ID
来源：http://tt.szxytkj.cn

INSERT INTO users (name) VALUES ('C');
来源：http://le.shxzukj.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://jd.shxzskj.cn

[Q13] 忽略重复插入
来源：http://lu.bjjhwx.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mr.yuntaijiaju.cn

[Q14] 存在则更新（upsert）
来源：http://bq.hahajie.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://sq.shxzukj.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://uc.szxytkj.cn

[Q15] 查询全部
来源：http://iw.haigaiapp.cn

SELECT * FROM users;
来源：http://ek.9csxet.cn

[Q16] 查询指定列
来源：http://ik.asd995.cn

SELECT id, name FROM users;
来源：http://fm.nicolike.cn

[Q17] 条件查询
来源：http://ho.shxzskj.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://rf.521024.cn

[Q18] 模糊匹配
来源：http://cs.yuexingan06.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://oj.gzmigu.cn

[Q19] 范围查询
来源：http://gj.muxihuayi.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://tl.9csxet.cn

[Q20] IN 列表
来源：http://rx.asd995.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://az.asd995.cn

[Q21] 空值判断
来源：http://kf.bookmarksfly.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://fv.jianghongdianzi.cn

[Q22] 排序
来源：http://yo.shxzskj.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://bo.huanxung.cn

[Q23] 分页
来源：http://sb.wgjwhj.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://sn.huixiangedu.cn

[Q24] 去重
来源：http://ro.jctech888.com.cn

SELECT DISTINCT city FROM users;
来源：http://xt.shtwfgs.cn

[Q25] 只取前 N 条
来源：http://ai.521024.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://re.szxytkj.cn

[Q26] 计数
来源：http://it.jianghongdianzi.cn

SELECT COUNT(*) FROM users;
来源：http://tm.huanxung.cn

[Q27] 条件计数
来源：http://su.shtwfgs.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://am.jctech888.com.cn

[Q28] 求和与平均
来源：http://ic.jianghongdianzi.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://bn.yuexingan06.cn

[Q29] 最大最小值
来源：http://kb.colortex.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://nz.shtwfgs.cn

[Q30] 分组统计
来源：http://ox.lnxyls.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ft.9csxet.cn

[Q31] 分组后过滤
来源：http://le.bjjhwx.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://fh.jctech888.com.cn

[Q32] 分组拼接字符串
来源：http://zb.chemitech.net.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://tl.9csxet.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://xw.lnxyls.cn

[Q33] 多列分组
来源：http://lx.jctech888.com.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://uh.shtwfgs.cn

[Q34] 每组取第一条
来源：http://qg.shtwfgs.cn

SELECT * FROM (
来源：http://zj.asd995.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://yj.hnjuh.cn

) t WHERE rn = 1;
来源：http://ar.gzmigu.cn

[Q35] 内连接
来源：http://eg.colortex.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ax.shxzukj.cn

[Q36] 左连接
来源：http://ee.hnjuh.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://pw.panjiajie.cn

[Q37] 右连接
来源：http://wm.521024.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://fr.521024.cn

[Q38] 全外连接（PostgreSQL）
来源：http://hs.chemitech.net.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ad.9csxet.cn

[Q39] 自连接（查上下级）
来源：http://ws.newstarts.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://ur.nszjky.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ki.asd995.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://fj.yuntaijiaju.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ho.szxytkj.cn

[Q41] 多表连接
来源：http://gt.chemitech.net.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://bt.shxzskj.cn

JOIN users u ON u.id = o.user_id
来源：http://dz.haigaiapp.cn

JOIN products p ON p.id = o.product_id;
来源：http://rb.huixinmuqiang.cn

[Q42] 连接条件附加过滤
来源：http://nz.szsharing.cn

SELECT u.name, o.amount FROM users u
来源：http://gg.newstarts.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://bb.huixiangedu.cn

[Q43] 标量子查询
来源：http://pd.colortex.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://go.muxihuayi.cn

[Q44] IN 子查询
来源：http://ea.newstarts.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ts.huixinmuqiang.cn

[Q45] EXISTS 判断存在
来源：http://ag.nszjky.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ku.szxytkj.cn

[Q46] NOT EXISTS 判断不存在
来源：http://go.asd995.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://yh.hnjuh.cn

[Q47] 与平均值比较
来源：http://ra.panjiajie.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://yn.yuexingan06.cn

[Q48] CTE 公用表表达式
来源：http://xv.panjiajie.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://bt.yuntaijiaju.cn

SELECT * FROM t WHERE c > 5;
来源：http://yi.shxzukj.cn

[Q49] 更新单行
来源：http://tz.szxytkj.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ca.lnxyls.cn

[Q50] 批量更新
来源：http://xd.wgjwhj.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://fr.wgjwhj.cn

[Q51] 用子查询更新
来源：http://mq.nicolike.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://qk.muxihuayi.cn

[Q52] 删除指定行
来源：http://dg.chemitech.net.cn

DELETE FROM users WHERE id = 10;
来源：http://if.yuntaijiaju.cn

[Q53] 按条件删除
来源：http://li.huixinmuqiang.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://bu.gzmigu.cn

[Q54] 清空表
来源：http://jt.yuntaijiaju.cn

TRUNCATE TABLE logs;
来源：http://pq.shxzskj.cn

[Q55] 排名（并列占位）
来源：http://dk.muxihuayi.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://se.gzmigu.cn

[Q56] 密集排名（并列不占位）
来源：http://ys.colortex.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://et.haigaiapp.cn

[Q57] 行号
来源：http://yp.521024.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://fh.bjjhwx.cn

[Q58] 累计求和
来源：http://zy.521024.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://at.yuntaijiaju.cn

[Q59] 分组内累计
来源：http://ub.huixinmuqiang.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://lj.newstarts.cn

[Q60] 取上一行 / 下一行
来源：http://ar.wgjwhj.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://po.shxzukj.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://lu.szsharing.cn

[Q61] 移动平均
来源：http://gt.yuexingan06.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://qc.newstarts.cn

[Q62] 分组占比
来源：http://kh.huanxung.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://tr.shxzukj.cn

[Q63] 开启事务
来源：http://gg.newstarts.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://io.szxytkj.cn

[Q64] 提交事务
来源：http://gn.jctech888.com.cn

COMMIT;
来源：http://dm.haigaiapp.cn

[Q65] 回滚事务
来源：http://up.huanxung.cn

ROLLBACK;
来源：http://ub.wgjwhj.cn

[Q66] 行锁查询
来源：http://ws.bjjhwx.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://tz.bookmarksfly.cn

[Q67] 设置隔离级别
来源：http://rf.asd995.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mr.wgjwhj.cn

[Q68] 保存点
来源：http://yk.muxihuayi.cn

SAVEPOINT sp1;
来源：http://vr.lnxyls.cn

ROLLBACK TO sp1;
来源：http://ne.shtwfgs.cn

[Q69] 查看执行计划
来源：http://yt.nszjky.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://vq.szxytkj.cn

[Q70] 更新统计信息
来源：http://bm.asd995.cn

ANALYZE TABLE users;
来源：http://gg.9csxet.cn

[Q71] 查看建表语句
来源：http://yh.hahajie.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://bm.newstarts.cn

[Q72] 查看索引
来源：http://md.yuexingan06.cn

SHOW INDEX FROM users;
来源：http://ku.wgjwhj.cn

[Q73] 查看表状态
来源：http://qs.shtwfgs.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://vg.nszjky.cn

[Q74] 强制使用索引
来源：http://kz.newstarts.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://kd.haigaiapp.cn

[Q75] 日期格式化
来源：http://ok.nicolike.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ap.shxzukj.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://cd.521024.cn

[Q76] 按天统计
来源：http://hv.chemitech.net.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://aj.huanxung.cn

[Q77] 时间加减
来源：http://js.newstarts.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://dr.shxzukj.cn

[Q78] 当前时间
来源：http://lp.chemitech.net.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://kt.bjjhwx.cn

[Q79] 字符串拼接
来源：http://aq.yuexingan06.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ix.szxytkj.cn

[Q80] 字符串截取
来源：http://jq.bjjhwx.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://fo.colortex.cn

[Q81] 字符串替换
来源：http://wm.jctech888.com.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://kx.lnxyls.cn

[Q82] 字符长度与字节长度
来源：http://qd.haigaiapp.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mn.wgjwhj.cn

[Q83] 大小写转换
来源：http://em.colortex.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://lv.shxzskj.cn

[Q84] 去除首尾空格
来源：http://ah.shtwfgs.cn

SELECT TRIM(name) FROM users;
来源：http://cy.wgjwhj.cn

[Q85] 数值取整
来源：http://wf.panjiajie.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mj.muxihuayi.cn

[Q86] 读取 JSON 字段
来源：http://vj.huixinmuqiang.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://su.haigaiapp.cn

[Q87] JSON 字段做条件
来源：http://fv.bjjhwx.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mc.jianghongdianzi.cn

[Q88] 行转列（条件聚合）
来源：http://mq.haigaiapp.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://cc.szsharing.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://uz.lnxyls.cn

[Q89] 判断表是否存在
来源：http://rp.asd995.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://rd.hnjuh.cn

[Q90] 生成序号列
来源：http://ez.hahajie.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ej.haigaiapp.cn

================================================================================
来源：http://mt.haigaiapp.cn

R. Bash 专题
来源：http://uk.newstarts.cn

================================================================================
来源：http://wm.shtwfgs.cn

[R01] shebang 与严格模式
来源：http://au.szsharing.cn

#!/usr/bin/env bash
来源：http://pf.nszjky.cn

set -euo pipefail
来源：http://yj.asd995.cn

[R02] 变量赋值与使用
来源：http://rq.colortex.cn

name="Tom"; echo "$name"
来源：http://yo.lnxyls.cn

[R03] 只读变量
来源：http://zk.newstarts.cn

readonly PI=3.14
来源：http://gh.panjiajie.cn

[R04] 位置参数
来源：http://dg.shxzskj.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://yk.lnxyls.cn

[R05] 参数默认值
来源：http://gr.huixiangedu.cn

name="${1:-default}"
来源：http://vf.huixiangedu.cn

[R06] 判断命令是否存在
来源：http://xx.huixiangedu.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://zl.lnxyls.cn

[R07] if 判断文件
来源：http://kw.newstarts.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ix.nszjky.cn

[R08] 数值比较
来源：http://wv.huixinmuqiang.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://bl.521024.cn

[R09] 字符串比较
来源：http://cy.521024.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://us.jctech888.com.cn

[R10] 正则匹配
来源：http://gn.bjjhwx.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hh.jianghongdianzi.cn

[R11] case 多分支
来源：http://xo.asd995.cn

case "$1" in
来源：http://kx.szxytkj.cn

start) echo "启动" ;;
来源：http://hh.panjiajie.cn

stop)  echo "停止" ;;
来源：http://ah.asd995.cn

*)     echo "未知命令" ;;
来源：http://ll.huixinmuqiang.cn

esac
来源：http://sz.shxzukj.cn

[R12] for 遍历文件
来源：http://po.huixiangedu.cn

for f in *.txt; do echo "$f"; done
来源：http://jc.jctech888.com.cn

[R13] for 计数循环
来源：http://ey.shtwfgs.cn

for i in {1..10}; do echo "$i"; done
来源：http://ng.gzmigu.cn

[R14] C 风格 for
来源：http://kb.wgjwhj.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://yb.lnxyls.cn

[R15] while 逐行读文件
来源：http://qq.9csxet.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://oj.9csxet.cn

[R16] until 等待条件
来源：http://am.asd995.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ef.colortex.cn

[R17] 数组定义与取值
来源：http://pj.chemitech.net.cn

arr=(a b c); echo "${arr[0]}"
来源：http://ev.gzmigu.cn

[R18] 遍历数组
来源：http://rc.shxzskj.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://pq.asd995.cn

[R19] 数组长度
来源：http://sp.asd995.cn

echo "${#arr[@]}"
来源：http://ro.shtwfgs.cn

[R20] 关联数组（字典）
来源：http://oi.yuntaijiaju.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ke.colortex.cn

[R21] 字符串长度
来源：http://we.bookmarksfly.cn

echo "${#s}"
来源：http://hl.bjjhwx.cn

[R22] 截取子串
来源：http://it.bookmarksfly.cn

echo "${s:0:5}"
来源：http://vw.huixinmuqiang.cn

[R23] 字符串替换
来源：http://pq.hnjuh.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://zv.jianghongdianzi.cn

[R24] 大小写转换
来源：http://gm.muxihuayi.cn

echo "${s^^}"; echo "${s,,}"
来源：http://zr.jctech888.com.cn

[R25] 去后缀 / 去前缀
来源：http://sr.9csxet.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://sx.521024.cn

[R26] 命令替换
来源：http://js.9csxet.cn

now=$(date +%F); echo "$now"
来源：http://ra.haigaiapp.cn

[R27] 算术展开
来源：http://ie.shxzukj.cn

echo $((1 + 2 * 3))
来源：http://dn.huixiangedu.cn

[R28] 浮点运算
来源：http://pc.shxzskj.cn

echo "scale=2; 10/3" | bc
来源：http://xl.szsharing.cn

[R29] 定义函数
来源：http://vu.chemitech.net.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://qk.panjiajie.cn

[R30] 函数返回状态码
来源：http://xe.asd995.cn

f() { return 0; }; f || echo "失败了"
来源：http://dv.bookmarksfly.cn

[R31] 局部变量
来源：http://gk.asd995.cn

f() { local x=1; echo "$x"; }
来源：http://oz.nszjky.cn

[R32] 参数个数校验
来源：http://pk.colortex.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://xh.lnxyls.cn

[R33] 捕获错误并提示行号
来源：http://ei.huanxung.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://uw.muxihuayi.cn

[R34] 退出时清理
来源：http://jh.szxytkj.cn

trap 'rm -f "$tmp"' EXIT
来源：http://uh.jctech888.com.cn

[R35] 后台执行并等待
来源：http://cy.asd995.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://xw.hahajie.cn

[R36] 并发执行多个任务
来源：http://al.lnxyls.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://il.bjjhwx.cn

[R37] 把输出赋给变量
来源：http://hz.huixiangedu.cn

files=$(ls -1)
来源：http://il.huanxung.cn

[R38] 管道串联
来源：http://xd.lnxyls.cn

cat a.txt | grep -i error | wc -l
来源：http://sy.yuexingan06.cn

[R39] 重定向标准输出与错误
来源：http://ab.bjjhwx.cn

cmd > out.log 2>&1
来源：http://vw.yuexingan06.cn

[R40] 追加写日志
来源：http://tp.newstarts.cn

echo "log" >> out.log
来源：http://rt.jianghongdianzi.cn

[R41] 丢弃输出
来源：http://dj.jianghongdianzi.cn

cmd >/dev/null 2>&1
来源：http://af.9csxet.cn

[R42] 输入重定向
来源：http://cc.huixinmuqiang.cn

wc -l < a.txt
来源：http://xq.yuntaijiaju.cn

[R43] 按名字查找文件
来源：http://lj.gzmigu.cn


<!-- 参考信息 -->