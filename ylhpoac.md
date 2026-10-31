代发 wailian999

);
来源：http://xf.nicolike.cn

[Q03] 增加列
来源：http://qm.chemitech.net.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://lr.shxzukj.cn

[Q04] 修改列类型
来源：http://mv.szsharing.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://zi.colortex.cn

[Q05] 重命名列
来源：http://yf.yuexingan06.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://to.colortex.cn

[Q06] 删除列
来源：http://kn.szsharing.cn

ALTER TABLE users DROP COLUMN age;
来源：http://fd.lnxyls.cn

[Q07] 删除表
来源：http://od.shtwfgs.cn

DROP TABLE IF EXISTS orders;
来源：http://tq.nicolike.cn

[Q08] 创建普通索引
来源：http://fl.asd995.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://gt.szsharing.cn

[Q09] 创建唯一索引
来源：http://te.muxihuayi.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://an.newstarts.cn

[Q10] 插入单行
来源：http://vb.hnjuh.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://zq.yuexingan06.cn

[Q11] 一次插入多行
来源：http://gw.shxzskj.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://vj.muxihuayi.cn

[Q12] 插入后取自增 ID
来源：http://me.yuntaijiaju.cn

INSERT INTO users (name) VALUES ('C');
来源：http://qs.huixiangedu.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://zt.nicolike.cn

[Q13] 忽略重复插入
来源：http://ah.muxihuayi.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://bx.9csxet.cn

[Q14] 存在则更新（upsert）
来源：http://mo.colortex.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ay.huanxung.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ul.nicolike.cn

[Q15] 查询全部
来源：http://fg.nicolike.cn

SELECT * FROM users;
来源：http://tu.nszjky.cn

[Q16] 查询指定列
来源：http://qz.asd995.cn

SELECT id, name FROM users;
来源：http://rg.hnjuh.cn

[Q17] 条件查询
来源：http://ou.bookmarksfly.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ik.newstarts.cn

[Q18] 模糊匹配
来源：http://lf.9csxet.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ha.newstarts.cn

[Q19] 范围查询
来源：http://gc.jianghongdianzi.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://pq.gzmigu.cn

[Q20] IN 列表
来源：http://be.yuntaijiaju.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://df.chemitech.net.cn

[Q21] 空值判断
来源：http://ny.muxihuayi.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://mj.shtwfgs.cn

[Q22] 排序
来源：http://mg.newstarts.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://sw.szxytkj.cn

[Q23] 分页
来源：http://kt.asd995.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://xg.521024.cn

[Q24] 去重
来源：http://ld.szxytkj.cn

SELECT DISTINCT city FROM users;
来源：http://jz.huixinmuqiang.cn

[Q25] 只取前 N 条
来源：http://cr.chemitech.net.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ps.shtwfgs.cn

[Q26] 计数
来源：http://nk.huixinmuqiang.cn

SELECT COUNT(*) FROM users;
来源：http://ke.shtwfgs.cn

[Q27] 条件计数
来源：http://ei.jianghongdianzi.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://cb.newstarts.cn

[Q28] 求和与平均
来源：http://cm.huixinmuqiang.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://ez.jianghongdianzi.cn

[Q29] 最大最小值
来源：http://ee.szxytkj.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://tj.yuexingan06.cn

[Q30] 分组统计
来源：http://fh.colortex.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://av.huanxung.cn

[Q31] 分组后过滤
来源：http://cr.yuntaijiaju.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://vh.wgjwhj.cn

[Q32] 分组拼接字符串
来源：http://we.wgjwhj.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://df.yuntaijiaju.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ao.lnxyls.cn

[Q33] 多列分组
来源：http://cy.9csxet.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://xj.muxihuayi.cn

[Q34] 每组取第一条
来源：http://bn.9csxet.cn

SELECT * FROM (
来源：http://eo.gzmigu.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ci.lnxyls.cn

) t WHERE rn = 1;
来源：http://ip.bookmarksfly.cn

[Q35] 内连接
来源：http://dv.lnxyls.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ze.muxihuayi.cn

[Q36] 左连接
来源：http://wz.colortex.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://tq.colortex.cn

[Q37] 右连接
来源：http://zx.yuntaijiaju.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://pj.colortex.cn

[Q38] 全外连接（PostgreSQL）
来源：http://qc.szsharing.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://cu.nicolike.cn

[Q39] 自连接（查上下级）
来源：http://dc.wgjwhj.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://im.shxzukj.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://lj.asd995.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://pw.wgjwhj.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://al.shxzukj.cn

