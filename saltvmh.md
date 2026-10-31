代发 wailian999

);
来源：http://fh.yuntaijiaju.cn

[Q03] 增加列
来源：http://ig.hahajie.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ei.wgjwhj.cn

[Q04] 修改列类型
来源：http://yn.asd995.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://xq.panjiajie.cn

[Q05] 重命名列
来源：http://nn.huixiangedu.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hv.panjiajie.cn

[Q06] 删除列
来源：http://kr.jianghongdianzi.cn

ALTER TABLE users DROP COLUMN age;
来源：http://vz.yuntaijiaju.cn

[Q07] 删除表
来源：http://lv.jianghongdianzi.cn

DROP TABLE IF EXISTS orders;
来源：http://lp.newstarts.cn

[Q08] 创建普通索引
来源：http://vf.wgjwhj.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://wv.shtwfgs.cn

[Q09] 创建唯一索引
来源：http://ty.haigaiapp.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://yz.jianghongdianzi.cn

[Q10] 插入单行
来源：http://ul.szsharing.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://yn.szsharing.cn

[Q11] 一次插入多行
来源：http://ry.asd995.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ep.huixinmuqiang.cn

[Q12] 插入后取自增 ID
来源：http://ec.szsharing.cn

INSERT INTO users (name) VALUES ('C');
来源：http://vc.huixinmuqiang.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://rq.colortex.cn

[Q13] 忽略重复插入
来源：http://kr.bjjhwx.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://dg.lnxyls.cn

[Q14] 存在则更新（upsert）
来源：http://zw.huixinmuqiang.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ad.huanxung.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://zt.muxihuayi.cn

[Q15] 查询全部
来源：http://bi.huanxung.cn

SELECT * FROM users;
来源：http://oz.szsharing.cn

[Q16] 查询指定列
来源：http://fu.lnxyls.cn

SELECT id, name FROM users;
来源：http://gt.colortex.cn

[Q17] 条件查询
来源：http://xz.bookmarksfly.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://bg.bjjhwx.cn

[Q18] 模糊匹配
来源：http://bt.521024.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://yf.wgjwhj.cn

[Q19] 范围查询
来源：http://tw.muxihuayi.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://tq.huanxung.cn

[Q20] IN 列表
来源：http://hm.haigaiapp.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://dn.newstarts.cn

[Q21] 空值判断
来源：http://ve.panjiajie.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://zt.panjiajie.cn

[Q22] 排序
来源：http://yt.hnjuh.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://qj.huixinmuqiang.cn

[Q23] 分页
来源：http://nz.yuntaijiaju.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://yr.jianghongdianzi.cn

[Q24] 去重
来源：http://jx.jianghongdianzi.cn

SELECT DISTINCT city FROM users;
来源：http://mh.jianghongdianzi.cn

[Q25] 只取前 N 条
来源：http://kh.521024.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://oz.panjiajie.cn

[Q26] 计数
来源：http://wa.haigaiapp.cn

SELECT COUNT(*) FROM users;
来源：http://vz.hnjuh.cn

[Q27] 条件计数
来源：http://gj.huanxung.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wm.9csxet.cn

[Q28] 求和与平均
来源：http://zu.huanxung.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://de.521024.cn

[Q29] 最大最小值
来源：http://ka.yuntaijiaju.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://xf.wgjwhj.cn

[Q30] 分组统计
来源：http://hq.newstarts.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://zj.hahajie.cn

[Q31] 分组后过滤
来源：http://dz.nszjky.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://yh.bookmarksfly.cn

[Q32] 分组拼接字符串
来源：http://de.gzmigu.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://xf.szsharing.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://fe.gzmigu.cn

[Q33] 多列分组
来源：http://oh.haigaiapp.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mg.huanxung.cn

[Q34] 每组取第一条
来源：http://zk.chemitech.net.cn

SELECT * FROM (
来源：http://fo.huixiangedu.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://pb.szsharing.cn

) t WHERE rn = 1;
来源：http://yy.asd995.cn

[Q35] 内连接
来源：http://tg.muxihuayi.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ov.hnjuh.cn

[Q36] 左连接
来源：http://pa.gzmigu.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://cu.huixinmuqiang.cn

[Q37] 右连接
来源：http://xq.asd995.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://vb.bjjhwx.cn

[Q38] 全外连接（PostgreSQL）
来源：http://hh.jianghongdianzi.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ie.lnxyls.cn

