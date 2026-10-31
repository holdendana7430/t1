代发 wailian999

);
来源：http://cr.colortex.cn

[Q03] 增加列
来源：http://uc.nicolike.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://cx.shxzskj.cn

[Q04] 修改列类型
来源：http://bj.hahajie.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ok.muxihuayi.cn

[Q05] 重命名列
来源：http://zz.shxzskj.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://yv.521024.cn

[Q06] 删除列
来源：http://fb.shxzukj.cn

ALTER TABLE users DROP COLUMN age;
来源：http://lh.yuexingan06.cn

[Q07] 删除表
来源：http://oq.9csxet.cn

DROP TABLE IF EXISTS orders;
来源：http://bn.colortex.cn

[Q08] 创建普通索引
来源：http://ug.lnxyls.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://ib.nszjky.cn

[Q09] 创建唯一索引
来源：http://cd.9csxet.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://dh.panjiajie.cn

[Q10] 插入单行
来源：http://ji.yuntaijiaju.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://of.shxzskj.cn

[Q11] 一次插入多行
来源：http://rj.huixiangedu.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://vy.shxzskj.cn

[Q12] 插入后取自增 ID
来源：http://cw.szxytkj.cn

INSERT INTO users (name) VALUES ('C');
来源：http://hr.hahajie.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://sk.shxzukj.cn

[Q13] 忽略重复插入
来源：http://if.asd995.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://pl.huixinmuqiang.cn

[Q14] 存在则更新（upsert）
来源：http://jl.huixiangedu.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ju.gzmigu.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://pi.haigaiapp.cn

[Q15] 查询全部
来源：http://yb.bookmarksfly.cn

SELECT * FROM users;
来源：http://ym.colortex.cn

[Q16] 查询指定列
来源：http://ks.hnjuh.cn

SELECT id, name FROM users;
来源：http://lc.wgjwhj.cn

[Q17] 条件查询
来源：http://nt.gzmigu.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://yl.521024.cn

[Q18] 模糊匹配
来源：http://tv.9csxet.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wi.jctech888.com.cn

[Q19] 范围查询
来源：http://tx.hnjuh.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://tv.newstarts.cn

[Q20] IN 列表
来源：http://ao.haigaiapp.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://zs.huixinmuqiang.cn

[Q21] 空值判断
来源：http://pz.yuntaijiaju.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://us.nicolike.cn

[Q22] 排序
来源：http://vg.hnjuh.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://nd.nszjky.cn

[Q23] 分页
来源：http://tr.chemitech.net.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ev.huixiangedu.cn

[Q24] 去重
来源：http://sc.yuntaijiaju.cn

SELECT DISTINCT city FROM users;
来源：http://pc.bookmarksfly.cn

[Q25] 只取前 N 条
来源：http://cy.shxzskj.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://bz.yuntaijiaju.cn

[Q26] 计数
来源：http://xg.huanxung.cn

SELECT COUNT(*) FROM users;
来源：http://hc.hahajie.cn

[Q27] 条件计数
来源：http://xl.jianghongdianzi.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://an.521024.cn

[Q28] 求和与平均
来源：http://wh.hnjuh.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://dm.asd995.cn

[Q29] 最大最小值
来源：http://uz.9csxet.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://ei.bjjhwx.cn

[Q30] 分组统计
来源：http://yx.521024.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hp.yuexingan06.cn

[Q31] 分组后过滤
来源：http://pz.yuntaijiaju.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://pc.gzmigu.cn

[Q32] 分组拼接字符串
来源：http://au.shxzukj.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://vg.nicolike.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ue.lnxyls.cn

[Q33] 多列分组
来源：http://on.yuntaijiaju.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://of.panjiajie.cn

[Q34] 每组取第一条
来源：http://go.jctech888.com.cn

SELECT * FROM (
来源：http://cj.521024.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ku.szxytkj.cn

) t WHERE rn = 1;
来源：http://cs.huanxung.cn

[Q35] 内连接
来源：http://nk.szxytkj.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://kg.jctech888.com.cn

[Q36] 左连接
来源：http://eg.panjiajie.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://zy.muxihuayi.cn

[Q37] 右连接
来源：http://ki.yuntaijiaju.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://oj.wgjwhj.cn

[Q38] 全外连接（PostgreSQL）
来源：http://ny.nicolike.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ku.wgjwhj.cn

[Q39] 自连接（查上下级）
来源：http://mr.huanxung.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://cl.bookmarksfly.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wf.asd995.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://ww.9csxet.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://cj.colortex.cn

