代发 wailian999

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://zn.gzmigu.cn

user_id INT NOT NULL,
来源：http://pc.asd995.cn

amount DECIMAL(10, 2),
来源：http://rk.bookmarksfly.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ug.jctech888.com.cn

);
来源：http://tz.521024.cn

[Q03] 增加列
来源：http://hr.bjjhwx.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wd.szxytkj.cn

[Q04] 修改列类型
来源：http://ln.shxzukj.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://fo.panjiajie.cn

[Q05] 重命名列
来源：http://db.szxytkj.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://si.szsharing.cn

[Q06] 删除列
来源：http://gj.nszjky.cn

ALTER TABLE users DROP COLUMN age;
来源：http://tp.asd995.cn

[Q07] 删除表
来源：http://ey.haigaiapp.cn

DROP TABLE IF EXISTS orders;
来源：http://jf.yuntaijiaju.cn

[Q08] 创建普通索引
来源：http://gd.wgjwhj.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://mt.chemitech.net.cn

[Q09] 创建唯一索引
来源：http://eh.lnxyls.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://dz.panjiajie.cn

[Q10] 插入单行
来源：http://px.colortex.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://it.huixinmuqiang.cn

[Q11] 一次插入多行
来源：http://pr.yuntaijiaju.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://of.jianghongdianzi.cn

[Q12] 插入后取自增 ID
来源：http://ux.hnjuh.cn

INSERT INTO users (name) VALUES ('C');
来源：http://xn.shxzskj.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hf.chemitech.net.cn

[Q13] 忽略重复插入
来源：http://rl.shxzukj.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://tv.szxytkj.cn

[Q14] 存在则更新（upsert）
来源：http://ff.yuntaijiaju.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://qj.shxzskj.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://op.hnjuh.cn

[Q15] 查询全部
来源：http://kn.hnjuh.cn

SELECT * FROM users;
来源：http://xm.gzmigu.cn

[Q16] 查询指定列
来源：http://lb.muxihuayi.cn

SELECT id, name FROM users;
来源：http://tf.jctech888.com.cn

[Q17] 条件查询
来源：http://qg.521024.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ou.chemitech.net.cn

[Q18] 模糊匹配
来源：http://de.nszjky.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ff.muxihuayi.cn

[Q19] 范围查询
来源：http://st.jianghongdianzi.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mh.yuntaijiaju.cn

[Q20] IN 列表
来源：http://et.szxytkj.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://yz.9csxet.cn

[Q21] 空值判断
来源：http://vn.szsharing.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://ig.yuntaijiaju.cn

[Q22] 排序
来源：http://gh.shxzskj.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hp.asd995.cn

[Q23] 分页
来源：http://sq.muxihuayi.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://rw.9csxet.cn

[Q24] 去重
来源：http://nz.huanxung.cn

SELECT DISTINCT city FROM users;
来源：http://ip.wgjwhj.cn

[Q25] 只取前 N 条
来源：http://sw.bookmarksfly.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://lb.newstarts.cn

[Q26] 计数
来源：http://zm.bjjhwx.cn

SELECT COUNT(*) FROM users;
来源：http://dg.haigaiapp.cn

[Q27] 条件计数
来源：http://pc.yuntaijiaju.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://pv.huixiangedu.cn

[Q28] 求和与平均
来源：http://we.yuexingan06.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://kq.hahajie.cn

[Q29] 最大最小值
来源：http://ra.colortex.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://qb.muxihuayi.cn

[Q30] 分组统计
来源：http://gy.9csxet.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://np.hnjuh.cn

[Q31] 分组后过滤
来源：http://hb.yuexingan06.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://gh.bjjhwx.cn

[Q32] 分组拼接字符串
来源：http://ei.yuexingan06.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wf.colortex.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://tq.nszjky.cn

[Q33] 多列分组
来源：http://lq.bookmarksfly.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://om.chemitech.net.cn

[Q34] 每组取第一条
来源：http://xe.newstarts.cn

SELECT * FROM (
来源：http://dk.huixinmuqiang.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://qg.shxzukj.cn

) t WHERE rn = 1;
来源：http://as.yuexingan06.cn

[Q35] 内连接
来源：http://du.shxzskj.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://we.szsharing.cn

[Q36] 左连接
来源：http://xt.9csxet.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ju.shxzskj.cn

[Q37] 右连接
来源：http://vr.shtwfgs.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://fb.nszjky.cn

