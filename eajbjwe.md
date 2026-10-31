代发 wailian999

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://zq.lnxyls.cn

);
来源：http://tv.szxytkj.cn

[Q02] 创建带外键的表
来源：http://hr.muxihuayi.cn

CREATE TABLE orders (
来源：http://px.colortex.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ww.szxytkj.cn

user_id INT NOT NULL,
来源：http://ba.lnxyls.cn

amount DECIMAL(10, 2),
来源：http://ki.jctech888.com.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://tw.jctech888.com.cn

);
来源：http://mo.chemitech.net.cn

[Q03] 增加列
来源：http://qy.lnxyls.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://dy.wgjwhj.cn

[Q04] 修改列类型
来源：http://qh.szxytkj.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ud.shxzukj.cn

[Q05] 重命名列
来源：http://hn.shxzskj.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hx.jianghongdianzi.cn

[Q06] 删除列
来源：http://or.521024.cn

ALTER TABLE users DROP COLUMN age;
来源：http://ej.haigaiapp.cn

[Q07] 删除表
来源：http://ch.huixiangedu.cn

DROP TABLE IF EXISTS orders;
来源：http://hg.yuntaijiaju.cn

[Q08] 创建普通索引
来源：http://th.shxzskj.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://mt.muxihuayi.cn

[Q09] 创建唯一索引
来源：http://hh.jctech888.com.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ph.huanxung.cn

[Q10] 插入单行
来源：http://bt.szxytkj.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://nl.huixiangedu.cn

[Q11] 一次插入多行
来源：http://fk.shxzukj.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://yh.muxihuayi.cn

[Q12] 插入后取自增 ID
来源：http://ku.lnxyls.cn

INSERT INTO users (name) VALUES ('C');
来源：http://ma.yuntaijiaju.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://st.nszjky.cn

[Q13] 忽略重复插入
来源：http://hf.jianghongdianzi.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://cv.yuntaijiaju.cn

[Q14] 存在则更新（upsert）
来源：http://li.yuexingan06.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://pj.huanxung.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ga.gzmigu.cn

[Q15] 查询全部
来源：http://er.nicolike.cn

SELECT * FROM users;
来源：http://zj.bookmarksfly.cn

[Q16] 查询指定列
来源：http://lf.shxzukj.cn

SELECT id, name FROM users;
来源：http://yk.chemitech.net.cn

[Q17] 条件查询
来源：http://nx.yuntaijiaju.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://dc.haigaiapp.cn

[Q18] 模糊匹配
来源：http://vf.haigaiapp.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://vu.jianghongdianzi.cn

[Q19] 范围查询
来源：http://ub.colortex.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://pq.haigaiapp.cn

[Q20] IN 列表
来源：http://ad.huixiangedu.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://sp.hnjuh.cn

[Q21] 空值判断
来源：http://lo.jianghongdianzi.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://jp.bookmarksfly.cn

[Q22] 排序
来源：http://rk.nicolike.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://gs.asd995.cn

[Q23] 分页
来源：http://wt.huixinmuqiang.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ay.hnjuh.cn

[Q24] 去重
来源：http://cy.colortex.cn

SELECT DISTINCT city FROM users;
来源：http://un.jctech888.com.cn

[Q25] 只取前 N 条
来源：http://so.hnjuh.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://my.newstarts.cn

[Q26] 计数
来源：http://wv.nszjky.cn

SELECT COUNT(*) FROM users;
来源：http://zg.9csxet.cn

[Q27] 条件计数
来源：http://in.hnjuh.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://md.huixinmuqiang.cn

[Q28] 求和与平均
来源：http://ao.newstarts.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://ac.asd995.cn

[Q29] 最大最小值
来源：http://qk.huixiangedu.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://zt.haigaiapp.cn

[Q30] 分组统计
来源：http://xc.colortex.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://cq.hnjuh.cn

[Q31] 分组后过滤
来源：http://kp.yuexingan06.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://lw.nicolike.cn

[Q32] 分组拼接字符串
来源：http://st.asd995.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://fn.wgjwhj.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://vv.lnxyls.cn

[Q33] 多列分组
来源：http://jz.chemitech.net.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ow.jianghongdianzi.cn

[Q34] 每组取第一条
来源：http://cz.gzmigu.cn

SELECT * FROM (
来源：http://vy.521024.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mi.newstarts.cn

) t WHERE rn = 1;
来源：http://xq.yuntaijiaju.cn