[Q39] 自连接（查上下级）
来源：http://ii.haigaiapp.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://ne.bookmarksfly.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://sq.muxihuayi.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://kn.newstarts.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ui.gzmigu.cn

[Q41] 多表连接
来源：http://nw.nicolike.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://jc.521024.cn

JOIN users u ON u.id = o.user_id
来源：http://df.hahajie.cn

JOIN products p ON p.id = o.product_id;
来源：http://zu.hnjuh.cn

[Q42] 连接条件附加过滤
来源：http://il.nszjky.cn

SELECT u.name, o.amount FROM users u
来源：http://cl.shtwfgs.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mq.521024.cn

[Q43] 标量子查询
来源：http://pl.haigaiapp.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://gz.shtwfgs.cn

[Q44] IN 子查询
来源：http://gz.huanxung.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ns.lnxyls.cn

[Q45] EXISTS 判断存在
来源：http://jw.shtwfgs.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ap.shxzukj.cn

[Q46] NOT EXISTS 判断不存在
来源：http://kc.yuntaijiaju.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hv.muxihuayi.cn

[Q47] 与平均值比较
来源：http://kl.shxzukj.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://yt.jianghongdianzi.cn

[Q48] CTE 公用表表达式
来源：http://fi.huanxung.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://pv.chemitech.net.cn

SELECT * FROM t WHERE c > 5;
来源：http://xz.lnxyls.cn

[Q49] 更新单行
来源：http://pp.szxytkj.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://cj.huixiangedu.cn

[Q50] 批量更新
来源：http://ww.yuntaijiaju.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://fp.huanxung.cn

[Q51] 用子查询更新
来源：http://jy.yuexingan06.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://nn.shxzskj.cn

[Q52] 删除指定行
来源：http://nq.nszjky.cn

DELETE FROM users WHERE id = 10;
来源：http://hr.asd995.cn

[Q53] 按条件删除
来源：http://ru.colortex.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://gb.shxzukj.cn

[Q54] 清空表
来源：http://me.nicolike.cn

TRUNCATE TABLE logs;
来源：http://na.newstarts.cn

[Q55] 排名（并列占位）
来源：http://fa.shtwfgs.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://fv.jctech888.com.cn

[Q56] 密集排名（并列不占位）
来源：http://ou.chemitech.net.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://no.9csxet.cn

[Q57] 行号
来源：http://np.shxzskj.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ww.nszjky.cn

[Q58] 累计求和
来源：http://hn.521024.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://fq.muxihuayi.cn

[Q59] 分组内累计
来源：http://zw.asd995.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://nd.colortex.cn

[Q60] 取上一行 / 下一行
来源：http://uc.shtwfgs.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://nh.bookmarksfly.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ae.huixiangedu.cn

[Q61] 移动平均
来源：http://ul.huanxung.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ln.521024.cn

[Q62] 分组占比
来源：http://kw.hahajie.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://db.lnxyls.cn

[Q63] 开启事务
来源：http://rr.asd995.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://tm.gzmigu.cn

[Q64] 提交事务
来源：http://gw.newstarts.cn

COMMIT;
来源：http://jd.hahajie.cn

[Q65] 回滚事务
来源：http://vx.gzmigu.cn

ROLLBACK;
来源：http://yz.hahajie.cn

[Q66] 行锁查询
来源：http://nf.yuexingan06.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://za.shxzukj.cn

[Q67] 设置隔离级别
来源：http://um.chemitech.net.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://do.colortex.cn

[Q68] 保存点
来源：http://fx.chemitech.net.cn

SAVEPOINT sp1;
来源：http://ys.szxytkj.cn

ROLLBACK TO sp1;
来源：http://aj.shxzukj.cn

[Q69] 查看执行计划
来源：http://ji.hahajie.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://yd.nicolike.cn

[Q70] 更新统计信息
来源：http://vt.szsharing.cn

ANALYZE TABLE users;
来源：http://ln.bookmarksfly.cn

[Q71] 查看建表语句
来源：http://ve.szxytkj.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://bp.hnjuh.cn

[Q72] 查看索引
来源：http://ol.muxihuayi.cn

SHOW INDEX FROM users;
来源：http://cq.nszjky.cn

[Q73] 查看表状态
来源：http://ii.muxihuayi.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://gw.haigaiapp.cn

[Q74] 强制使用索引
来源：http://vz.huanxung.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://df.521024.cn

[Q75] 日期格式化
来源：http://vx.bjjhwx.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ne.panjiajie.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ga.szxytkj.cn