[Q41] 多表连接
来源：http://im.9csxet.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://hv.newstarts.cn

JOIN users u ON u.id = o.user_id
来源：http://ze.bookmarksfly.cn

JOIN products p ON p.id = o.product_id;
来源：http://od.colortex.cn

[Q42] 连接条件附加过滤
来源：http://io.haigaiapp.cn

SELECT u.name, o.amount FROM users u
来源：http://of.huanxung.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://nq.wgjwhj.cn

[Q43] 标量子查询
来源：http://sm.hahajie.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://sa.bjjhwx.cn

[Q44] IN 子查询
来源：http://nh.shxzskj.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wn.jianghongdianzi.cn

[Q45] EXISTS 判断存在
来源：http://nh.lnxyls.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://og.nicolike.cn

[Q46] NOT EXISTS 判断不存在
来源：http://jm.shxzukj.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://zn.szxytkj.cn

[Q47] 与平均值比较
来源：http://xf.521024.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://rn.muxihuayi.cn

[Q48] CTE 公用表表达式
来源：http://di.hnjuh.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mo.bookmarksfly.cn

SELECT * FROM t WHERE c > 5;
来源：http://cp.panjiajie.cn

[Q49] 更新单行
来源：http://xj.shxzskj.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://zm.shtwfgs.cn

[Q50] 批量更新
来源：http://uf.haigaiapp.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://dm.muxihuayi.cn

[Q51] 用子查询更新
来源：http://sa.9csxet.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://po.bjjhwx.cn

[Q52] 删除指定行
来源：http://ni.huixiangedu.cn

DELETE FROM users WHERE id = 10;
来源：http://nc.hnjuh.cn

[Q53] 按条件删除
来源：http://oa.chemitech.net.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://vu.yuntaijiaju.cn

[Q54] 清空表
来源：http://ls.521024.cn

TRUNCATE TABLE logs;
来源：http://vk.panjiajie.cn

[Q55] 排名（并列占位）
来源：http://ca.shxzukj.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://qt.yuntaijiaju.cn

[Q56] 密集排名（并列不占位）
来源：http://ek.szxytkj.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://iv.newstarts.cn

[Q57] 行号
来源：http://py.huixiangedu.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://tt.szxytkj.cn

[Q58] 累计求和
来源：http://yw.shxzukj.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://vk.hnjuh.cn

[Q59] 分组内累计
来源：http://ga.yuntaijiaju.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://in.nicolike.cn

[Q60] 取上一行 / 下一行
来源：http://bj.gzmigu.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://pw.lnxyls.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hw.szsharing.cn

[Q61] 移动平均
来源：http://go.chemitech.net.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ld.hahajie.cn

[Q62] 分组占比
来源：http://rd.asd995.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://aa.colortex.cn

[Q63] 开启事务
来源：http://xc.521024.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://ai.asd995.cn

[Q64] 提交事务
来源：http://gf.huixiangedu.cn

COMMIT;
来源：http://kj.521024.cn

[Q65] 回滚事务
来源：http://id.nicolike.cn

ROLLBACK;
来源：http://xd.szsharing.cn

[Q66] 行锁查询
来源：http://ze.wgjwhj.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://zw.hnjuh.cn

[Q67] 设置隔离级别
来源：http://fi.hnjuh.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://xu.bjjhwx.cn

[Q68] 保存点
来源：http://aq.colortex.cn

SAVEPOINT sp1;
来源：http://tw.panjiajie.cn

ROLLBACK TO sp1;
来源：http://uf.newstarts.cn

[Q69] 查看执行计划
来源：http://mz.bjjhwx.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://jy.hahajie.cn

[Q70] 更新统计信息
来源：http://cz.wgjwhj.cn

ANALYZE TABLE users;
来源：http://ec.yuntaijiaju.cn

[Q71] 查看建表语句
来源：http://ev.jianghongdianzi.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://os.shxzskj.cn

[Q72] 查看索引
来源：http://sl.chemitech.net.cn

SHOW INDEX FROM users;
来源：http://gu.521024.cn

[Q73] 查看表状态
来源：http://yj.bjjhwx.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://jt.bookmarksfly.cn

[Q74] 强制使用索引
来源：http://lw.colortex.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://af.lnxyls.cn

[Q75] 日期格式化
来源：http://ov.nicolike.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://db.asd995.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://fh.bjjhwx.cn

