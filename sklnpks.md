代发 wailian999

================================================================================
来源：http://qc.muxihuayi.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://he.jctech888.com.cn

================================================================================
来源：http://sb.hnjuh.cn

[Q01] 创建表
来源：http://io.yuexingan06.cn

CREATE TABLE users (
来源：http://rk.yuexingan06.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://vk.9csxet.cn

name VARCHAR(50) NOT NULL,
来源：http://uf.huixinmuqiang.cn

email VARCHAR(100) UNIQUE,
来源：http://wo.huixinmuqiang.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://gf.nicolike.cn

);
来源：http://kt.colortex.cn

[Q02] 创建带外键的表
来源：http://fo.wgjwhj.cn

CREATE TABLE orders (
来源：http://ov.muxihuayi.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://kb.newstarts.cn

user_id INT NOT NULL,
来源：http://al.chemitech.net.cn

amount DECIMAL(10, 2),
来源：http://si.szsharing.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://sk.hnjuh.cn

);
来源：http://ly.bjjhwx.cn

[Q03] 增加列
来源：http://qh.shxzukj.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://rl.hnjuh.cn

[Q04] 修改列类型
来源：http://sf.colortex.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://va.chemitech.net.cn

[Q05] 重命名列
来源：http://lp.lnxyls.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://tj.muxihuayi.cn

[Q06] 删除列
来源：http://yd.521024.cn

ALTER TABLE users DROP COLUMN age;
来源：http://zl.huixiangedu.cn

[Q07] 删除表
来源：http://df.lnxyls.cn

DROP TABLE IF EXISTS orders;
来源：http://uq.yuntaijiaju.cn

[Q08] 创建普通索引
来源：http://jf.shxzskj.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://dy.gzmigu.cn

[Q09] 创建唯一索引
来源：http://rg.newstarts.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://un.asd995.cn

[Q10] 插入单行
来源：http://va.nszjky.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://nl.bookmarksfly.cn

[Q11] 一次插入多行
来源：http://lu.huixinmuqiang.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://nb.jctech888.com.cn

[Q12] 插入后取自增 ID
来源：http://lg.shtwfgs.cn

INSERT INTO users (name) VALUES ('C');
来源：http://jg.nszjky.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://iu.9csxet.cn

[Q13] 忽略重复插入
来源：http://xf.muxihuayi.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://qd.chemitech.net.cn

[Q14] 存在则更新（upsert）
来源：http://fy.szxytkj.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mm.yuexingan06.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://vn.chemitech.net.cn

[Q15] 查询全部
来源：http://rn.huanxung.cn

SELECT * FROM users;
来源：http://zk.shtwfgs.cn

[Q16] 查询指定列
来源：http://wc.jianghongdianzi.cn

SELECT id, name FROM users;
来源：http://wo.muxihuayi.cn

[Q17] 条件查询
来源：http://zy.szsharing.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hv.huanxung.cn

[Q18] 模糊匹配
来源：http://hl.newstarts.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://jd.521024.cn

[Q19] 范围查询
来源：http://dq.chemitech.net.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://gn.wgjwhj.cn

[Q20] IN 列表
来源：http://zl.huixinmuqiang.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ps.lnxyls.cn

[Q21] 空值判断
来源：http://rz.yuexingan06.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://qi.muxihuayi.cn

[Q22] 排序
来源：http://gd.nicolike.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://bo.newstarts.cn

[Q23] 分页
来源：http://yh.asd995.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://yr.haigaiapp.cn

[Q24] 去重
来源：http://vm.szxytkj.cn

SELECT DISTINCT city FROM users;
来源：http://yz.nszjky.cn

[Q25] 只取前 N 条
来源：http://wb.bookmarksfly.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://pn.shxzukj.cn

[Q26] 计数
来源：http://ce.jianghongdianzi.cn

SELECT COUNT(*) FROM users;
来源：http://ig.haigaiapp.cn

[Q27] 条件计数
来源：http://mr.asd995.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ll.jianghongdianzi.cn

[Q28] 求和与平均
来源：http://iz.newstarts.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://vq.huixinmuqiang.cn

[Q29] 最大最小值
来源：http://dl.huanxung.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://zc.jctech888.com.cn

[Q30] 分组统计
来源：http://jg.shxzukj.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://xv.szsharing.cn

[Q31] 分组后过滤
来源：http://nb.lnxyls.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://lr.hnjuh.cn