[Q38] 全外连接（PostgreSQL）
来源：http://wj.521024.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://jr.huixinmuqiang.cn

[Q39] 自连接（查上下级）
来源：http://qg.panjiajie.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://yy.shtwfgs.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ag.jctech888.com.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://yj.shxzskj.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://oc.shtwfgs.cn

[Q41] 多表连接
来源：http://zj.huixiangedu.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://cz.yuntaijiaju.cn

JOIN users u ON u.id = o.user_id
来源：http://da.nicolike.cn

JOIN products p ON p.id = o.product_id;
来源：http://ky.panjiajie.cn

[Q42] 连接条件附加过滤
来源：http://lc.haigaiapp.cn

SELECT u.name, o.amount FROM users u
来源：http://nq.haigaiapp.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://sw.hnjuh.cn

[Q43] 标量子查询
来源：http://uk.lnxyls.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://vg.bookmarksfly.cn

[Q44] IN 子查询
来源：http://es.shxzukj.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://pc.521024.cn

[Q45] EXISTS 判断存在
来源：http://hn.yuntaijiaju.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ij.haigaiapp.cn

[Q46] NOT EXISTS 判断不存在
来源：http://gy.asd995.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ul.yuntaijiaju.cn

[Q47] 与平均值比较
来源：http://os.nicolike.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ed.hnjuh.cn

[Q48] CTE 公用表表达式
来源：http://oe.panjiajie.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://nj.muxihuayi.cn

SELECT * FROM t WHERE c > 5;
来源：http://xv.asd995.cn

[Q49] 更新单行
来源：http://jh.chemitech.net.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://jg.bjjhwx.cn

[Q50] 批量更新
来源：http://bk.shxzukj.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://bx.wgjwhj.cn

[Q51] 用子查询更新
来源：http://uk.lnxyls.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://da.huixiangedu.cn

[Q52] 删除指定行
来源：http://nv.yuntaijiaju.cn

DELETE FROM users WHERE id = 10;
来源：http://cc.jctech888.com.cn

[Q53] 按条件删除
来源：http://zx.bookmarksfly.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://sc.szsharing.cn

[Q54] 清空表
来源：http://fx.jianghongdianzi.cn

TRUNCATE TABLE logs;
来源：http://zy.lnxyls.cn

[Q55] 排名（并列占位）
来源：http://xw.521024.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://cz.hahajie.cn

[Q56] 密集排名（并列不占位）
来源：http://aa.huanxung.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://pb.hnjuh.cn

[Q57] 行号
来源：http://mc.chemitech.net.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://jj.szsharing.cn

[Q58] 累计求和
来源：http://wg.panjiajie.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://lv.hahajie.cn

[Q59] 分组内累计
来源：http://cd.muxihuayi.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://es.yuexingan06.cn

[Q60] 取上一行 / 下一行
来源：http://sl.lnxyls.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://zw.szsharing.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://vf.yuexingan06.cn

[Q61] 移动平均
来源：http://li.muxihuayi.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://pm.shtwfgs.cn

[Q62] 分组占比
来源：http://cm.9csxet.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://nv.huixinmuqiang.cn

[Q63] 开启事务
来源：http://vb.jianghongdianzi.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://zb.huanxung.cn

[Q64] 提交事务
来源：http://ku.panjiajie.cn

COMMIT;
来源：http://iu.hnjuh.cn

[Q65] 回滚事务
来源：http://bz.shxzskj.cn

ROLLBACK;
来源：http://de.colortex.cn

[Q66] 行锁查询
来源：http://ji.colortex.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mk.gzmigu.cn

[Q67] 设置隔离级别
来源：http://qn.gzmigu.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://fv.hahajie.cn

[Q68] 保存点
来源：http://oi.shtwfgs.cn

SAVEPOINT sp1;
来源：http://ac.haigaiapp.cn

ROLLBACK TO sp1;
来源：http://mf.chemitech.net.cn

[Q69] 查看执行计划
来源：http://vx.bookmarksfly.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://gm.panjiajie.cn

[Q70] 更新统计信息
来源：http://ri.bookmarksfly.cn

ANALYZE TABLE users;
来源：http://mv.shxzskj.cn

[Q71] 查看建表语句
来源：http://if.huixiangedu.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://pm.wgjwhj.cn

[Q72] 查看索引
来源：http://fw.bookmarksfly.cn

SHOW INDEX FROM users;
来源：http://ja.muxihuayi.cn