[Q76] 按天统计
来源：http://fp.muxihuayi.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://pk.szxytkj.cn

[Q77] 时间加减
来源：http://jj.szxytkj.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://tf.asd995.cn

[Q78] 当前时间
来源：http://po.jianghongdianzi.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ll.yuntaijiaju.cn

[Q79] 字符串拼接
来源：http://rp.huixiangedu.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://qn.chemitech.net.cn

[Q80] 字符串截取
来源：http://vv.szsharing.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://za.jctech888.com.cn

[Q81] 字符串替换
来源：http://qp.hnjuh.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://kl.newstarts.cn

[Q82] 字符长度与字节长度
来源：http://hp.nszjky.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://fz.bookmarksfly.cn

[Q83] 大小写转换
来源：http://zp.hnjuh.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.hahajie.cn

[Q84] 去除首尾空格
来源：http://ds.yuntaijiaju.cn

SELECT TRIM(name) FROM users;
来源：http://my.521024.cn

[Q85] 数值取整
来源：http://st.bjjhwx.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ns.colortex.cn

[Q86] 读取 JSON 字段
来源：http://fa.huanxung.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://fh.nszjky.cn

[Q87] JSON 字段做条件
来源：http://qh.jianghongdianzi.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ui.szxytkj.cn

[Q88] 行转列（条件聚合）
来源：http://ef.lnxyls.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ge.haigaiapp.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://et.haigaiapp.cn

[Q89] 判断表是否存在
来源：http://tz.hahajie.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://gd.huanxung.cn

[Q90] 生成序号列
来源：http://zg.521024.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://jx.yuntaijiaju.cn

================================================================================
来源：http://jl.asd995.cn

R. Bash 专题
来源：http://gv.newstarts.cn

================================================================================
来源：http://vy.szxytkj.cn

[R01] shebang 与严格模式
来源：http://ta.asd995.cn

#!/usr/bin/env bash
来源：http://qn.521024.cn

set -euo pipefail
来源：http://bf.haigaiapp.cn

[R02] 变量赋值与使用
来源：http://yk.bjjhwx.cn

name="Tom"; echo "$name"
来源：http://wz.shxzukj.cn

[R03] 只读变量
来源：http://jr.yuexingan06.cn

readonly PI=3.14
来源：http://ec.lnxyls.cn

[R04] 位置参数
来源：http://sp.panjiajie.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://rn.lnxyls.cn

[R05] 参数默认值
来源：http://qa.jianghongdianzi.cn

name="${1:-default}"
来源：http://tb.yuntaijiaju.cn

[R06] 判断命令是否存在
来源：http://jy.haigaiapp.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://xn.lnxyls.cn

[R07] if 判断文件
来源：http://qd.szsharing.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hi.jctech888.com.cn

[R08] 数值比较
来源：http://fd.shtwfgs.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://kc.shxzukj.cn

[R09] 字符串比较
来源：http://ca.huixinmuqiang.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://je.gzmigu.cn

[R10] 正则匹配
来源：http://cd.szxytkj.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ik.muxihuayi.cn

[R11] case 多分支
来源：http://ar.shtwfgs.cn

case "$1" in
来源：http://yq.huanxung.cn

start) echo "启动" ;;
来源：http://lx.muxihuayi.cn

stop)  echo "停止" ;;
来源：http://xn.hnjuh.cn

*)     echo "未知命令" ;;
来源：http://pe.newstarts.cn

esac
来源：http://pc.wgjwhj.cn

[R12] for 遍历文件
来源：http://rl.bookmarksfly.cn

for f in *.txt; do echo "$f"; done
来源：http://gh.chemitech.net.cn

[R13] for 计数循环
来源：http://sx.nicolike.cn

for i in {1..10}; do echo "$i"; done
来源：http://rn.shxzskj.cn

[R14] C 风格 for
来源：http://zd.chemitech.net.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://za.lnxyls.cn

[R15] while 逐行读文件
来源：http://vz.asd995.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://zb.bjjhwx.cn

[R16] until 等待条件
来源：http://qx.huanxung.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://nm.huixiangedu.cn

[R17] 数组定义与取值
来源：http://xl.shtwfgs.cn

arr=(a b c); echo "${arr[0]}"
来源：http://sw.szxytkj.cn

[R18] 遍历数组
来源：http://uk.huanxung.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://pp.yuexingan06.cn

[R19] 数组长度
来源：http://vd.newstarts.cn

