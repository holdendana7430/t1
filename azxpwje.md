代发 wailian999

);
来源：http://yw.huixinmuqiang.cn

[Q03] 增加列
来源：http://ez.nszjky.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://vx.muxihuayi.cn

[Q04] 修改列类型
来源：http://ls.szxytkj.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://gq.shtwfgs.cn

[Q05] 重命名列
来源：http://sf.lnxyls.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://uy.shtwfgs.cn

[Q06] 删除列
来源：http://fy.huanxung.cn

ALTER TABLE users DROP COLUMN age;
来源：http://wa.huixiangedu.cn

[Q07] 删除表
来源：http://hc.hahajie.cn

DROP TABLE IF EXISTS orders;
来源：http://yk.9csxet.cn

[Q08] 创建普通索引
来源：http://az.lnxyls.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://dl.huanxung.cn

[Q09] 创建唯一索引
来源：http://li.newstarts.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://dl.asd995.cn

[Q10] 插入单行
来源：http://ey.szsharing.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ey.bookmarksfly.cn

[Q11] 一次插入多行
来源：http://qt.szsharing.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://bi.hnjuh.cn

[Q12] 插入后取自增 ID
来源：http://lo.hnjuh.cn

INSERT INTO users (name) VALUES ('C');
来源：http://ww.521024.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://vx.shxzukj.cn

[Q13] 忽略重复插入
来源：http://qm.colortex.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://uv.hnjuh.cn

[Q14] 存在则更新（upsert）
来源：http://wo.hnjuh.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://le.yuntaijiaju.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://jj.nszjky.cn

[Q15] 查询全部
来源：http://kf.jianghongdianzi.cn

SELECT * FROM users;
来源：http://fg.huanxung.cn

[Q16] 查询指定列
来源：http://gb.shxzukj.cn

SELECT id, name FROM users;
来源：http://qm.asd995.cn

[Q17] 条件查询
来源：http://eq.bjjhwx.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ny.wgjwhj.cn

[Q18] 模糊匹配
来源：http://yl.yuexingan06.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://gl.huixiangedu.cn

[Q19] 范围查询
来源：http://ph.jctech888.com.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://vx.lnxyls.cn

[Q20] IN 列表
来源：http://pe.gzmigu.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://tn.bookmarksfly.cn

[Q21] 空值判断
来源：http://yq.shxzskj.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://qi.521024.cn

[Q22] 排序
来源：http://pb.huanxung.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://yv.colortex.cn

[Q23] 分页
来源：http://sj.shtwfgs.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://dn.yuexingan06.cn

[Q24] 去重
来源：http://az.hnjuh.cn

SELECT DISTINCT city FROM users;
来源：http://pt.hahajie.cn

[Q25] 只取前 N 条
来源：http://mv.jctech888.com.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://fa.nszjky.cn

[Q26] 计数
来源：http://lx.jctech888.com.cn

SELECT COUNT(*) FROM users;
来源：http://dn.hnjuh.cn

[Q27] 条件计数
来源：http://lk.shtwfgs.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wv.colortex.cn

[Q28] 求和与平均
来源：http://ux.wgjwhj.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://gt.haigaiapp.cn

[Q29] 最大最小值
来源：http://ii.jctech888.com.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://la.panjiajie.cn

[Q30] 分组统计
来源：http://ky.chemitech.net.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://rg.yuexingan06.cn

[Q31] 分组后过滤
来源：http://un.panjiajie.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://rf.panjiajie.cn

[Q32] 分组拼接字符串
来源：http://zl.shxzukj.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://tr.asd995.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://sp.newstarts.cn

[Q33] 多列分组
来源：http://gw.panjiajie.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://la.shtwfgs.cn

[Q34] 每组取第一条
来源：http://mw.huixiangedu.cn

SELECT * FROM (
来源：http://rh.gzmigu.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://lp.shtwfgs.cn

) t WHERE rn = 1;
来源：http://bn.shtwfgs.cn

[Q35] 内连接
来源：http://ge.nicolike.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://qq.yuexingan06.cn

[Q36] 左连接
来源：http://jt.nicolike.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://pm.huixinmuqiang.cn

[Q37] 右连接
来源：http://kp.gzmigu.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://fn.panjiajie.cn

[Q38] 全外连接（PostgreSQL）
来源：http://vo.colortex.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://xt.asd995.cn

[Q39] 自连接（查上下级）
来源：http://qc.chemitech.net.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://xb.jianghongdianzi.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mk.newstarts.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://li.jctech888.com.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://cd.wgjwhj.cn