[Q73] 查看表状态
来源：http://no.jctech888.com.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://es.521024.cn

[Q74] 强制使用索引
来源：http://fx.yuexingan06.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://bz.nicolike.cn

[Q75] 日期格式化
来源：http://bq.shtwfgs.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://cp.chemitech.net.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://sn.haigaiapp.cn

[Q76] 按天统计
来源：http://kn.shxzukj.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://es.gzmigu.cn

[Q77] 时间加减
来源：http://ov.panjiajie.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://av.panjiajie.cn

[Q78] 当前时间
来源：http://di.chemitech.net.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ib.bookmarksfly.cn

[Q79] 字符串拼接
来源：http://af.asd995.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://cx.szsharing.cn

[Q80] 字符串截取
来源：http://qt.colortex.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://sr.bjjhwx.cn

[Q81] 字符串替换
来源：http://vh.9csxet.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hc.bjjhwx.cn

[Q82] 字符长度与字节长度
来源：http://ub.huanxung.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ox.bjjhwx.cn

[Q83] 大小写转换
来源：http://ff.hnjuh.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://oc.chemitech.net.cn

[Q84] 去除首尾空格
来源：http://bm.huixinmuqiang.cn

SELECT TRIM(name) FROM users;
来源：http://pd.shtwfgs.cn

[Q85] 数值取整
来源：http://aa.asd995.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://yk.shxzskj.cn

[Q86] 读取 JSON 字段
来源：http://sb.panjiajie.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://fc.muxihuayi.cn

[Q87] JSON 字段做条件
来源：http://tf.wgjwhj.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://oe.chemitech.net.cn

[Q88] 行转列（条件聚合）
来源：http://uz.9csxet.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://qf.9csxet.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://gf.colortex.cn

[Q89] 判断表是否存在
来源：http://gh.hnjuh.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wt.shxzukj.cn

[Q90] 生成序号列
来源：http://ei.haigaiapp.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://aa.huanxung.cn

================================================================================
来源：http://bs.bookmarksfly.cn

R. Bash 专题
来源：http://ki.asd995.cn

================================================================================
来源：http://wp.hnjuh.cn

[R01] shebang 与严格模式
来源：http://cl.bjjhwx.cn

#!/usr/bin/env bash
来源：http://aq.yuntaijiaju.cn

set -euo pipefail
来源：http://az.panjiajie.cn

[R02] 变量赋值与使用
来源：http://km.hahajie.cn

name="Tom"; echo "$name"
来源：http://vi.shtwfgs.cn

[R03] 只读变量
来源：http://vi.hnjuh.cn

readonly PI=3.14
来源：http://bu.colortex.cn

[R04] 位置参数
来源：http://mg.nicolike.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://pp.jianghongdianzi.cn

[R05] 参数默认值
来源：http://gs.shxzukj.cn

name="${1:-default}"
来源：http://mw.haigaiapp.cn

[R06] 判断命令是否存在
来源：http://su.szsharing.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://yk.colortex.cn

[R07] if 判断文件
来源：http://ui.panjiajie.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://qj.521024.cn

[R08] 数值比较
来源：http://uj.muxihuayi.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://ek.nicolike.cn

[R09] 字符串比较
来源：http://tr.hnjuh.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://qy.jctech888.com.cn

[R10] 正则匹配
来源：http://ha.haigaiapp.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://qc.huixinmuqiang.cn

[R11] case 多分支
来源：http://ar.newstarts.cn

case "$1" in
来源：http://mh.newstarts.cn

start) echo "启动" ;;
来源：http://jl.panjiajie.cn

stop)  echo "停止" ;;
来源：http://ex.lnxyls.cn

*)     echo "未知命令" ;;
来源：http://gp.shxzukj.cn

esac
来源：http://lh.szsharing.cn

[R12] for 遍历文件
来源：http://he.lnxyls.cn

for f in *.txt; do echo "$f"; done
来源：http://kp.newstarts.cn

[R13] for 计数循环
来源：http://ab.shxzskj.cn

for i in {1..10}; do echo "$i"; done
来源：http://cg.shxzukj.cn

[R14] C 风格 for
来源：http://ua.jctech888.com.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://zg.9csxet.cn

[R15] while 逐行读文件
来源：http://ug.newstarts.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://vm.9csxet.cn

[R16] until 等待条件
来源：http://xw.9csxet.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://pt.colortex.cn