[Q35] 内连接
来源：http://ys.jctech888.com.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://cp.wgjwhj.cn

[Q36] 左连接
来源：http://su.nszjky.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://lh.shtwfgs.cn

[Q37] 右连接
来源：http://he.haigaiapp.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://vi.szsharing.cn

[Q38] 全外连接（PostgreSQL）
来源：http://sg.bjjhwx.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://fg.huixiangedu.cn

[Q39] 自连接（查上下级）
来源：http://ru.szsharing.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://lf.panjiajie.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://in.nszjky.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://jh.bjjhwx.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://iw.chemitech.net.cn

[Q41] 多表连接
来源：http://eg.colortex.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://wb.shxzukj.cn

JOIN users u ON u.id = o.user_id
来源：http://ve.gzmigu.cn

JOIN products p ON p.id = o.product_id;
来源：http://cq.newstarts.cn

[Q42] 连接条件附加过滤
来源：http://ry.hahajie.cn

SELECT u.name, o.amount FROM users u
来源：http://lz.huixiangedu.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://fy.wgjwhj.cn

[Q43] 标量子查询
来源：http://xy.hnjuh.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://ut.colortex.cn

[Q44] IN 子查询
来源：http://xi.huixiangedu.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://qk.wgjwhj.cn

[Q45] EXISTS 判断存在
来源：http://cg.haigaiapp.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://et.yuexingan06.cn

[Q46] NOT EXISTS 判断不存在
来源：http://cn.haigaiapp.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://so.yuexingan06.cn

[Q47] 与平均值比较
来源：http://gq.newstarts.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://we.haigaiapp.cn

[Q48] CTE 公用表表达式
来源：http://px.huixinmuqiang.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ib.panjiajie.cn

SELECT * FROM t WHERE c > 5;
来源：http://wl.bjjhwx.cn

[Q49] 更新单行
来源：http://oe.nicolike.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://li.asd995.cn

[Q50] 批量更新
来源：http://rd.521024.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://gy.huixiangedu.cn

[Q51] 用子查询更新
来源：http://zu.shxzukj.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mf.jianghongdianzi.cn

[Q52] 删除指定行
来源：http://oi.lnxyls.cn

DELETE FROM users WHERE id = 10;
来源：http://ub.huixinmuqiang.cn

[Q53] 按条件删除
来源：http://vu.nszjky.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://af.nicolike.cn

[Q54] 清空表
来源：http://lm.wgjwhj.cn

TRUNCATE TABLE logs;
来源：http://rq.gzmigu.cn

[Q55] 排名（并列占位）
来源：http://ql.bjjhwx.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://rv.hnjuh.cn

[Q56] 密集排名（并列不占位）
来源：http://yw.huixinmuqiang.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://iy.huixinmuqiang.cn

[Q57] 行号
来源：http://fc.shtwfgs.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://oj.asd995.cn

[Q58] 累计求和
来源：http://dh.szxytkj.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://av.muxihuayi.cn

[Q59] 分组内累计
来源：http://cj.lnxyls.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ke.asd995.cn

[Q60] 取上一行 / 下一行
来源：http://tl.nszjky.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://to.colortex.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wk.nszjky.cn

[Q61] 移动平均
来源：http://ch.yuexingan06.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://oa.lnxyls.cn

[Q62] 分组占比
来源：http://jj.panjiajie.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://rh.haigaiapp.cn

[Q63] 开启事务
来源：http://gw.bjjhwx.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://tr.asd995.cn

[Q64] 提交事务
来源：http://je.chemitech.net.cn

COMMIT;
来源：http://ey.bookmarksfly.cn

[Q65] 回滚事务
来源：http://as.jctech888.com.cn

ROLLBACK;
来源：http://rb.9csxet.cn

[Q66] 行锁查询
来源：http://se.521024.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://tv.chemitech.net.cn

[Q67] 设置隔离级别
来源：http://px.wgjwhj.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://xf.szsharing.cn

[Q68] 保存点
来源：http://ga.bookmarksfly.cn

SAVEPOINT sp1;
来源：http://fc.yuexingan06.cn

ROLLBACK TO sp1;
来源：http://wh.huixiangedu.cn

[Q69] 查看执行计划
来源：http://vb.lnxyls.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ds.asd995.cn

[Q70] 更新统计信息
来源：http://wy.nicolike.cn

ANALYZE TABLE users;
来源：http://lt.yuntaijiaju.cn

