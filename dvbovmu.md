代发 wailian999

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ja.muxihuayi.cn

user_id INT NOT NULL,
来源：http://hd.asd995.cn

amount DECIMAL(10, 2),
来源：http://tz.muxihuayi.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://cp.hahajie.cn

);
来源：http://il.wgjwhj.cn

[Q03] 增加列
来源：http://af.lnxyls.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mx.nszjky.cn

[Q04] 修改列类型
来源：http://er.szsharing.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://fj.newstarts.cn

[Q05] 重命名列
来源：http://xu.shtwfgs.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://li.shxzukj.cn

[Q06] 删除列
来源：http://tz.lnxyls.cn

ALTER TABLE users DROP COLUMN age;
来源：http://sy.nicolike.cn

[Q07] 删除表
来源：http://dx.9csxet.cn

DROP TABLE IF EXISTS orders;
来源：http://mu.asd995.cn

[Q08] 创建普通索引
来源：http://yt.bookmarksfly.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://ta.huanxung.cn

[Q09] 创建唯一索引
来源：http://gs.bjjhwx.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://au.hnjuh.cn

[Q10] 插入单行
来源：http://kl.yuexingan06.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://im.yuntaijiaju.cn

[Q11] 一次插入多行
来源：http://jm.hnjuh.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wg.hnjuh.cn

[Q12] 插入后取自增 ID
来源：http://ry.jianghongdianzi.cn

INSERT INTO users (name) VALUES ('C');
来源：http://dv.521024.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://pj.newstarts.cn

[Q13] 忽略重复插入
来源：http://bs.jctech888.com.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ab.wgjwhj.cn

[Q14] 存在则更新（upsert）
来源：http://ep.newstarts.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ua.huixiangedu.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://vn.9csxet.cn

[Q15] 查询全部
来源：http://gd.521024.cn

SELECT * FROM users;
来源：http://an.chemitech.net.cn

[Q16] 查询指定列
来源：http://zo.yuntaijiaju.cn

SELECT id, name FROM users;
来源：http://dv.wgjwhj.cn

[Q17] 条件查询
来源：http://ew.jctech888.com.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://da.521024.cn

[Q18] 模糊匹配
来源：http://kn.newstarts.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.panjiajie.cn

[Q19] 范围查询
来源：http://pn.szxytkj.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://dc.huixiangedu.cn

[Q20] IN 列表
来源：http://vw.jianghongdianzi.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://jv.hnjuh.cn

[Q21] 空值判断
来源：http://ua.huanxung.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://th.newstarts.cn

[Q22] 排序
来源：http://fc.huixinmuqiang.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ms.huanxung.cn

[Q23] 分页
来源：http://fd.chemitech.net.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://uw.nicolike.cn

[Q24] 去重
来源：http://lz.nszjky.cn

SELECT DISTINCT city FROM users;
来源：http://lr.nicolike.cn

[Q25] 只取前 N 条
来源：http://ob.shxzskj.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mo.huixinmuqiang.cn

[Q26] 计数
来源：http://mn.huixinmuqiang.cn

SELECT COUNT(*) FROM users;
来源：http://va.huixiangedu.cn

[Q27] 条件计数
来源：http://po.wgjwhj.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://va.521024.cn

[Q28] 求和与平均
来源：http://mp.hahajie.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://zg.shtwfgs.cn

[Q29] 最大最小值
来源：http://dc.huanxung.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://hv.colortex.cn

[Q30] 分组统计
来源：http://vs.newstarts.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ji.521024.cn

[Q31] 分组后过滤
来源：http://nq.huanxung.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://eb.bjjhwx.cn

[Q32] 分组拼接字符串
来源：http://ww.9csxet.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://zm.huixiangedu.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://jl.colortex.cn

[Q33] 多列分组
来源：http://rj.jctech888.com.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://yz.panjiajie.cn

[Q34] 每组取第一条
来源：http://eg.9csxet.cn

SELECT * FROM (
来源：http://gm.nszjky.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://bh.newstarts.cn

) t WHERE rn = 1;
来源：http://xb.shtwfgs.cn

[Q35] 内连接
来源：http://kj.wgjwhj.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hi.hnjuh.cn

[Q36] 左连接
来源：http://ye.haigaiapp.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://dy.jctech888.com.cn

[Q37] 右连接
来源：http://iu.haigaiapp.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ki.szsharing.cn