[Q76] 按天统计
来源：http://az.huanxung.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ig.haigaiapp.cn

[Q77] 时间加减
来源：http://sc.nszjky.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://yd.jctech888.com.cn

[Q78] 当前时间
来源：http://bq.huixiangedu.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://pn.szsharing.cn

[Q79] 字符串拼接
来源：http://en.szxytkj.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://sw.hnjuh.cn

[Q80] 字符串截取
来源：http://kx.nszjky.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wm.panjiajie.cn

[Q81] 字符串替换
来源：http://xo.521024.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ps.huanxung.cn

[Q82] 字符长度与字节长度
来源：http://se.shtwfgs.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://we.nszjky.cn

[Q83] 大小写转换
来源：http://cv.lnxyls.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://tn.bjjhwx.cn

[Q84] 去除首尾空格
来源：http://jx.yuntaijiaju.cn

SELECT TRIM(name) FROM users;
来源：http://ow.yuntaijiaju.cn

[Q85] 数值取整
来源：http://tc.nicolike.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://zl.huanxung.cn

[Q86] 读取 JSON 字段
来源：http://bm.yuexingan06.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ac.nszjky.cn

[Q87] JSON 字段做条件
来源：http://da.jctech888.com.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://pz.lnxyls.cn

[Q88] 行转列（条件聚合）
来源：http://tc.chemitech.net.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://tf.bjjhwx.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mb.jianghongdianzi.cn

[Q89] 判断表是否存在
来源：http://fi.newstarts.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://tg.bookmarksfly.cn

[Q90] 生成序号列
来源：http://gw.huixinmuqiang.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://uk.yuntaijiaju.cn

================================================================================
来源：http://wt.yuexingan06.cn

R. Bash 专题
来源：http://dj.chemitech.net.cn

================================================================================
来源：http://pp.haigaiapp.cn

[R01] shebang 与严格模式
来源：http://lh.bookmarksfly.cn

#!/usr/bin/env bash
来源：http://qz.chemitech.net.cn

set -euo pipefail
来源：http://ha.nszjky.cn

[R02] 变量赋值与使用
来源：http://ug.colortex.cn

name="Tom"; echo "$name"
来源：http://em.szsharing.cn

[R03] 只读变量
来源：http://sb.shtwfgs.cn

readonly PI=3.14
来源：http://nf.haigaiapp.cn

[R04] 位置参数
来源：http://sz.huanxung.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://qc.chemitech.net.cn

[R05] 参数默认值
来源：http://gu.shtwfgs.cn

name="${1:-default}"
来源：http://dq.hahajie.cn

[R06] 判断命令是否存在
来源：http://tg.shxzskj.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://zx.bookmarksfly.cn

[R07] if 判断文件
来源：http://gz.huixinmuqiang.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://eu.haigaiapp.cn

[R08] 数值比较
来源：http://co.shxzskj.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://dx.9csxet.cn

[R09] 字符串比较
来源：http://kt.newstarts.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ng.jianghongdianzi.cn

[R10] 正则匹配
来源：http://bj.nszjky.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wp.nszjky.cn

[R11] case 多分支
来源：http://xm.9csxet.cn

case "$1" in
来源：http://bd.szsharing.cn

start) echo "启动" ;;
来源：http://bh.hnjuh.cn

stop)  echo "停止" ;;
来源：http://dj.nszjky.cn

*)     echo "未知命令" ;;
来源：http://va.jctech888.com.cn

esac
来源：http://oq.huanxung.cn

[R12] for 遍历文件
来源：http://et.huixinmuqiang.cn

for f in *.txt; do echo "$f"; done
来源：http://ly.521024.cn

[R13] for 计数循环
来源：http://ew.gzmigu.cn

for i in {1..10}; do echo "$i"; done
来源：http://sh.bjjhwx.cn

[R14] C 风格 for
来源：http://ti.newstarts.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://he.colortex.cn

[R15] while 逐行读文件
来源：http://fk.muxihuayi.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://xp.wgjwhj.cn

[R16] until 等待条件
来源：http://jw.huixiangedu.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://so.shxzukj.cn

[R17] 数组定义与取值
来源：http://aw.huixiangedu.cn

arr=(a b c); echo "${arr[0]}"
来源：http://xq.gzmigu.cn

[R18] 遍历数组
来源：http://wb.hahajie.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://lq.colortex.cn

