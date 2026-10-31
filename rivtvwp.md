代发 wailian999

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://tz.hnjuh.cn

);
来源：http://xn.gzmigu.cn

[Q02] 创建带外键的表
来源：http://fa.hnjuh.cn

CREATE TABLE orders (
来源：http://cv.haigaiapp.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ud.newstarts.cn

user_id INT NOT NULL,
来源：http://ho.shxzukj.cn

amount DECIMAL(10, 2),
来源：http://in.colortex.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ns.szxytkj.cn

);
来源：http://wr.haigaiapp.cn

[Q03] 增加列
来源：http://ec.szsharing.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://pg.szxytkj.cn

[Q04] 修改列类型
来源：http://oh.szsharing.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://dh.yuntaijiaju.cn

[Q05] 重命名列
来源：http://vk.shxzukj.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://id.huixinmuqiang.cn

[Q06] 删除列
来源：http://lx.chemitech.net.cn

ALTER TABLE users DROP COLUMN age;
来源：http://kl.shtwfgs.cn

[Q07] 删除表
来源：http://iu.jctech888.com.cn

DROP TABLE IF EXISTS orders;
来源：http://te.jctech888.com.cn

[Q08] 创建普通索引
来源：http://wz.nszjky.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://kr.shtwfgs.cn

[Q09] 创建唯一索引
来源：http://hi.shxzukj.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://dg.chemitech.net.cn

[Q10] 插入单行
来源：http://py.asd995.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ol.huanxung.cn

[Q11] 一次插入多行
来源：http://bc.chemitech.net.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://br.hahajie.cn

[Q12] 插入后取自增 ID
来源：http://nk.shxzskj.cn

INSERT INTO users (name) VALUES ('C');
来源：http://ow.jctech888.com.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://qk.shxzskj.cn

[Q13] 忽略重复插入
来源：http://ja.huixinmuqiang.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://gk.521024.cn

[Q14] 存在则更新（upsert）
来源：http://ix.wgjwhj.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ye.huixinmuqiang.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://gt.hahajie.cn

[Q15] 查询全部
来源：http://fg.hnjuh.cn

SELECT * FROM users;
来源：http://cx.nicolike.cn

[Q16] 查询指定列
来源：http://cb.muxihuayi.cn

SELECT id, name FROM users;
来源：http://ap.yuntaijiaju.cn

[Q17] 条件查询
来源：http://ng.9csxet.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://af.shtwfgs.cn

[Q18] 模糊匹配
来源：http://zk.9csxet.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://pw.shxzskj.cn

[Q19] 范围查询
来源：http://pj.panjiajie.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://cl.colortex.cn

[Q20] IN 列表
来源：http://ba.nszjky.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wk.panjiajie.cn

[Q21] 空值判断
来源：http://qo.521024.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://fr.szxytkj.cn

[Q22] 排序
来源：http://er.jianghongdianzi.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://xz.gzmigu.cn

[Q23] 分页
来源：http://fk.muxihuayi.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ah.szxytkj.cn

[Q24] 去重
来源：http://tw.521024.cn

SELECT DISTINCT city FROM users;
来源：http://tf.nszjky.cn

[Q25] 只取前 N 条
来源：http://dh.huixiangedu.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://lb.newstarts.cn

[Q26] 计数
来源：http://rd.jctech888.com.cn

SELECT COUNT(*) FROM users;
来源：http://tz.gzmigu.cn

[Q27] 条件计数
来源：http://hb.jianghongdianzi.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ko.bookmarksfly.cn

[Q28] 求和与平均
来源：http://vd.yuexingan06.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://xq.jctech888.com.cn

[Q29] 最大最小值
来源：http://hx.szsharing.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://kp.yuntaijiaju.cn

[Q30] 分组统计
来源：http://pv.hahajie.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://kg.jianghongdianzi.cn

[Q31] 分组后过滤
来源：http://xm.521024.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://pf.bookmarksfly.cn

[Q32] 分组拼接字符串
来源：http://tr.panjiajie.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://rm.gzmigu.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ic.yuntaijiaju.cn

[Q33] 多列分组
来源：http://dw.jctech888.com.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://si.huanxung.cn

[Q34] 每组取第一条
来源：http://bc.521024.cn

SELECT * FROM (
来源：http://tn.yuntaijiaju.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://lt.521024.cn

) t WHERE rn = 1;
来源：http://vi.bjjhwx.cn