[Q38] 全外连接（PostgreSQL）
来源：http://lx.szxytkj.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://cf.huixinmuqiang.cn

[Q39] 自连接（查上下级）
来源：http://cw.nszjky.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://wl.chemitech.net.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://kx.bjjhwx.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://gp.huixiangedu.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://dj.9csxet.cn

[Q41] 多表连接
来源：http://si.nszjky.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://qm.szsharing.cn

JOIN users u ON u.id = o.user_id
来源：http://hm.yuexingan06.cn

JOIN products p ON p.id = o.product_id;
来源：http://yq.asd995.cn

[Q42] 连接条件附加过滤
来源：http://hd.szxytkj.cn

SELECT u.name, o.amount FROM users u
来源：http://fy.colortex.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://jg.huixiangedu.cn

[Q43] 标量子查询
来源：http://dq.huanxung.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://dd.jianghongdianzi.cn

[Q44] IN 子查询
来源：http://xp.chemitech.net.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://rv.szsharing.cn

[Q45] EXISTS 判断存在
来源：http://mc.szsharing.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://lz.chemitech.net.cn

[Q46] NOT EXISTS 判断不存在
来源：http://le.9csxet.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://zu.lnxyls.cn

[Q47] 与平均值比较
来源：http://vh.chemitech.net.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://vw.muxihuayi.cn

[Q48] CTE 公用表表达式
来源：http://eb.9csxet.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mc.yuntaijiaju.cn

SELECT * FROM t WHERE c > 5;
来源：http://he.521024.cn

[Q49] 更新单行
来源：http://ih.bjjhwx.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ve.9csxet.cn

[Q50] 批量更新
来源：http://qo.lnxyls.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://oc.shxzukj.cn

[Q51] 用子查询更新
来源：http://ez.panjiajie.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://rf.chemitech.net.cn

[Q52] 删除指定行
来源：http://ui.shxzukj.cn

DELETE FROM users WHERE id = 10;
来源：http://az.asd995.cn

[Q53] 按条件删除
来源：http://ue.wgjwhj.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mq.wgjwhj.cn

[Q54] 清空表
来源：http://xh.szsharing.cn

TRUNCATE TABLE logs;
来源：http://el.9csxet.cn

[Q55] 排名（并列占位）
来源：http://wk.hahajie.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://yn.shxzukj.cn

[Q56] 密集排名（并列不占位）
来源：http://rk.9csxet.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://iv.9csxet.cn

[Q57] 行号
来源：http://gr.colortex.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://sc.colortex.cn

[Q58] 累计求和
来源：http://ws.bjjhwx.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ha.nszjky.cn

[Q59] 分组内累计
来源：http://up.jianghongdianzi.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://jt.521024.cn

[Q60] 取上一行 / 下一行
来源：http://ld.jctech888.com.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ag.jianghongdianzi.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://vg.panjiajie.cn

[Q61] 移动平均
来源：http://bf.szxytkj.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://zc.nszjky.cn

[Q62] 分组占比
来源：http://sa.huixinmuqiang.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://de.wgjwhj.cn

[Q63] 开启事务
来源：http://nj.hahajie.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://vs.hnjuh.cn

[Q64] 提交事务
来源：http://hb.jctech888.com.cn

COMMIT;
来源：http://eb.nicolike.cn

[Q65] 回滚事务
来源：http://ul.hahajie.cn

ROLLBACK;
来源：http://iw.521024.cn

[Q66] 行锁查询
来源：http://vj.bookmarksfly.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ki.wgjwhj.cn

[Q67] 设置隔离级别
来源：http://bj.asd995.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ap.nszjky.cn

[Q68] 保存点
来源：http://jn.bjjhwx.cn

SAVEPOINT sp1;
来源：http://uh.szxytkj.cn

ROLLBACK TO sp1;
来源：http://yu.bookmarksfly.cn

[Q69] 查看执行计划
来源：http://cu.wgjwhj.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://qg.szsharing.cn

[Q70] 更新统计信息
来源：http://pv.szsharing.cn

ANALYZE TABLE users;
来源：http://ks.yuntaijiaju.cn

[Q71] 查看建表语句
来源：http://ye.shxzukj.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://io.szsharing.cn

[Q72] 查看索引
来源：http://fc.521024.cn

SHOW INDEX FROM users;
来源：http://vh.chemitech.net.cn

[Q73] 查看表状态
来源：http://dy.wgjwhj.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://bd.bookmarksfly.cn