[Q41] 多表连接
来源：http://yi.huanxung.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://ht.jianghongdianzi.cn

JOIN users u ON u.id = o.user_id
来源：http://ts.hahajie.cn

JOIN products p ON p.id = o.product_id;
来源：http://dy.huixiangedu.cn

[Q42] 连接条件附加过滤
来源：http://cs.newstarts.cn

SELECT u.name, o.amount FROM users u
来源：http://jl.huanxung.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ez.yuntaijiaju.cn

[Q43] 标量子查询
来源：http://dq.jianghongdianzi.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://gg.huanxung.cn

[Q44] IN 子查询
来源：http://jj.gzmigu.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://oe.huanxung.cn

[Q45] EXISTS 判断存在
来源：http://eu.szxytkj.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://sl.newstarts.cn

[Q46] NOT EXISTS 判断不存在
来源：http://yo.muxihuayi.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://kt.shxzukj.cn

[Q47] 与平均值比较
来源：http://mj.chemitech.net.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://sz.yuexingan06.cn

[Q48] CTE 公用表表达式
来源：http://dk.nszjky.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ws.lnxyls.cn

SELECT * FROM t WHERE c > 5;
来源：http://bq.nszjky.cn

[Q49] 更新单行
来源：http://pe.hnjuh.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://fh.gzmigu.cn

[Q50] 批量更新
来源：http://wo.hahajie.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hn.jianghongdianzi.cn

[Q51] 用子查询更新
来源：http://wd.shxzukj.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hd.shxzukj.cn

[Q52] 删除指定行
来源：http://oy.yuntaijiaju.cn

DELETE FROM users WHERE id = 10;
来源：http://hc.shxzukj.cn

[Q53] 按条件删除
来源：http://oj.szxytkj.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wg.huanxung.cn

[Q54] 清空表
来源：http://oz.nicolike.cn

TRUNCATE TABLE logs;
来源：http://xo.bookmarksfly.cn

[Q55] 排名（并列占位）
来源：http://lh.asd995.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://xs.nicolike.cn

[Q56] 密集排名（并列不占位）
来源：http://wg.yuntaijiaju.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://dh.yuntaijiaju.cn

[Q57] 行号
来源：http://lg.szsharing.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://lr.jctech888.com.cn

[Q58] 累计求和
来源：http://qp.muxihuayi.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://df.gzmigu.cn

[Q59] 分组内累计
来源：http://pk.chemitech.net.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://et.muxihuayi.cn

[Q60] 取上一行 / 下一行
来源：http://ci.huixinmuqiang.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://tw.huanxung.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://im.shxzskj.cn

[Q61] 移动平均
来源：http://xh.haigaiapp.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ij.shxzskj.cn

[Q62] 分组占比
来源：http://dr.9csxet.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://gu.bookmarksfly.cn

[Q63] 开启事务
来源：http://vp.asd995.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://dh.shxzukj.cn

[Q64] 提交事务
来源：http://ly.shxzskj.cn

COMMIT;
来源：http://yp.shxzskj.cn

[Q65] 回滚事务
来源：http://vp.jianghongdianzi.cn

ROLLBACK;
来源：http://dv.yuexingan06.cn

[Q66] 行锁查询
来源：http://ne.lnxyls.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://yd.yuntaijiaju.cn

[Q67] 设置隔离级别
来源：http://tg.nszjky.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://gz.yuntaijiaju.cn

[Q68] 保存点
来源：http://ef.bookmarksfly.cn

SAVEPOINT sp1;
来源：http://lz.bookmarksfly.cn

ROLLBACK TO sp1;
来源：http://kg.colortex.cn

[Q69] 查看执行计划
来源：http://ft.huanxung.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://lw.shxzukj.cn

[Q70] 更新统计信息
来源：http://yf.521024.cn

ANALYZE TABLE users;
来源：http://ic.shxzukj.cn

[Q71] 查看建表语句
来源：http://ft.muxihuayi.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://no.bjjhwx.cn

[Q72] 查看索引
来源：http://zb.wgjwhj.cn

SHOW INDEX FROM users;
来源：http://nd.bjjhwx.cn

[Q73] 查看表状态
来源：http://jh.nszjky.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://cy.bookmarksfly.cn

[Q74] 强制使用索引
来源：http://hc.jianghongdianzi.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://pb.hahajie.cn