[Q41] 多表连接
来源：http://hg.9csxet.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://fw.jctech888.com.cn

JOIN users u ON u.id = o.user_id
来源：http://uh.hahajie.cn

JOIN products p ON p.id = o.product_id;
来源：http://ny.jctech888.com.cn

[Q42] 连接条件附加过滤
来源：http://ob.521024.cn

SELECT u.name, o.amount FROM users u
来源：http://ao.9csxet.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://pc.panjiajie.cn

[Q43] 标量子查询
来源：http://hr.yuntaijiaju.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://ls.huanxung.cn

[Q44] IN 子查询
来源：http://ig.asd995.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://fm.wgjwhj.cn

[Q45] EXISTS 判断存在
来源：http://ft.wgjwhj.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://rt.jianghongdianzi.cn

[Q46] NOT EXISTS 判断不存在
来源：http://lh.shtwfgs.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://kx.shtwfgs.cn

[Q47] 与平均值比较
来源：http://dk.huixiangedu.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://xa.bjjhwx.cn

[Q48] CTE 公用表表达式
来源：http://pg.hahajie.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wo.chemitech.net.cn

SELECT * FROM t WHERE c > 5;
来源：http://of.huixinmuqiang.cn

[Q49] 更新单行
来源：http://md.muxihuayi.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://pv.yuexingan06.cn

[Q50] 批量更新
来源：http://kg.colortex.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://dr.haigaiapp.cn

[Q51] 用子查询更新
来源：http://no.colortex.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://jc.bookmarksfly.cn

[Q52] 删除指定行
来源：http://ho.newstarts.cn

DELETE FROM users WHERE id = 10;
来源：http://zi.yuexingan06.cn

[Q53] 按条件删除
来源：http://qo.szsharing.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://zn.chemitech.net.cn

[Q54] 清空表
来源：http://kp.huixiangedu.cn

TRUNCATE TABLE logs;
来源：http://md.bookmarksfly.cn

[Q55] 排名（并列占位）
来源：http://na.szxytkj.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://fx.muxihuayi.cn

[Q56] 密集排名（并列不占位）
来源：http://rg.yuexingan06.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://jr.muxihuayi.cn

[Q57] 行号
来源：http://on.yuexingan06.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wj.huixinmuqiang.cn

[Q58] 累计求和
来源：http://pw.haigaiapp.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://dr.huixiangedu.cn

[Q59] 分组内累计
来源：http://ov.asd995.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://fe.asd995.cn

[Q60] 取上一行 / 下一行
来源：http://ly.hahajie.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mz.newstarts.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://jx.nicolike.cn

[Q61] 移动平均
来源：http://pt.shxzskj.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://di.bjjhwx.cn

[Q62] 分组占比
来源：http://sv.bjjhwx.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://dv.chemitech.net.cn

[Q63] 开启事务
来源：http://pc.jianghongdianzi.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://vs.szxytkj.cn

[Q64] 提交事务
来源：http://sz.lnxyls.cn

COMMIT;
来源：http://jq.haigaiapp.cn

[Q65] 回滚事务
来源：http://rb.huixiangedu.cn

ROLLBACK;
来源：http://vj.chemitech.net.cn

[Q66] 行锁查询
来源：http://ui.wgjwhj.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ar.nicolike.cn

[Q67] 设置隔离级别
来源：http://cy.521024.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://uq.asd995.cn

[Q68] 保存点
来源：http://qr.wgjwhj.cn

SAVEPOINT sp1;
来源：http://yk.yuexingan06.cn

ROLLBACK TO sp1;
来源：http://pv.szxytkj.cn

[Q69] 查看执行计划
来源：http://cq.huixiangedu.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ar.colortex.cn

[Q70] 更新统计信息
来源：http://uu.huanxung.cn

ANALYZE TABLE users;
来源：http://sw.hahajie.cn

[Q71] 查看建表语句
来源：http://hm.newstarts.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://pk.muxihuayi.cn

[Q72] 查看索引
来源：http://se.521024.cn

SHOW INDEX FROM users;
来源：http://pd.gzmigu.cn

[Q73] 查看表状态
来源：http://rh.yuntaijiaju.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://ox.nicolike.cn

[Q74] 强制使用索引
来源：http://cf.haigaiapp.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://la.szxytkj.cn

[Q75] 日期格式化
来源：http://zs.9csxet.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hp.shxzskj.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://gz.jctech888.com.cn