[Q71] 查看建表语句
来源：http://cw.muxihuayi.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://sz.haigaiapp.cn

[Q72] 查看索引
来源：http://hu.jianghongdianzi.cn

SHOW INDEX FROM users;
来源：http://ty.nicolike.cn

[Q73] 查看表状态
来源：http://eu.szsharing.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://ir.shtwfgs.cn

[Q74] 强制使用索引
来源：http://if.yuntaijiaju.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://tq.panjiajie.cn

[Q75] 日期格式化
来源：http://wf.9csxet.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://so.9csxet.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mn.lnxyls.cn

[Q76] 按天统计
来源：http://vm.hahajie.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wp.haigaiapp.cn

[Q77] 时间加减
来源：http://yr.9csxet.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://cm.yuntaijiaju.cn

[Q78] 当前时间
来源：http://ly.bjjhwx.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://vu.yuexingan06.cn

[Q79] 字符串拼接
来源：http://pa.szxytkj.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://cq.muxihuayi.cn

[Q80] 字符串截取
来源：http://mv.gzmigu.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://yt.9csxet.cn

[Q81] 字符串替换
来源：http://lc.nszjky.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://vs.szxytkj.cn

[Q82] 字符长度与字节长度
来源：http://jt.yuexingan06.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ty.hnjuh.cn

[Q83] 大小写转换
来源：http://vd.nicolike.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ej.jctech888.com.cn

[Q84] 去除首尾空格
来源：http://gl.bjjhwx.cn

SELECT TRIM(name) FROM users;
来源：http://jj.chemitech.net.cn

[Q85] 数值取整
来源：http://xr.shtwfgs.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ue.muxihuayi.cn

[Q86] 读取 JSON 字段
来源：http://jy.yuntaijiaju.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://bz.huanxung.cn

[Q87] JSON 字段做条件
来源：http://vz.szsharing.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wi.szsharing.cn

[Q88] 行转列（条件聚合）
来源：http://mr.shxzskj.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ms.huixiangedu.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hr.yuexingan06.cn

[Q89] 判断表是否存在
来源：http://tm.nszjky.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://jk.szsharing.cn

[Q90] 生成序号列
来源：http://ni.panjiajie.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://fu.nicolike.cn

================================================================================
来源：http://kb.nszjky.cn

R. Bash 专题
来源：http://bq.chemitech.net.cn

================================================================================
来源：http://cu.jianghongdianzi.cn

[R01] shebang 与严格模式
来源：http://jp.hahajie.cn

#!/usr/bin/env bash
来源：http://aq.jctech888.com.cn

set -euo pipefail
来源：http://yj.jianghongdianzi.cn

[R02] 变量赋值与使用
来源：http://hu.nicolike.cn

name="Tom"; echo "$name"
来源：http://wf.szsharing.cn

[R03] 只读变量
来源：http://gd.muxihuayi.cn

readonly PI=3.14
来源：http://vy.szsharing.cn

[R04] 位置参数
来源：http://ef.huanxung.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://zl.shxzukj.cn

[R05] 参数默认值
来源：http://la.huixiangedu.cn

name="${1:-default}"
来源：http://ps.haigaiapp.cn

[R06] 判断命令是否存在
来源：http://nn.bookmarksfly.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ut.huixinmuqiang.cn

[R07] if 判断文件
来源：http://rm.gzmigu.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://qd.chemitech.net.cn

[R08] 数值比较
来源：http://cd.521024.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://nb.lnxyls.cn

[R09] 字符串比较
来源：http://ly.yuntaijiaju.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://lk.newstarts.cn

[R10] 正则匹配
来源：http://xj.hahajie.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ka.yuexingan06.cn

[R11] case 多分支
来源：http://av.nicolike.cn

case "$1" in
来源：http://pg.bjjhwx.cn

start) echo "启动" ;;
来源：http://hx.hahajie.cn

stop)  echo "停止" ;;
来源：http://vj.9csxet.cn

*)     echo "未知命令" ;;
来源：http://qa.shtwfgs.cn

esac
来源：http://ia.szxytkj.cn

[R12] for 遍历文件
来源：http://iy.jianghongdianzi.cn

for f in *.txt; do echo "$f"; done
来源：http://xl.szsharing.cn

[R13] for 计数循环
来源：http://zk.521024.cn

for i in {1..10}; do echo "$i"; done
来源：http://yj.9csxet.cn