[Q75] 日期格式化
来源：http://qr.bookmarksfly.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ts.muxihuayi.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://rk.muxihuayi.cn

[Q76] 按天统计
来源：http://ly.shxzukj.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://nu.chemitech.net.cn

[Q77] 时间加减
来源：http://pq.wgjwhj.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://up.hahajie.cn

[Q78] 当前时间
来源：http://sb.gzmigu.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://tn.haigaiapp.cn

[Q79] 字符串拼接
来源：http://sz.panjiajie.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://pz.521024.cn

[Q80] 字符串截取
来源：http://op.nszjky.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://me.newstarts.cn

[Q81] 字符串替换
来源：http://ri.jctech888.com.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://gk.huixiangedu.cn

[Q82] 字符长度与字节长度
来源：http://rp.521024.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ch.nicolike.cn

[Q83] 大小写转换
来源：http://yr.bjjhwx.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ab.asd995.cn

[Q84] 去除首尾空格
来源：http://fa.jianghongdianzi.cn

SELECT TRIM(name) FROM users;
来源：http://in.huixinmuqiang.cn

[Q85] 数值取整
来源：http://md.yuexingan06.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ig.nicolike.cn

[Q86] 读取 JSON 字段
来源：http://ht.huanxung.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://sg.muxihuayi.cn

[Q87] JSON 字段做条件
来源：http://ly.huixinmuqiang.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ig.nicolike.cn

[Q88] 行转列（条件聚合）
来源：http://dk.bookmarksfly.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://cr.shxzskj.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://qa.bookmarksfly.cn

[Q89] 判断表是否存在
来源：http://dw.shxzskj.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://zg.gzmigu.cn

[Q90] 生成序号列
来源：http://gj.lnxyls.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ko.jianghongdianzi.cn

================================================================================
来源：http://mu.jianghongdianzi.cn

R. Bash 专题
来源：http://bd.9csxet.cn

================================================================================
来源：http://rf.chemitech.net.cn

[R01] shebang 与严格模式
来源：http://nd.chemitech.net.cn

#!/usr/bin/env bash
来源：http://so.nicolike.cn

set -euo pipefail
来源：http://rq.shtwfgs.cn

[R02] 变量赋值与使用
来源：http://oy.szxytkj.cn

name="Tom"; echo "$name"
来源：http://vd.lnxyls.cn

[R03] 只读变量
来源：http://ot.jctech888.com.cn

readonly PI=3.14
来源：http://lx.gzmigu.cn

[R04] 位置参数
来源：http://za.jianghongdianzi.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://oj.nicolike.cn

[R05] 参数默认值
来源：http://uc.shxzskj.cn

name="${1:-default}"
来源：http://cm.bjjhwx.cn

[R06] 判断命令是否存在
来源：http://tv.lnxyls.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://uo.huixiangedu.cn

[R07] if 判断文件
来源：http://bn.newstarts.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://vm.huanxung.cn

[R08] 数值比较
来源：http://sy.huixinmuqiang.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://yx.shxzukj.cn

[R09] 字符串比较
来源：http://fj.521024.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wy.colortex.cn

[R10] 正则匹配
来源：http://ww.shtwfgs.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://oi.asd995.cn

[R11] case 多分支
来源：http://lq.nicolike.cn

case "$1" in
来源：http://sv.nicolike.cn

start) echo "启动" ;;
来源：http://nz.huanxung.cn

stop)  echo "停止" ;;
来源：http://un.colortex.cn

*)     echo "未知命令" ;;
来源：http://im.nicolike.cn

esac
来源：http://ij.shxzukj.cn

[R12] for 遍历文件
来源：http://rx.nszjky.cn

for f in *.txt; do echo "$f"; done
来源：http://gc.colortex.cn

[R13] for 计数循环
来源：http://vt.521024.cn

for i in {1..10}; do echo "$i"; done
来源：http://ja.nicolike.cn

[R14] C 风格 for
来源：http://mv.colortex.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://vw.bookmarksfly.cn

[R15] while 逐行读文件
来源：http://wf.nszjky.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://af.huanxung.cn

[R16] until 等待条件
来源：http://dx.bookmarksfly.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://on.huixiangedu.cn

[R17] 数组定义与取值
来源：http://jj.521024.cn

arr=(a b c); echo "${arr[0]}"
来源：http://fp.nszjky.cn

[R18] 遍历数组
来源：http://ka.yuntaijiaju.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://rv.haigaiapp.cn

[R19] 数组长度
来源：http://fc.gzmigu.cn