[Q32] 分组拼接字符串
来源：http://gz.hahajie.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ce.yuexingan06.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://tm.wgjwhj.cn

[Q33] 多列分组
来源：http://rr.shxzskj.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://qc.jctech888.com.cn

[Q34] 每组取第一条
来源：http://vk.521024.cn

SELECT * FROM (
来源：http://qw.nszjky.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wv.hnjuh.cn

) t WHERE rn = 1;
来源：http://jr.shtwfgs.cn

[Q35] 内连接
来源：http://xr.shxzskj.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ti.yuexingan06.cn

[Q36] 左连接
来源：http://kj.muxihuayi.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://yx.nszjky.cn

[Q37] 右连接
来源：http://tv.9csxet.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://jk.9csxet.cn

[Q38] 全外连接（PostgreSQL）
来源：http://hj.yuntaijiaju.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://px.wgjwhj.cn

[Q39] 自连接（查上下级）
来源：http://em.hnjuh.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://nj.jctech888.com.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wl.hahajie.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://uh.huanxung.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://au.yuexingan06.cn

[Q41] 多表连接
来源：http://rp.jianghongdianzi.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://ix.hahajie.cn

JOIN users u ON u.id = o.user_id
来源：http://vh.gzmigu.cn

JOIN products p ON p.id = o.product_id;
来源：http://si.jianghongdianzi.cn

[Q42] 连接条件附加过滤
来源：http://ct.bjjhwx.cn

SELECT u.name, o.amount FROM users u
来源：http://ne.asd995.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://rp.szxytkj.cn

[Q43] 标量子查询
来源：http://dv.9csxet.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://dv.huanxung.cn

[Q44] IN 子查询
来源：http://iy.lnxyls.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://zk.shtwfgs.cn

[Q45] EXISTS 判断存在
来源：http://wk.9csxet.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://zz.lnxyls.cn

[Q46] NOT EXISTS 判断不存在
来源：http://rp.szxytkj.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://tl.asd995.cn

[Q47] 与平均值比较
来源：http://sa.huixinmuqiang.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://da.chemitech.net.cn

[Q48] CTE 公用表表达式
来源：http://qf.chemitech.net.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://as.gzmigu.cn

SELECT * FROM t WHERE c > 5;
来源：http://qw.yuexingan06.cn

[Q49] 更新单行
来源：http://ty.wgjwhj.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ev.bjjhwx.cn

[Q50] 批量更新
来源：http://pk.shxzskj.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://nl.bookmarksfly.cn

[Q51] 用子查询更新
来源：http://wh.chemitech.net.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://ix.shxzskj.cn

[Q52] 删除指定行
来源：http://od.bjjhwx.cn

DELETE FROM users WHERE id = 10;
来源：http://la.shxzskj.cn

[Q53] 按条件删除
来源：http://ol.shxzukj.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://uh.newstarts.cn

[Q54] 清空表
来源：http://xn.asd995.cn

TRUNCATE TABLE logs;
来源：http://ng.shxzskj.cn

[Q55] 排名（并列占位）
来源：http://vl.nszjky.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://sq.muxihuayi.cn

[Q56] 密集排名（并列不占位）
来源：http://mp.shxzukj.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://vp.9csxet.cn

[Q57] 行号
来源：http://mu.yuexingan06.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://rg.haigaiapp.cn

[Q58] 累计求和
来源：http://uf.huanxung.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://bw.yuexingan06.cn

[Q59] 分组内累计
来源：http://mv.nicolike.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ak.bjjhwx.cn

[Q60] 取上一行 / 下一行
来源：http://dh.colortex.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://zy.hnjuh.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://fu.panjiajie.cn

[Q61] 移动平均
来源：http://yp.nicolike.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://bi.muxihuayi.cn

[Q62] 分组占比
来源：http://fu.jianghongdianzi.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wu.haigaiapp.cn

[Q63] 开启事务
来源：http://pz.wgjwhj.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://vq.colortex.cn

[Q64] 提交事务
来源：http://or.nicolike.cn

COMMIT;
来源：http://tl.hahajie.cn

[Q65] 回滚事务
来源：http://sy.jctech888.com.cn

ROLLBACK;
来源：http://rg.muxihuayi.cn

[Q66] 行锁查询
来源：http://np.muxihuayi.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mh.newstarts.cn

[Q67] 设置隔离级别
来源：http://ny.huixiangedu.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://po.jianghongdianzi.cn