[Q35] 内连接
来源：http://br.9csxet.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mq.huixiangedu.cn

[Q36] 左连接
来源：http://pr.9csxet.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://sv.szsharing.cn

[Q37] 右连接
来源：http://ux.huixinmuqiang.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://og.hahajie.cn

[Q38] 全外连接（PostgreSQL）
来源：http://bn.huixiangedu.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://uf.yuexingan06.cn

[Q39] 自连接（查上下级）
来源：http://vh.hahajie.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://sz.jctech888.com.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ba.shxzukj.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://lm.shxzukj.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://gj.jctech888.com.cn

[Q41] 多表连接
来源：http://el.szxytkj.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://zq.huixinmuqiang.cn

JOIN users u ON u.id = o.user_id
来源：http://jd.haigaiapp.cn

JOIN products p ON p.id = o.product_id;
来源：http://jw.huixiangedu.cn

[Q42] 连接条件附加过滤
来源：http://it.szsharing.cn

SELECT u.name, o.amount FROM users u
来源：http://nf.haigaiapp.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://tw.muxihuayi.cn

[Q43] 标量子查询
来源：http://oi.haigaiapp.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://jc.muxihuayi.cn

[Q44] IN 子查询
来源：http://jg.nszjky.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://yr.jctech888.com.cn

[Q45] EXISTS 判断存在
来源：http://gi.9csxet.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://rd.colortex.cn

[Q46] NOT EXISTS 判断不存在
来源：http://nf.shtwfgs.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ts.9csxet.cn

[Q47] 与平均值比较
来源：http://xq.521024.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://fa.shxzukj.cn

[Q48] CTE 公用表表达式
来源：http://zf.hahajie.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://jl.lnxyls.cn

SELECT * FROM t WHERE c > 5;
来源：http://lx.jctech888.com.cn

[Q49] 更新单行
来源：http://oi.hnjuh.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://zy.szsharing.cn

[Q50] 批量更新
来源：http://to.shxzskj.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://rn.wgjwhj.cn

[Q51] 用子查询更新
来源：http://uc.nicolike.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hc.szxytkj.cn

[Q52] 删除指定行
来源：http://bp.521024.cn

DELETE FROM users WHERE id = 10;
来源：http://wu.gzmigu.cn

[Q53] 按条件删除
来源：http://fh.shtwfgs.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://fz.9csxet.cn

[Q54] 清空表
来源：http://dl.newstarts.cn

TRUNCATE TABLE logs;
来源：http://wt.bjjhwx.cn

[Q55] 排名（并列占位）
来源：http://ty.newstarts.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://at.muxihuayi.cn

[Q56] 密集排名（并列不占位）
来源：http://mt.shtwfgs.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://bz.shxzukj.cn

[Q57] 行号
来源：http://ev.szxytkj.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://xr.wgjwhj.cn

[Q58] 累计求和
来源：http://zq.bjjhwx.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://lw.nicolike.cn

[Q59] 分组内累计
来源：http://zl.huixinmuqiang.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ie.haigaiapp.cn

[Q60] 取上一行 / 下一行
来源：http://oc.colortex.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mi.muxihuayi.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://pe.shxzukj.cn

[Q61] 移动平均
来源：http://mv.szsharing.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mc.nicolike.cn

[Q62] 分组占比
来源：http://mc.bookmarksfly.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ra.szxytkj.cn

[Q63] 开启事务
来源：http://eu.nszjky.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://er.newstarts.cn

[Q64] 提交事务
来源：http://bh.yuntaijiaju.cn

COMMIT;
来源：http://wg.nszjky.cn

[Q65] 回滚事务
来源：http://yz.shtwfgs.cn

ROLLBACK;
来源：http://qu.bjjhwx.cn

[Q66] 行锁查询
来源：http://sd.szxytkj.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mh.521024.cn

[Q67] 设置隔离级别
来源：http://nl.newstarts.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://yn.jctech888.com.cn

[Q68] 保存点
来源：http://yy.shtwfgs.cn

SAVEPOINT sp1;
来源：http://iu.huixinmuqiang.cn

ROLLBACK TO sp1;
来源：http://sf.yuexingan06.cn

[Q69] 查看执行计划
来源：http://jx.szsharing.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ov.colortex.cn

[Q70] 更新统计信息
来源：http://vz.panjiajie.cn

ANALYZE TABLE users;
来源：http://hw.yuntaijiaju.cn