[R17] 数组定义与取值
来源：http://vz.gzmigu.cn

arr=(a b c); echo "${arr[0]}"
来源：http://bq.chemitech.net.cn

[R18] 遍历数组
来源：http://vc.lnxyls.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ta.haigaiapp.cn

[R19] 数组长度
来源：http://vb.nicolike.cn

echo "${#arr[@]}"
来源：http://am.shxzukj.cn

[R20] 关联数组（字典）
来源：http://xu.nicolike.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://yd.hnjuh.cn

[R21] 字符串长度
来源：http://jk.huixiangedu.cn

echo "${#s}"
来源：http://xl.gzmigu.cn

[R22] 截取子串
来源：http://cy.shxzskj.cn

echo "${s:0:5}"
来源：http://gu.hahajie.cn

[R23] 字符串替换
来源：http://fv.nicolike.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://qa.chemitech.net.cn

[R24] 大小写转换
来源：http://av.wgjwhj.cn

echo "${s^^}"; echo "${s,,}"
来源：http://zg.521024.cn

[R25] 去后缀 / 去前缀
来源：http://av.shxzskj.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://fz.nszjky.cn

[R26] 命令替换
来源：http://yi.bjjhwx.cn

now=$(date +%F); echo "$now"
来源：http://fw.gzmigu.cn

[R27] 算术展开
来源：http://ft.yuntaijiaju.cn

echo $((1 + 2 * 3))
来源：http://ba.hnjuh.cn

[R28] 浮点运算
来源：http://rc.muxihuayi.cn

echo "scale=2; 10/3" | bc
来源：http://go.huixiangedu.cn

[R29] 定义函数
来源：http://ht.yuntaijiaju.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hs.yuexingan06.cn

[R30] 函数返回状态码
来源：http://am.9csxet.cn

f() { return 0; }; f || echo "失败了"
来源：http://va.szsharing.cn

[R31] 局部变量
来源：http://ot.shtwfgs.cn

f() { local x=1; echo "$x"; }
来源：http://uk.gzmigu.cn

[R32] 参数个数校验
来源：http://vl.shtwfgs.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://rk.szsharing.cn

[R33] 捕获错误并提示行号
来源：http://yl.newstarts.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://yq.shxzskj.cn

[R34] 退出时清理
来源：http://gd.chemitech.net.cn

trap 'rm -f "$tmp"' EXIT
来源：http://ju.jctech888.com.cn

[R35] 后台执行并等待
来源：http://an.huixiangedu.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://ph.hnjuh.cn

[R36] 并发执行多个任务
来源：http://bw.yuexingan06.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://nd.wgjwhj.cn

[R37] 把输出赋给变量
来源：http://iw.szsharing.cn

files=$(ls -1)
来源：http://sp.jctech888.com.cn

[R38] 管道串联
来源：http://nv.9csxet.cn

cat a.txt | grep -i error | wc -l
来源：http://jj.shxzukj.cn

[R39] 重定向标准输出与错误
来源：http://cl.shxzskj.cn

cmd > out.log 2>&1
来源：http://ny.yuexingan06.cn

[R40] 追加写日志
来源：http://xo.bookmarksfly.cn

echo "log" >> out.log
来源：http://po.colortex.cn

[R41] 丢弃输出
来源：http://rs.nszjky.cn

cmd >/dev/null 2>&1
来源：http://lh.nszjky.cn

[R42] 输入重定向
来源：http://sk.9csxet.cn

wc -l < a.txt
来源：http://pr.szsharing.cn

[R43] 按名字查找文件
来源：http://uc.lnxyls.cn

find . -name "*.log" -type f
来源：http://mv.hahajie.cn

[R44] 按修改时间查找
来源：http://xw.hnjuh.cn

find . -mtime -7 -type f
来源：http://ef.shxzskj.cn

[R45] 批量删除
来源：http://gy.521024.cn

find . -name "*.tmp" -delete
来源：http://or.huanxung.cn

[R46] 递归替换文件内容
来源：http://bj.521024.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://qi.newstarts.cn

[R47] sed 单行替换
来源：http://ku.shxzukj.cn

sed -i 's/foo/bar/g' a.txt
来源：http://oj.newstarts.cn

[R48] awk 取指定列
来源：http://re.asd995.cn

awk '{print $1, $3}' a.txt
来源：http://mn.szxytkj.cn

[R49] awk 带条件
来源：http://dv.colortex.cn


<!-- 参考信息 -->