[Q68] 保存点
来源：http://om.jctech888.com.cn

SAVEPOINT sp1;
来源：http://si.panjiajie.cn

ROLLBACK TO sp1;
来源：http://rp.huanxung.cn

[Q69] 查看执行计划
来源：http://ay.shtwfgs.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ou.shxzukj.cn

[Q70] 更新统计信息
来源：http://oh.nszjky.cn

ANALYZE TABLE users;
来源：http://hy.huixinmuqiang.cn

[Q71] 查看建表语句
来源：http://zu.haigaiapp.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://kh.haigaiapp.cn

[Q72] 查看索引
来源：http://hm.muxihuayi.cn

SHOW INDEX FROM users;
来源：http://ch.colortex.cn

[Q73] 查看表状态
来源：http://tx.shxzskj.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://sh.lnxyls.cn

[Q74] 强制使用索引
来源：http://mq.szxytkj.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://qh.haigaiapp.cn

[Q75] 日期格式化
来源：http://zk.shxzukj.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wt.hahajie.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ej.chemitech.net.cn

[Q76] 按天统计
来源：http://yg.bookmarksfly.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://xj.lnxyls.cn

[Q77] 时间加减
来源：http://fl.lnxyls.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://or.shxzukj.cn

[Q78] 当前时间
来源：http://ry.huixiangedu.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://oo.haigaiapp.cn

[Q79] 字符串拼接
来源：http://mk.szxytkj.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://li.yuexingan06.cn

[Q80] 字符串截取
来源：http://tw.hnjuh.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://qu.hnjuh.cn

[Q81] 字符串替换
来源：http://jn.szxytkj.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://dg.bookmarksfly.cn

[Q82] 字符长度与字节长度
来源：http://ay.hnjuh.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ct.9csxet.cn

[Q83] 大小写转换
来源：http://ao.colortex.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://pk.asd995.cn

[Q84] 去除首尾空格
来源：http://cx.yuntaijiaju.cn

SELECT TRIM(name) FROM users;
来源：http://sn.jianghongdianzi.cn

[Q85] 数值取整
来源：http://bs.nszjky.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ww.chemitech.net.cn

[Q86] 读取 JSON 字段
来源：http://hd.hahajie.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://nq.panjiajie.cn

[Q87] JSON 字段做条件
来源：http://wy.szsharing.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://nd.jctech888.com.cn

[Q88] 行转列（条件聚合）
来源：http://dr.9csxet.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mq.szxytkj.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://zy.hnjuh.cn

[Q89] 判断表是否存在
来源：http://yy.jctech888.com.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wu.shxzukj.cn

[Q90] 生成序号列
来源：http://xz.jianghongdianzi.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://aw.muxihuayi.cn

================================================================================
来源：http://qz.nicolike.cn

R. Bash 专题
来源：http://jj.huanxung.cn

================================================================================
来源：http://bf.hahajie.cn

[R01] shebang 与严格模式
来源：http://pv.bookmarksfly.cn

#!/usr/bin/env bash
来源：http://mf.hnjuh.cn

set -euo pipefail
来源：http://ou.huixinmuqiang.cn

[R02] 变量赋值与使用
来源：http://cq.newstarts.cn

name="Tom"; echo "$name"
来源：http://ij.colortex.cn

[R03] 只读变量
来源：http://ah.521024.cn

readonly PI=3.14
来源：http://ff.9csxet.cn

[R04] 位置参数
来源：http://xi.jianghongdianzi.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ud.nicolike.cn

[R05] 参数默认值
来源：http://nx.wgjwhj.cn

name="${1:-default}"
来源：http://ie.jianghongdianzi.cn

[R06] 判断命令是否存在
来源：http://fu.muxihuayi.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://eh.huixinmuqiang.cn

[R07] if 判断文件
来源：http://pw.huanxung.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://so.asd995.cn

[R08] 数值比较
来源：http://jd.colortex.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://og.newstarts.cn

[R09] 字符串比较
来源：http://os.huixinmuqiang.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://gb.colortex.cn

[R10] 正则匹配
来源：http://iq.wgjwhj.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mv.521024.cn

[R11] case 多分支
来源：http://pp.521024.cn

case "$1" in
来源：http://ay.nicolike.cn

start) echo "启动" ;;
来源：http://fc.9csxet.cn