[Q71] 查看建表语句
来源：http://as.shxzukj.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://vx.huanxung.cn

[Q72] 查看索引
来源：http://be.hnjuh.cn

SHOW INDEX FROM users;
来源：http://cm.shxzskj.cn

[Q73] 查看表状态
来源：http://uk.nszjky.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://wp.gzmigu.cn

[Q74] 强制使用索引
来源：http://un.szxytkj.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hi.huixiangedu.cn

[Q75] 日期格式化
来源：http://hh.yuexingan06.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mb.yuexingan06.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ph.521024.cn

[Q76] 按天统计
来源：http://yb.szsharing.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://qw.shxzskj.cn

[Q77] 时间加减
来源：http://fq.newstarts.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ef.huixinmuqiang.cn

[Q78] 当前时间
来源：http://bm.yuexingan06.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://vs.jctech888.com.cn

[Q79] 字符串拼接
来源：http://lr.chemitech.net.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://li.521024.cn

[Q80] 字符串截取
来源：http://bx.hnjuh.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://qx.szsharing.cn

[Q81] 字符串替换
来源：http://og.bjjhwx.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mg.hnjuh.cn

[Q82] 字符长度与字节长度
来源：http://oe.yuexingan06.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://lz.muxihuayi.cn

[Q83] 大小写转换
来源：http://pk.wgjwhj.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://xn.szsharing.cn

[Q84] 去除首尾空格
来源：http://hx.bookmarksfly.cn

SELECT TRIM(name) FROM users;
来源：http://wv.haigaiapp.cn

[Q85] 数值取整
来源：http://de.nszjky.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://zo.521024.cn

[Q86] 读取 JSON 字段
来源：http://ha.9csxet.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://rk.jianghongdianzi.cn

[Q87] JSON 字段做条件
来源：http://ax.haigaiapp.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://kx.chemitech.net.cn

[Q88] 行转列（条件聚合）
来源：http://wc.nicolike.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ig.panjiajie.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://pp.hahajie.cn

[Q89] 判断表是否存在
来源：http://rf.szsharing.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ky.shxzukj.cn

[Q90] 生成序号列
来源：http://nk.shtwfgs.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://xo.gzmigu.cn

================================================================================
来源：http://rc.huixinmuqiang.cn

R. Bash 专题
来源：http://fl.gzmigu.cn

================================================================================
来源：http://vc.nszjky.cn

[R01] shebang 与严格模式
来源：http://ok.asd995.cn

#!/usr/bin/env bash
来源：http://pu.szxytkj.cn

set -euo pipefail
来源：http://th.lnxyls.cn

[R02] 变量赋值与使用
来源：http://jk.shxzskj.cn

name="Tom"; echo "$name"
来源：http://xm.nszjky.cn

[R03] 只读变量
来源：http://gw.lnxyls.cn

readonly PI=3.14
来源：http://xg.chemitech.net.cn

[R04] 位置参数
来源：http://dl.haigaiapp.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://eq.bjjhwx.cn

[R05] 参数默认值
来源：http://aa.huixiangedu.cn

name="${1:-default}"
来源：http://yd.panjiajie.cn

[R06] 判断命令是否存在
来源：http://nt.bookmarksfly.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://vb.wgjwhj.cn

[R07] if 判断文件
来源：http://ta.shtwfgs.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mz.yuexingan06.cn

[R08] 数值比较
来源：http://om.panjiajie.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://ut.bjjhwx.cn

[R09] 字符串比较
来源：http://ng.hahajie.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://nw.shxzukj.cn

[R10] 正则匹配
来源：http://na.szxytkj.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mk.wgjwhj.cn

[R11] case 多分支
来源：http://kf.shxzskj.cn

case "$1" in
来源：http://pd.yuexingan06.cn

start) echo "启动" ;;
来源：http://dr.jctech888.com.cn

stop)  echo "停止" ;;
来源：http://rb.colortex.cn

*)     echo "未知命令" ;;
来源：http://ei.wgjwhj.cn

esac
来源：http://ej.nszjky.cn

[R12] for 遍历文件
来源：http://zj.yuexingan06.cn

for f in *.txt; do echo "$f"; done
来源：http://wo.huixiangedu.cn

[R13] for 计数循环
来源：http://mt.yuntaijiaju.cn

for i in {1..10}; do echo "$i"; done
来源：http://ol.asd995.cn