echo "${#arr[@]}"
来源：http://nu.yuexingan06.cn

[R20] 关联数组（字典）
来源：http://qv.shxzskj.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://kt.newstarts.cn

[R21] 字符串长度
来源：http://hw.chemitech.net.cn

echo "${#s}"
来源：http://nf.9csxet.cn

[R22] 截取子串
来源：http://vo.shtwfgs.cn

echo "${s:0:5}"
来源：http://di.shtwfgs.cn

[R23] 字符串替换
来源：http://hp.szxytkj.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://zx.bookmarksfly.cn

[R24] 大小写转换
来源：http://vv.lnxyls.cn

echo "${s^^}"; echo "${s,,}"
来源：http://sq.nszjky.cn

[R25] 去后缀 / 去前缀
来源：http://hu.muxihuayi.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://nc.yuntaijiaju.cn

[R26] 命令替换
来源：http://kp.shtwfgs.cn

now=$(date +%F); echo "$now"
来源：http://ar.szsharing.cn

[R27] 算术展开
来源：http://wc.szxytkj.cn

echo $((1 + 2 * 3))
来源：http://lv.jctech888.com.cn

[R28] 浮点运算
来源：http://es.huanxung.cn

echo "scale=2; 10/3" | bc
来源：http://sa.colortex.cn

[R29] 定义函数
来源：http://np.9csxet.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ed.yuexingan06.cn

[R30] 函数返回状态码
来源：http://mf.huixinmuqiang.cn

f() { return 0; }; f || echo "失败了"
来源：http://nf.jianghongdianzi.cn

[R31] 局部变量
来源：http://xf.huixinmuqiang.cn

f() { local x=1; echo "$x"; }
来源：http://bk.hnjuh.cn

[R32] 参数个数校验
来源：http://jg.muxihuayi.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://jh.gzmigu.cn

[R33] 捕获错误并提示行号
来源：http://hg.haigaiapp.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://rj.bjjhwx.cn

[R34] 退出时清理
来源：http://lo.lnxyls.cn

trap 'rm -f "$tmp"' EXIT
来源：http://sv.colortex.cn

[R35] 后台执行并等待
来源：http://kv.9csxet.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://hy.9csxet.cn

[R36] 并发执行多个任务
来源：http://iv.bjjhwx.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://oe.521024.cn

[R37] 把输出赋给变量
来源：http://wo.yuexingan06.cn

files=$(ls -1)
来源：http://tf.nicolike.cn

[R38] 管道串联
来源：http://it.shxzukj.cn

cat a.txt | grep -i error | wc -l
来源：http://ru.asd995.cn

[R39] 重定向标准输出与错误
来源：http://xx.bookmarksfly.cn

cmd > out.log 2>&1
来源：http://tp.haigaiapp.cn

[R40] 追加写日志
来源：http://eq.colortex.cn

echo "log" >> out.log
来源：http://rb.bjjhwx.cn

[R41] 丢弃输出
来源：http://ff.nicolike.cn

cmd >/dev/null 2>&1
来源：http://xn.szsharing.cn

[R42] 输入重定向
来源：http://sm.nicolike.cn

wc -l < a.txt
来源：http://nw.panjiajie.cn

[R43] 按名字查找文件
来源：http://uz.shxzukj.cn

find . -name "*.log" -type f
来源：http://ji.nszjky.cn

[R44] 按修改时间查找
来源：http://gb.hnjuh.cn

find . -mtime -7 -type f
来源：http://vl.szsharing.cn

[R45] 批量删除
来源：http://ji.shxzskj.cn

find . -name "*.tmp" -delete
来源：http://jl.szsharing.cn

[R46] 递归替换文件内容
来源：http://ja.shtwfgs.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://li.jctech888.com.cn

[R47] sed 单行替换
来源：http://sl.muxihuayi.cn

sed -i 's/foo/bar/g' a.txt
来源：http://zc.shxzukj.cn

[R48] awk 取指定列
来源：http://ns.huixiangedu.cn

awk '{print $1, $3}' a.txt
来源：http://jq.huixiangedu.cn

[R49] awk 带条件
来源：http://rn.newstarts.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://nc.bjjhwx.cn

[R50] awk 求和
来源：http://qi.521024.cn

awk '{s += $2} END {print s}' a.txt
来源：http://ij.nszjky.cn

[R51] 排序去重取前几
来源：http://an.panjiajie.cn


<!-- 参考信息 -->