stop)  echo "停止" ;;
来源：http://cv.haigaiapp.cn

*)     echo "未知命令" ;;
来源：http://eq.szxytkj.cn

esac
来源：http://dy.yuexingan06.cn

[R12] for 遍历文件
来源：http://ky.9csxet.cn

for f in *.txt; do echo "$f"; done
来源：http://hx.hahajie.cn

[R13] for 计数循环
来源：http://sj.lnxyls.cn

for i in {1..10}; do echo "$i"; done
来源：http://gu.muxihuayi.cn

[R14] C 风格 for
来源：http://ki.gzmigu.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://xi.huixinmuqiang.cn

[R15] while 逐行读文件
来源：http://yt.colortex.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ts.asd995.cn

[R16] until 等待条件
来源：http://rx.szsharing.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://zr.szxytkj.cn

[R17] 数组定义与取值
来源：http://hi.huixiangedu.cn

arr=(a b c); echo "${arr[0]}"
来源：http://mg.nszjky.cn

[R18] 遍历数组
来源：http://oc.shxzukj.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://gn.colortex.cn

[R19] 数组长度
来源：http://wk.bjjhwx.cn

echo "${#arr[@]}"
来源：http://zi.szsharing.cn

[R20] 关联数组（字典）
来源：http://ui.shtwfgs.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://vb.jianghongdianzi.cn

[R21] 字符串长度
来源：http://xe.bookmarksfly.cn

echo "${#s}"
来源：http://hx.shtwfgs.cn

[R22] 截取子串
来源：http://xj.lnxyls.cn

echo "${s:0:5}"
来源：http://rs.521024.cn

[R23] 字符串替换
来源：http://dr.nszjky.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ez.shxzukj.cn

[R24] 大小写转换
来源：http://vx.chemitech.net.cn

echo "${s^^}"; echo "${s,,}"
来源：http://ul.panjiajie.cn

[R25] 去后缀 / 去前缀
来源：http://gr.nszjky.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://zb.yuexingan06.cn

[R26] 命令替换
来源：http://tv.nicolike.cn

now=$(date +%F); echo "$now"
来源：http://po.colortex.cn

[R27] 算术展开
来源：http://po.jianghongdianzi.cn

echo $((1 + 2 * 3))
来源：http://ds.9csxet.cn

[R28] 浮点运算
来源：http://md.bookmarksfly.cn

echo "scale=2; 10/3" | bc
来源：http://vt.9csxet.cn

[R29] 定义函数
来源：http://dm.nicolike.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://yv.hahajie.cn

[R30] 函数返回状态码
来源：http://fr.nicolike.cn

f() { return 0; }; f || echo "失败了"
来源：http://dx.521024.cn

[R31] 局部变量
来源：http://dk.521024.cn

f() { local x=1; echo "$x"; }
来源：http://fd.muxihuayi.cn

[R32] 参数个数校验
来源：http://nd.szxytkj.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://kz.shxzskj.cn

[R33] 捕获错误并提示行号
来源：http://ih.szxytkj.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://tg.newstarts.cn

[R34] 退出时清理
来源：http://ur.bookmarksfly.cn

trap 'rm -f "$tmp"' EXIT
来源：http://vr.9csxet.cn

[R35] 后台执行并等待
来源：http://zn.gzmigu.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://bg.wgjwhj.cn

[R36] 并发执行多个任务
来源：http://sv.bjjhwx.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://my.shtwfgs.cn

[R37] 把输出赋给变量
来源：http://um.521024.cn

files=$(ls -1)
来源：http://ww.shxzukj.cn

[R38] 管道串联
来源：http://eb.jctech888.com.cn

cat a.txt | grep -i error | wc -l
来源：http://ye.521024.cn

[R39] 重定向标准输出与错误
来源：http://xu.gzmigu.cn

cmd > out.log 2>&1
来源：http://zt.nicolike.cn

[R40] 追加写日志
来源：http://pu.jctech888.com.cn

echo "log" >> out.log
来源：http://pc.hahajie.cn

[R41] 丢弃输出
来源：http://ra.huixiangedu.cn

cmd >/dev/null 2>&1
来源：http://kh.shxzskj.cn

[R42] 输入重定向
来源：http://lg.huixinmuqiang.cn

wc -l < a.txt
来源：http://qd.chemitech.net.cn

[R43] 按名字查找文件
来源：http://su.asd995.cn


<!-- 参考信息 -->