[Q74] 强制使用索引
来源：http://sp.jianghongdianzi.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://pb.newstarts.cn

[Q75] 日期格式化
来源：http://kc.9csxet.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://jz.szsharing.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hk.9csxet.cn

[Q76] 按天统计
来源：http://eo.9csxet.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://rp.jctech888.com.cn

[Q77] 时间加减
来源：http://qe.haigaiapp.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://pm.shxzukj.cn

[Q78] 当前时间
来源：http://ak.shxzukj.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://im.panjiajie.cn

[Q79] 字符串拼接
来源：http://yl.huixinmuqiang.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ut.szxytkj.cn

[Q80] 字符串截取
来源：http://qo.shtwfgs.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://al.yuexingan06.cn

[Q81] 字符串替换
来源：http://ee.szsharing.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ud.haigaiapp.cn

[Q82] 字符长度与字节长度
来源：http://zg.muxihuayi.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://pu.newstarts.cn

[Q83] 大小写转换
来源：http://em.bookmarksfly.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://cy.hahajie.cn

[Q84] 去除首尾空格
来源：http://fn.lnxyls.cn

SELECT TRIM(name) FROM users;
来源：http://ts.huanxung.cn

[Q85] 数值取整
来源：http://bu.newstarts.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://nl.jctech888.com.cn

[Q86] 读取 JSON 字段
来源：http://mw.jctech888.com.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hj.521024.cn

[Q87] JSON 字段做条件
来源：http://po.jianghongdianzi.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://pj.szsharing.cn

[Q88] 行转列（条件聚合）
来源：http://nj.jianghongdianzi.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hp.huanxung.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://gg.newstarts.cn

[Q89] 判断表是否存在
来源：http://uw.yuexingan06.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://vf.panjiajie.cn

[Q90] 生成序号列
来源：http://bc.jianghongdianzi.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ny.colortex.cn

================================================================================
来源：http://jv.huixiangedu.cn

R. Bash 专题
来源：http://xu.nicolike.cn

================================================================================
来源：http://in.szsharing.cn

[R01] shebang 与严格模式
来源：http://ah.yuexingan06.cn

#!/usr/bin/env bash
来源：http://xp.huanxung.cn

set -euo pipefail
来源：http://eq.huixinmuqiang.cn

[R02] 变量赋值与使用
来源：http://my.nicolike.cn

name="Tom"; echo "$name"
来源：http://uq.panjiajie.cn

[R03] 只读变量
来源：http://ok.huixinmuqiang.cn

readonly PI=3.14
来源：http://td.jianghongdianzi.cn

[R04] 位置参数
来源：http://ke.yuexingan06.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ka.muxihuayi.cn

[R05] 参数默认值
来源：http://bt.asd995.cn

name="${1:-default}"
来源：http://kb.szxytkj.cn

[R06] 判断命令是否存在
来源：http://no.9csxet.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://yj.lnxyls.cn

[R07] if 判断文件
来源：http://ab.521024.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://zo.yuntaijiaju.cn

[R08] 数值比较
来源：http://sb.gzmigu.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://ip.nszjky.cn

[R09] 字符串比较
来源：http://zq.asd995.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://lq.nszjky.cn

[R10] 正则匹配
来源：http://jw.jctech888.com.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://rc.bjjhwx.cn

[R11] case 多分支
来源：http://ko.nicolike.cn

case "$1" in
来源：http://mi.9csxet.cn

start) echo "启动" ;;
来源：http://am.colortex.cn

stop)  echo "停止" ;;
来源：http://cj.huanxung.cn

*)     echo "未知命令" ;;
来源：http://vd.panjiajie.cn

esac
来源：http://ql.shxzukj.cn

[R12] for 遍历文件
来源：http://uy.yuexingan06.cn

for f in *.txt; do echo "$f"; done
来源：http://rt.wgjwhj.cn

[R13] for 计数循环
来源：http://el.bjjhwx.cn

for i in {1..10}; do echo "$i"; done
来源：http://bs.bookmarksfly.cn

[R14] C 风格 for
来源：http://mi.yuexingan06.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://yr.shxzskj.cn

[R15] while 逐行读文件
来源：http://bd.chemitech.net.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://xb.lnxyls.cn

[R16] until 等待条件
来源：http://wr.szsharing.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ez.szxytkj.cn

[R17] 数组定义与取值
来源：http://ms.haigaiapp.cn

arr=(a b c); echo "${arr[0]}"
来源：http://gl.gzmigu.cn