[Q76] 按天统计
来源：http://ml.wgjwhj.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hy.bjjhwx.cn

[Q77] 时间加减
来源：http://jv.szxytkj.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ua.jctech888.com.cn

[Q78] 当前时间
来源：http://bq.asd995.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wi.9csxet.cn

[Q79] 字符串拼接
来源：http://xg.bjjhwx.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://nr.yuntaijiaju.cn

[Q80] 字符串截取
来源：http://ej.lnxyls.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wh.bookmarksfly.cn

[Q81] 字符串替换
来源：http://rm.huixiangedu.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://bd.colortex.cn

[Q82] 字符长度与字节长度
来源：http://ey.shxzskj.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://vb.szxytkj.cn

[Q83] 大小写转换
来源：http://zf.chemitech.net.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://zm.9csxet.cn

[Q84] 去除首尾空格
来源：http://uc.hahajie.cn

SELECT TRIM(name) FROM users;
来源：http://ix.haigaiapp.cn

[Q85] 数值取整
来源：http://ku.huanxung.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://bg.szxytkj.cn

[Q86] 读取 JSON 字段
来源：http://qy.panjiajie.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://az.wgjwhj.cn

[Q87] JSON 字段做条件
来源：http://mi.huixinmuqiang.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ie.wgjwhj.cn

[Q88] 行转列（条件聚合）
来源：http://fy.shxzukj.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://rq.newstarts.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://rw.jctech888.com.cn

[Q89] 判断表是否存在
来源：http://wh.jianghongdianzi.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://qk.colortex.cn

[Q90] 生成序号列
来源：http://mo.9csxet.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ob.shxzukj.cn

================================================================================
来源：http://la.nszjky.cn

R. Bash 专题
来源：http://dv.panjiajie.cn

================================================================================
来源：http://na.asd995.cn

[R01] shebang 与严格模式
来源：http://lo.colortex.cn

#!/usr/bin/env bash
来源：http://ee.shxzukj.cn

set -euo pipefail
来源：http://yx.shxzskj.cn

[R02] 变量赋值与使用
来源：http://rj.wgjwhj.cn

name="Tom"; echo "$name"
来源：http://pf.newstarts.cn

[R03] 只读变量
来源：http://oo.haigaiapp.cn

readonly PI=3.14
来源：http://md.nszjky.cn

[R04] 位置参数
来源：http://cx.huanxung.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://bj.9csxet.cn

[R05] 参数默认值
来源：http://ew.jctech888.com.cn

name="${1:-default}"
来源：http://mq.yuntaijiaju.cn

[R06] 判断命令是否存在
来源：http://jt.hahajie.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://fp.jctech888.com.cn

[R07] if 判断文件
来源：http://vq.szsharing.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://vt.yuntaijiaju.cn

[R08] 数值比较
来源：http://ha.yuntaijiaju.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://br.jianghongdianzi.cn

[R09] 字符串比较
来源：http://qy.bjjhwx.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ax.hnjuh.cn

[R10] 正则匹配
来源：http://gv.hahajie.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hi.nicolike.cn

[R11] case 多分支
来源：http://br.hahajie.cn

case "$1" in
来源：http://ue.huixinmuqiang.cn

start) echo "启动" ;;
来源：http://sn.haigaiapp.cn

stop)  echo "停止" ;;
来源：http://vk.szxytkj.cn

*)     echo "未知命令" ;;
来源：http://mt.huixinmuqiang.cn

esac
来源：http://dg.hnjuh.cn

[R12] for 遍历文件
来源：http://ij.jianghongdianzi.cn

for f in *.txt; do echo "$f"; done
来源：http://pb.wgjwhj.cn

[R13] for 计数循环
来源：http://kn.chemitech.net.cn

for i in {1..10}; do echo "$i"; done
来源：http://jd.wgjwhj.cn

[R14] C 风格 for
来源：http://wb.bjjhwx.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ig.jianghongdianzi.cn

[R15] while 逐行读文件
来源：http://fz.colortex.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://zo.huanxung.cn

[R16] until 等待条件
来源：http://rl.shtwfgs.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://xb.asd995.cn

[R17] 数组定义与取值
来源：http://aa.haigaiapp.cn

arr=(a b c); echo "${arr[0]}"
来源：http://mj.shtwfgs.cn

[R18] 遍历数组
来源：http://ad.jianghongdianzi.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wj.shxzskj.cn

[R19] 数组长度
来源：http://pw.yuexingan06.cn