[R14] C 风格 for
来源：http://qv.521024.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://gx.hnjuh.cn

[R15] while 逐行读文件
来源：http://dx.haigaiapp.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ae.gzmigu.cn

[R16] until 等待条件
来源：http://as.9csxet.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ce.lnxyls.cn

[R17] 数组定义与取值
来源：http://ql.wgjwhj.cn

arr=(a b c); echo "${arr[0]}"
来源：http://gt.hnjuh.cn

[R18] 遍历数组
来源：http://fu.haigaiapp.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://qh.huixiangedu.cn

[R19] 数组长度
来源：http://qw.nszjky.cn

echo "${#arr[@]}"
来源：http://wy.huanxung.cn

[R20] 关联数组（字典）
来源：http://sh.hnjuh.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://yk.huanxung.cn

[R21] 字符串长度
来源：http://nd.chemitech.net.cn

echo "${#s}"
来源：http://zn.panjiajie.cn

[R22] 截取子串
来源：http://zy.521024.cn

echo "${s:0:5}"
来源：http://yo.shxzskj.cn

[R23] 字符串替换
来源：http://jl.hahajie.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://xp.haigaiapp.cn

[R24] 大小写转换
来源：http://jj.huixinmuqiang.cn

echo "${s^^}"; echo "${s,,}"
来源：http://rc.bjjhwx.cn

[R25] 去后缀 / 去前缀
来源：http://sy.nicolike.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://hc.hahajie.cn

[R26] 命令替换
来源：http://xx.yuntaijiaju.cn

now=$(date +%F); echo "$now"
来源：http://bq.bjjhwx.cn

[R27] 算术展开
来源：http://dk.huanxung.cn

echo $((1 + 2 * 3))
来源：http://jd.yuexingan06.cn

[R28] 浮点运算
来源：http://uk.hahajie.cn

echo "scale=2; 10/3" | bc
来源：http://nq.nszjky.cn

[R29] 定义函数
来源：http://jl.shxzskj.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://bb.colortex.cn

[R30] 函数返回状态码
来源：http://dh.panjiajie.cn

f() { return 0; }; f || echo "失败了"
来源：http://cv.panjiajie.cn

[R31] 局部变量
来源：http://zn.9csxet.cn

f() { local x=1; echo "$x"; }
来源：http://md.wgjwhj.cn

[R32] 参数个数校验
来源：http://zo.shxzskj.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://sh.hahajie.cn

[R33] 捕获错误并提示行号
来源：http://jh.asd995.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ok.bjjhwx.cn

[R34] 退出时清理
来源：http://vt.shxzskj.cn

trap 'rm -f "$tmp"' EXIT
来源：http://zg.asd995.cn

[R35] 后台执行并等待
来源：http://ao.bjjhwx.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://qg.9csxet.cn

[R36] 并发执行多个任务
来源：http://nl.newstarts.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://sa.shtwfgs.cn

[R37] 把输出赋给变量
来源：http://fb.jctech888.com.cn

files=$(ls -1)
来源：http://ec.asd995.cn

[R38] 管道串联
来源：http://ps.bjjhwx.cn

cat a.txt | grep -i error | wc -l
来源：http://dr.szsharing.cn

[R39] 重定向标准输出与错误
来源：http://ba.wgjwhj.cn

cmd > out.log 2>&1
来源：http://ut.9csxet.cn

[R40] 追加写日志
来源：http://fe.shxzukj.cn

echo "log" >> out.log
来源：http://pe.muxihuayi.cn

[R41] 丢弃输出
来源：http://ca.haigaiapp.cn

cmd >/dev/null 2>&1
来源：http://tp.jianghongdianzi.cn

[R42] 输入重定向
来源：http://da.bjjhwx.cn

wc -l < a.txt
来源：http://vf.asd995.cn

[R43] 按名字查找文件
来源：http://ar.hnjuh.cn

find . -name "*.log" -type f
来源：http://ka.shtwfgs.cn

[R44] 按修改时间查找
来源：http://lk.521024.cn

find . -mtime -7 -type f
来源：http://ng.szxytkj.cn

[R45] 批量删除
来源：http://qd.nszjky.cn

find . -name "*.tmp" -delete
来源：http://nu.huixinmuqiang.cn

[R46] 递归替换文件内容
来源：http://ce.9csxet.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://dl.hahajie.cn

[R47] sed 单行替换
来源：http://ms.hahajie.cn


<!-- 参考信息 -->