[R18] 遍历数组
来源：http://mw.jianghongdianzi.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://yj.gzmigu.cn

[R19] 数组长度
来源：http://eo.huanxung.cn

echo "${#arr[@]}"
来源：http://ll.chemitech.net.cn

[R20] 关联数组（字典）
来源：http://rw.shxzukj.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ib.hahajie.cn

[R21] 字符串长度
来源：http://eb.shxzskj.cn

echo "${#s}"
来源：http://ys.huixiangedu.cn

[R22] 截取子串
来源：http://no.shtwfgs.cn

echo "${s:0:5}"
来源：http://wi.hahajie.cn

[R23] 字符串替换
来源：http://xg.asd995.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://oc.haigaiapp.cn

[R24] 大小写转换
来源：http://kl.9csxet.cn

echo "${s^^}"; echo "${s,,}"
来源：http://qv.nszjky.cn

[R25] 去后缀 / 去前缀
来源：http://lj.asd995.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://he.lnxyls.cn

[R26] 命令替换
来源：http://mj.gzmigu.cn

now=$(date +%F); echo "$now"
来源：http://cu.newstarts.cn

[R27] 算术展开
来源：http://me.huixiangedu.cn

echo $((1 + 2 * 3))
来源：http://xq.huixiangedu.cn

[R28] 浮点运算
来源：http://qa.shtwfgs.cn

echo "scale=2; 10/3" | bc
来源：http://on.panjiajie.cn

[R29] 定义函数
来源：http://gf.panjiajie.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ii.jianghongdianzi.cn

[R30] 函数返回状态码
来源：http://rc.bjjhwx.cn

f() { return 0; }; f || echo "失败了"
来源：http://zl.hnjuh.cn

[R31] 局部变量
来源：http://cq.bookmarksfly.cn

f() { local x=1; echo "$x"; }
来源：http://sn.nszjky.cn

[R32] 参数个数校验
来源：http://xp.muxihuayi.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ai.huixinmuqiang.cn

[R33] 捕获错误并提示行号
来源：http://dq.huixinmuqiang.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://eh.yuntaijiaju.cn

[R34] 退出时清理
来源：http://ax.yuexingan06.cn

trap 'rm -f "$tmp"' EXIT
来源：http://aw.huanxung.cn

[R35] 后台执行并等待
来源：http://ir.jctech888.com.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://mp.shxzskj.cn

[R36] 并发执行多个任务
来源：http://nh.shtwfgs.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://uh.bookmarksfly.cn

[R37] 把输出赋给变量
来源：http://xn.muxihuayi.cn

files=$(ls -1)
来源：http://ou.521024.cn

[R38] 管道串联
来源：http://kv.huanxung.cn

cat a.txt | grep -i error | wc -l
来源：http://xf.wgjwhj.cn

[R39] 重定向标准输出与错误
来源：http://kr.521024.cn

cmd > out.log 2>&1
来源：http://yg.nszjky.cn

[R40] 追加写日志
来源：http://eu.yuexingan06.cn

echo "log" >> out.log
来源：http://jt.szxytkj.cn

[R41] 丢弃输出
来源：http://kk.colortex.cn

cmd >/dev/null 2>&1
来源：http://yu.yuntaijiaju.cn

[R42] 输入重定向
来源：http://xp.yuntaijiaju.cn

wc -l < a.txt
来源：http://zx.yuntaijiaju.cn

[R43] 按名字查找文件
来源：http://go.bookmarksfly.cn

find . -name "*.log" -type f
来源：http://lv.bjjhwx.cn

[R44] 按修改时间查找
来源：http://uf.panjiajie.cn

find . -mtime -7 -type f
来源：http://av.hnjuh.cn

[R45] 批量删除
来源：http://li.haigaiapp.cn

find . -name "*.tmp" -delete
来源：http://jn.chemitech.net.cn

[R46] 递归替换文件内容
来源：http://gb.bookmarksfly.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://li.panjiajie.cn

[R47] sed 单行替换
来源：http://ug.bjjhwx.cn

sed -i 's/foo/bar/g' a.txt
来源：http://pi.lnxyls.cn

[R48] awk 取指定列
来源：http://jo.muxihuayi.cn

awk '{print $1, $3}' a.txt
来源：http://yv.gzmigu.cn

[R49] awk 带条件
来源：http://ma.gzmigu.cn


<!-- 参考信息 -->