[R14] C 风格 for
来源：http://fm.huixiangedu.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ix.asd995.cn

[R15] while 逐行读文件
来源：http://ds.hnjuh.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://oy.shxzukj.cn

[R16] until 等待条件
来源：http://cy.colortex.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://yy.szsharing.cn

[R17] 数组定义与取值
来源：http://tb.huanxung.cn

arr=(a b c); echo "${arr[0]}"
来源：http://mi.9csxet.cn

[R18] 遍历数组
来源：http://gn.bjjhwx.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ks.panjiajie.cn

[R19] 数组长度
来源：http://ky.szsharing.cn

echo "${#arr[@]}"
来源：http://hp.wgjwhj.cn

[R20] 关联数组（字典）
来源：http://qc.colortex.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://zm.hnjuh.cn

[R21] 字符串长度
来源：http://cp.lnxyls.cn

echo "${#s}"
来源：http://wq.bjjhwx.cn

[R22] 截取子串
来源：http://oa.muxihuayi.cn

echo "${s:0:5}"
来源：http://zo.szxytkj.cn

[R23] 字符串替换
来源：http://ka.wgjwhj.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://kr.521024.cn

[R24] 大小写转换
来源：http://td.chemitech.net.cn

echo "${s^^}"; echo "${s,,}"
来源：http://rd.hahajie.cn

[R25] 去后缀 / 去前缀
来源：http://vn.chemitech.net.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://sy.asd995.cn

[R26] 命令替换
来源：http://gk.521024.cn

now=$(date +%F); echo "$now"
来源：http://iw.yuntaijiaju.cn

[R27] 算术展开
来源：http://ab.hnjuh.cn

echo $((1 + 2 * 3))
来源：http://ht.haigaiapp.cn

[R28] 浮点运算
来源：http://wy.chemitech.net.cn

echo "scale=2; 10/3" | bc
来源：http://ak.nicolike.cn

[R29] 定义函数
来源：http://wu.lnxyls.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://yp.huixinmuqiang.cn

[R30] 函数返回状态码
来源：http://dr.yuexingan06.cn

f() { return 0; }; f || echo "失败了"
来源：http://su.colortex.cn

[R31] 局部变量
来源：http://pt.yuntaijiaju.cn

f() { local x=1; echo "$x"; }
来源：http://hf.yuntaijiaju.cn

[R32] 参数个数校验
来源：http://pg.jianghongdianzi.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://sh.hahajie.cn

[R33] 捕获错误并提示行号
来源：http://pq.bjjhwx.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wi.szsharing.cn

[R34] 退出时清理
来源：http://jw.lnxyls.cn

trap 'rm -f "$tmp"' EXIT
来源：http://yi.9csxet.cn

[R35] 后台执行并等待
来源：http://vm.szsharing.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://ja.wgjwhj.cn

[R36] 并发执行多个任务
来源：http://tl.521024.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://vt.colortex.cn

[R37] 把输出赋给变量
来源：http://dt.gzmigu.cn

files=$(ls -1)
来源：http://rg.haigaiapp.cn

[R38] 管道串联
来源：http://uz.shxzskj.cn

cat a.txt | grep -i error | wc -l
来源：http://el.jctech888.com.cn

[R39] 重定向标准输出与错误
来源：http://zg.hnjuh.cn

cmd > out.log 2>&1
来源：http://bs.jianghongdianzi.cn

[R40] 追加写日志
来源：http://xl.chemitech.net.cn

echo "log" >> out.log
来源：http://ec.colortex.cn

[R41] 丢弃输出
来源：http://jk.szsharing.cn

cmd >/dev/null 2>&1
来源：http://ps.asd995.cn

[R42] 输入重定向
来源：http://ie.hahajie.cn

wc -l < a.txt
来源：http://iw.jianghongdianzi.cn

[R43] 按名字查找文件
来源：http://zx.shxzskj.cn

find . -name "*.log" -type f
来源：http://ox.shxzskj.cn

[R44] 按修改时间查找
来源：http://as.asd995.cn

find . -mtime -7 -type f
来源：http://jp.muxihuayi.cn

[R45] 批量删除
来源：http://kp.chemitech.net.cn

find . -name "*.tmp" -delete
来源：http://dz.panjiajie.cn

[R46] 递归替换文件内容
来源：http://vr.huixinmuqiang.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://re.gzmigu.cn

[R47] sed 单行替换
来源：http://fa.hahajie.cn


<!-- 参考信息 -->