echo "${#arr[@]}"
来源：http://ne.nicolike.cn

[R20] 关联数组（字典）
来源：http://tt.asd995.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://eh.bjjhwx.cn

[R21] 字符串长度
来源：http://jb.huixinmuqiang.cn

echo "${#s}"
来源：http://mq.yuntaijiaju.cn

[R22] 截取子串
来源：http://lw.szsharing.cn

echo "${s:0:5}"
来源：http://to.asd995.cn

[R23] 字符串替换
来源：http://eg.nicolike.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://um.chemitech.net.cn

[R24] 大小写转换
来源：http://kv.jctech888.com.cn

echo "${s^^}"; echo "${s,,}"
来源：http://fn.szsharing.cn

[R25] 去后缀 / 去前缀
来源：http://rh.jianghongdianzi.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://fl.panjiajie.cn

[R26] 命令替换
来源：http://eu.hnjuh.cn

now=$(date +%F); echo "$now"
来源：http://bt.wgjwhj.cn

[R27] 算术展开
来源：http://xk.lnxyls.cn

echo $((1 + 2 * 3))
来源：http://hq.szxytkj.cn

[R28] 浮点运算
来源：http://qh.huixinmuqiang.cn

echo "scale=2; 10/3" | bc
来源：http://pi.hahajie.cn

[R29] 定义函数
来源：http://kr.521024.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://iz.nszjky.cn

[R30] 函数返回状态码
来源：http://bt.huanxung.cn

f() { return 0; }; f || echo "失败了"
来源：http://mc.nszjky.cn

[R31] 局部变量
来源：http://zb.panjiajie.cn

f() { local x=1; echo "$x"; }
来源：http://dg.jianghongdianzi.cn

[R32] 参数个数校验
来源：http://kq.huixiangedu.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://sx.panjiajie.cn

[R33] 捕获错误并提示行号
来源：http://rf.lnxyls.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://yf.jctech888.com.cn

[R34] 退出时清理
来源：http://vy.newstarts.cn

trap 'rm -f "$tmp"' EXIT
来源：http://pr.hnjuh.cn

[R35] 后台执行并等待
来源：http://vf.asd995.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://im.newstarts.cn

[R36] 并发执行多个任务
来源：http://bz.yuexingan06.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://sr.nicolike.cn

[R37] 把输出赋给变量
来源：http://su.yuexingan06.cn

files=$(ls -1)
来源：http://jd.yuntaijiaju.cn

[R38] 管道串联
来源：http://ai.yuntaijiaju.cn

cat a.txt | grep -i error | wc -l
来源：http://aq.yuntaijiaju.cn

[R39] 重定向标准输出与错误
来源：http://xz.szsharing.cn

cmd > out.log 2>&1
来源：http://cq.521024.cn

[R40] 追加写日志
来源：http://bo.szxytkj.cn

echo "log" >> out.log
来源：http://sj.shtwfgs.cn

[R41] 丢弃输出
来源：http://db.yuexingan06.cn

cmd >/dev/null 2>&1
来源：http://gz.szsharing.cn

[R42] 输入重定向
来源：http://hv.shtwfgs.cn

wc -l < a.txt
来源：http://af.wgjwhj.cn

[R43] 按名字查找文件
来源：http://jq.wgjwhj.cn

find . -name "*.log" -type f
来源：http://mc.shtwfgs.cn

[R44] 按修改时间查找
来源：http://bh.jianghongdianzi.cn

find . -mtime -7 -type f
来源：http://dm.yuntaijiaju.cn

[R45] 批量删除
来源：http://fg.hnjuh.cn

find . -name "*.tmp" -delete
来源：http://cg.wgjwhj.cn

[R46] 递归替换文件内容
来源：http://kl.newstarts.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://so.huixiangedu.cn

[R47] sed 单行替换
来源：http://mm.panjiajie.cn

sed -i 's/foo/bar/g' a.txt
来源：http://wb.shxzskj.cn

[R48] awk 取指定列
来源：http://sk.hnjuh.cn

awk '{print $1, $3}' a.txt
来源：http://vr.hahajie.cn

[R49] awk 带条件
来源：http://ab.yuntaijiaju.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hp.muxihuayi.cn

[R50] awk 求和
来源：http://lx.haigaiapp.cn

awk '{s += $2} END {print s}' a.txt
来源：http://zj.shtwfgs.cn

[R51] 排序去重取前几
来源：http://vc.szxytkj.cn


<!-- 参考信息 -->