[R19] 数组长度
来源：http://uk.nszjky.cn

echo "${#arr[@]}"
来源：http://xe.huixinmuqiang.cn

[R20] 关联数组（字典）
来源：http://dv.asd995.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hv.shtwfgs.cn

[R21] 字符串长度
来源：http://tg.huanxung.cn

echo "${#s}"
来源：http://jv.521024.cn

[R22] 截取子串
来源：http://rs.newstarts.cn

echo "${s:0:5}"
来源：http://qe.shtwfgs.cn

[R23] 字符串替换
来源：http://un.bjjhwx.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://sy.lnxyls.cn

[R24] 大小写转换
来源：http://ug.shxzukj.cn

echo "${s^^}"; echo "${s,,}"
来源：http://wt.gzmigu.cn

[R25] 去后缀 / 去前缀
来源：http://yl.jctech888.com.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://oc.huanxung.cn

[R26] 命令替换
来源：http://vl.yuexingan06.cn

now=$(date +%F); echo "$now"
来源：http://va.wgjwhj.cn

[R27] 算术展开
来源：http://wd.9csxet.cn

echo $((1 + 2 * 3))
来源：http://cq.panjiajie.cn

[R28] 浮点运算
来源：http://sz.521024.cn

echo "scale=2; 10/3" | bc
来源：http://wd.yuexingan06.cn

[R29] 定义函数
来源：http://dn.panjiajie.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mn.bookmarksfly.cn

[R30] 函数返回状态码
来源：http://qz.521024.cn

f() { return 0; }; f || echo "失败了"
来源：http://lt.lnxyls.cn

[R31] 局部变量
来源：http://dj.newstarts.cn

f() { local x=1; echo "$x"; }
来源：http://xt.hahajie.cn

[R32] 参数个数校验
来源：http://rh.gzmigu.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ci.muxihuayi.cn

[R33] 捕获错误并提示行号
来源：http://ce.wgjwhj.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://aw.muxihuayi.cn

[R34] 退出时清理
来源：http://mn.9csxet.cn

trap 'rm -f "$tmp"' EXIT
来源：http://wd.yuexingan06.cn

[R35] 后台执行并等待
来源：http://xw.shtwfgs.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://hj.huixiangedu.cn

[R36] 并发执行多个任务
来源：http://ul.chemitech.net.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://cs.muxihuayi.cn

[R37] 把输出赋给变量
来源：http://qt.haigaiapp.cn

files=$(ls -1)
来源：http://we.shtwfgs.cn

[R38] 管道串联
来源：http://dw.szxytkj.cn

cat a.txt | grep -i error | wc -l
来源：http://fh.szsharing.cn

[R39] 重定向标准输出与错误
来源：http://va.colortex.cn

cmd > out.log 2>&1
来源：http://xj.yuntaijiaju.cn

[R40] 追加写日志
来源：http://dc.hnjuh.cn

echo "log" >> out.log
来源：http://pj.panjiajie.cn

[R41] 丢弃输出
来源：http://ph.huixiangedu.cn

cmd >/dev/null 2>&1
来源：http://ux.szsharing.cn

[R42] 输入重定向
来源：http://gm.hahajie.cn

wc -l < a.txt
来源：http://le.521024.cn

[R43] 按名字查找文件
来源：http://wy.asd995.cn

find . -name "*.log" -type f
来源：http://ul.gzmigu.cn

[R44] 按修改时间查找
来源：http://hg.nszjky.cn

find . -mtime -7 -type f
来源：http://ls.lnxyls.cn

[R45] 批量删除
来源：http://vl.szxytkj.cn

find . -name "*.tmp" -delete
来源：http://ds.colortex.cn

[R46] 递归替换文件内容
来源：http://fl.bjjhwx.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://tm.szxytkj.cn

[R47] sed 单行替换
来源：http://hy.huanxung.cn

sed -i 's/foo/bar/g' a.txt
来源：http://iu.panjiajie.cn

[R48] awk 取指定列
来源：http://nw.nszjky.cn

awk '{print $1, $3}' a.txt
来源：http://ep.colortex.cn

[R49] awk 带条件
来源：http://wu.bookmarksfly.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ws.bookmarksfly.cn

[R50] awk 求和
来源：http://kp.huixinmuqiang.cn

awk '{s += $2} END {print s}' a.txt
来源：http://ar.yuexingan06.cn

[R51] 排序去重取前几
来源：http://gn.panjiajie.cn


<!-- 参考信息 -->