echo "${#arr[@]}"
来源：http://mm.shtwfgs.cn

[R20] 关联数组（字典）
来源：http://hr.shxzskj.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ja.huixinmuqiang.cn

[R21] 字符串长度
来源：http://im.szsharing.cn

echo "${#s}"
来源：http://jo.wgjwhj.cn

[R22] 截取子串
来源：http://xj.szxytkj.cn

echo "${s:0:5}"
来源：http://jr.bookmarksfly.cn

[R23] 字符串替换
来源：http://yg.shxzukj.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://qe.colortex.cn

[R24] 大小写转换
来源：http://cq.chemitech.net.cn

echo "${s^^}"; echo "${s,,}"
来源：http://jn.haigaiapp.cn

[R25] 去后缀 / 去前缀
来源：http://st.chemitech.net.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://ms.haigaiapp.cn

[R26] 命令替换
来源：http://oy.bjjhwx.cn

now=$(date +%F); echo "$now"
来源：http://lw.yuntaijiaju.cn

[R27] 算术展开
来源：http://rz.yuntaijiaju.cn

echo $((1 + 2 * 3))
来源：http://uj.nszjky.cn

[R28] 浮点运算
来源：http://cb.nicolike.cn

echo "scale=2; 10/3" | bc
来源：http://kg.bjjhwx.cn

[R29] 定义函数
来源：http://na.huixiangedu.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://tp.nicolike.cn

[R30] 函数返回状态码
来源：http://hz.szsharing.cn

f() { return 0; }; f || echo "失败了"
来源：http://dg.bookmarksfly.cn

[R31] 局部变量
来源：http://as.shtwfgs.cn

f() { local x=1; echo "$x"; }
来源：http://dm.9csxet.cn

[R32] 参数个数校验
来源：http://vh.nszjky.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wt.9csxet.cn

[R33] 捕获错误并提示行号
来源：http://hr.colortex.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ep.jianghongdianzi.cn

[R34] 退出时清理
来源：http://me.shtwfgs.cn

trap 'rm -f "$tmp"' EXIT
来源：http://lw.gzmigu.cn

[R35] 后台执行并等待
来源：http://xq.asd995.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://fo.lnxyls.cn

[R36] 并发执行多个任务
来源：http://hd.wgjwhj.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://jb.bjjhwx.cn

[R37] 把输出赋给变量
来源：http://kf.bjjhwx.cn

files=$(ls -1)
来源：http://fi.jctech888.com.cn

[R38] 管道串联
来源：http://tq.wgjwhj.cn

cat a.txt | grep -i error | wc -l
来源：http://ud.panjiajie.cn

[R39] 重定向标准输出与错误
来源：http://vz.chemitech.net.cn

cmd > out.log 2>&1
来源：http://ki.hahajie.cn

[R40] 追加写日志
来源：http://cz.9csxet.cn

echo "log" >> out.log
来源：http://qf.nicolike.cn

[R41] 丢弃输出
来源：http://ht.jctech888.com.cn

cmd >/dev/null 2>&1
来源：http://ou.shxzskj.cn

[R42] 输入重定向
来源：http://ty.bookmarksfly.cn

wc -l < a.txt
来源：http://dh.haigaiapp.cn

[R43] 按名字查找文件
来源：http://gj.nszjky.cn

find . -name "*.log" -type f
来源：http://fl.nicolike.cn

[R44] 按修改时间查找
来源：http://zz.yuntaijiaju.cn

find . -mtime -7 -type f
来源：http://li.szsharing.cn

[R45] 批量删除
来源：http://ei.521024.cn

find . -name "*.tmp" -delete
来源：http://ys.haigaiapp.cn

[R46] 递归替换文件内容
来源：http://qr.yuexingan06.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://js.szxytkj.cn

[R47] sed 单行替换
来源：http://am.huixiangedu.cn

sed -i 's/foo/bar/g' a.txt
来源：http://xe.jianghongdianzi.cn

[R48] awk 取指定列
来源：http://iz.colortex.cn

awk '{print $1, $3}' a.txt
来源：http://io.bookmarksfly.cn

[R49] awk 带条件
来源：http://rn.newstarts.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://vn.huanxung.cn

[R50] awk 求和
来源：http://xk.huanxung.cn

awk '{s += $2} END {print s}' a.txt
来源：http://ce.chemitech.net.cn

[R51] 排序去重取前几
来源：http://no.hnjuh.cn


<!-- 参考信息 -->