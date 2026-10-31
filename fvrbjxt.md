代发 wailian999

);
来源：http://li.huanxung.cn

[Q03] 增加列
来源：http://rg.9csxet.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://qh.muxihuayi.cn

[Q04] 修改列类型
来源：http://zi.yuntaijiaju.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://aa.gzmigu.cn

[Q05] 重命名列
来源：http://pl.jctech888.com.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://tr.colortex.cn

[Q06] 删除列
来源：http://fv.gzmigu.cn

ALTER TABLE users DROP COLUMN age;
来源：http://fy.bjjhwx.cn

[Q07] 删除表
来源：http://jg.wgjwhj.cn

DROP TABLE IF EXISTS orders;
来源：http://xq.jctech888.com.cn

[Q08] 创建普通索引
来源：http://su.nszjky.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://zh.lnxyls.cn

[Q09] 创建唯一索引
来源：http://uo.shxzskj.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ug.wgjwhj.cn

[Q10] 插入单行
来源：http://fx.muxihuayi.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://tz.szxytkj.cn

[Q11] 一次插入多行
来源：http://zr.nicolike.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://bn.nszjky.cn

[Q12] 插入后取自增 ID
来源：http://bh.bjjhwx.cn

INSERT INTO users (name) VALUES ('C');
来源：http://ma.newstarts.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hg.521024.cn

[Q13] 忽略重复插入
来源：http://vp.asd995.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://yy.huixinmuqiang.cn

[Q14] 存在则更新（upsert）
来源：http://zi.lnxyls.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://vp.huanxung.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://yy.asd995.cn

[Q15] 查询全部
来源：http://jj.shtwfgs.cn

SELECT * FROM users;
来源：http://mo.lnxyls.cn

[Q16] 查询指定列
来源：http://at.shxzukj.cn

SELECT id, name FROM users;
来源：http://kj.shxzukj.cn

[Q17] 条件查询
来源：http://dj.shxzukj.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://zz.asd995.cn

[Q18] 模糊匹配
来源：http://gt.huixiangedu.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://vs.bjjhwx.cn

[Q19] 范围查询
来源：http://dh.nicolike.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ae.shxzskj.cn

[Q20] IN 列表
来源：http://cz.asd995.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://tl.huanxung.cn

[Q21] 空值判断
来源：http://cd.lnxyls.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://om.yuexingan06.cn

[Q22] 排序
来源：http://kp.shxzskj.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://op.newstarts.cn

[Q23] 分页
来源：http://bh.chemitech.net.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://tx.9csxet.cn

[Q24] 去重
来源：http://va.newstarts.cn

SELECT DISTINCT city FROM users;
来源：http://sq.szsharing.cn

[Q25] 只取前 N 条
来源：http://pc.muxihuayi.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://tv.chemitech.net.cn

[Q26] 计数
来源：http://zn.shtwfgs.cn

SELECT COUNT(*) FROM users;
来源：http://ul.colortex.cn

[Q27] 条件计数
来源：http://yg.shxzskj.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://fn.szsharing.cn

[Q28] 求和与平均
来源：http://mg.hnjuh.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://xe.newstarts.cn

[Q29] 最大最小值
来源：http://xe.yuntaijiaju.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://ns.asd995.cn

[Q30] 分组统计
来源：http://ue.huanxung.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://jj.szsharing.cn

[Q31] 分组后过滤
来源：http://mp.shtwfgs.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://bv.lnxyls.cn

[Q32] 分组拼接字符串
来源：http://pr.szsharing.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://qp.shxzskj.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://jj.gzmigu.cn

[Q33] 多列分组
来源：http://ek.nszjky.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://do.nszjky.cn

[Q34] 每组取第一条
来源：http://uz.haigaiapp.cn

SELECT * FROM (
来源：http://qi.yuntaijiaju.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://bm.colortex.cn

) t WHERE rn = 1;
来源：http://bs.jianghongdianzi.cn

[Q35] 内连接
来源：http://nt.newstarts.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://rz.9csxet.cn

[Q36] 左连接
来源：http://ds.gzmigu.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mm.muxihuayi.cn

[Q37] 右连接
来源：http://ac.szxytkj.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://jg.gzmigu.cn

[Q38] 全外连接（PostgreSQL）
来源：http://ey.panjiajie.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://af.lnxyls.cn

[Q39] 自连接（查上下级）
来源：http://ef.wgjwhj.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://oq.hahajie.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hu.nicolike.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://zj.huanxung.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ta.bookmarksfly.cn

[Q41] 多表连接
来源：http://us.yuntaijiaju.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://mn.nicolike.cn

JOIN users u ON u.id = o.user_id
来源：http://xu.hahajie.cn

JOIN products p ON p.id = o.product_id;
来源：http://ng.huixiangedu.cn

[Q42] 连接条件附加过滤
来源：http://lf.bookmarksfly.cn

SELECT u.name, o.amount FROM users u
来源：http://iu.hnjuh.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://rq.gzmigu.cn

[Q43] 标量子查询
来源：http://ja.nicolike.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wt.szxytkj.cn

[Q44] IN 子查询
来源：http://ha.jctech888.com.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ab.hahajie.cn

[Q45] EXISTS 判断存在
来源：http://ke.521024.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://gv.jctech888.com.cn

[Q46] NOT EXISTS 判断不存在
来源：http://if.hnjuh.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://id.nicolike.cn

[Q47] 与平均值比较
来源：http://ov.bookmarksfly.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://sx.huixiangedu.cn

[Q48] CTE 公用表表达式
来源：http://kj.panjiajie.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://cg.shxzukj.cn

SELECT * FROM t WHERE c > 5;
来源：http://cj.9csxet.cn

[Q49] 更新单行
来源：http://aw.jianghongdianzi.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://jb.lnxyls.cn

[Q50] 批量更新
来源：http://go.asd995.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mj.newstarts.cn

[Q51] 用子查询更新
来源：http://wv.bjjhwx.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://th.szxytkj.cn

[Q52] 删除指定行
来源：http://xy.jianghongdianzi.cn

DELETE FROM users WHERE id = 10;
来源：http://tg.asd995.cn

[Q53] 按条件删除
来源：http://zi.colortex.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://fs.huanxung.cn

[Q54] 清空表
来源：http://zt.jianghongdianzi.cn

TRUNCATE TABLE logs;
来源：http://qn.haigaiapp.cn

[Q55] 排名（并列占位）
来源：http://vh.shxzukj.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://kp.huixiangedu.cn

[Q56] 密集排名（并列不占位）
来源：http://tc.521024.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://fz.newstarts.cn

[Q57] 行号
来源：http://du.shtwfgs.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://jb.521024.cn

[Q58] 累计求和
来源：http://wi.huixiangedu.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ky.yuntaijiaju.cn

[Q59] 分组内累计
来源：http://he.hnjuh.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ql.hnjuh.cn

[Q60] 取上一行 / 下一行
来源：http://vt.szxytkj.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://uh.hahajie.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mi.muxihuayi.cn

[Q61] 移动平均
来源：http://fa.chemitech.net.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://aq.colortex.cn

[Q62] 分组占比
来源：http://hd.chemitech.net.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://zs.nszjky.cn

[Q63] 开启事务
来源：http://jr.nszjky.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://pv.gzmigu.cn

[Q64] 提交事务
来源：http://pq.newstarts.cn

COMMIT;
来源：http://pa.huixinmuqiang.cn

[Q65] 回滚事务
来源：http://uk.haigaiapp.cn

ROLLBACK;
来源：http://zq.panjiajie.cn

[Q66] 行锁查询
来源：http://ks.jianghongdianzi.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://xg.haigaiapp.cn

[Q67] 设置隔离级别
来源：http://rh.gzmigu.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://jc.nszjky.cn

[Q68] 保存点
来源：http://rq.chemitech.net.cn

SAVEPOINT sp1;
来源：http://ks.wgjwhj.cn

ROLLBACK TO sp1;
来源：http://cp.shxzskj.cn

[Q69] 查看执行计划
来源：http://oq.newstarts.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://fx.yuexingan06.cn

[Q70] 更新统计信息
来源：http://nz.521024.cn

ANALYZE TABLE users;
来源：http://gi.shxzukj.cn

[Q71] 查看建表语句
来源：http://fg.nszjky.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://tz.hnjuh.cn

[Q72] 查看索引
来源：http://ef.panjiajie.cn

SHOW INDEX FROM users;
来源：http://sb.9csxet.cn

[Q73] 查看表状态
来源：http://be.muxihuayi.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://xt.huanxung.cn

[Q74] 强制使用索引
来源：http://fw.szxytkj.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hh.521024.cn

[Q75] 日期格式化
来源：http://wd.shxzskj.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://bz.asd995.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://yl.chemitech.net.cn

[Q76] 按天统计
来源：http://lg.newstarts.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://el.jctech888.com.cn

[Q77] 时间加减
来源：http://pr.hnjuh.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ud.jctech888.com.cn

[Q78] 当前时间
来源：http://hx.9csxet.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://cq.nszjky.cn

[Q79] 字符串拼接
来源：http://of.gzmigu.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://lt.gzmigu.cn

[Q80] 字符串截取
来源：http://to.521024.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://aq.newstarts.cn

[Q81] 字符串替换
来源：http://er.hahajie.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://xy.wgjwhj.cn

[Q82] 字符长度与字节长度
来源：http://tw.lnxyls.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://xp.lnxyls.cn

[Q83] 大小写转换
来源：http://ya.lnxyls.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://cq.haigaiapp.cn

[Q84] 去除首尾空格
来源：http://je.wgjwhj.cn

SELECT TRIM(name) FROM users;
来源：http://tu.shtwfgs.cn

[Q85] 数值取整
来源：http://or.yuexingan06.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://lc.panjiajie.cn

[Q86] 读取 JSON 字段
来源：http://pf.hnjuh.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://lo.wgjwhj.cn

[Q87] JSON 字段做条件
来源：http://np.huanxung.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://tw.shtwfgs.cn

[Q88] 行转列（条件聚合）
来源：http://lg.nszjky.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mk.gzmigu.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ra.jctech888.com.cn

[Q89] 判断表是否存在
来源：http://pj.gzmigu.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://zn.yuntaijiaju.cn

[Q90] 生成序号列
来源：http://xf.bjjhwx.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://yd.panjiajie.cn

================================================================================
来源：http://hs.huanxung.cn

R. Bash 专题
来源：http://wm.yuexingan06.cn

================================================================================
来源：http://ce.yuexingan06.cn

[R01] shebang 与严格模式
来源：http://mr.panjiajie.cn

#!/usr/bin/env bash
来源：http://nr.gzmigu.cn

set -euo pipefail
来源：http://rj.huanxung.cn

[R02] 变量赋值与使用
来源：http://ae.nszjky.cn

name="Tom"; echo "$name"
来源：http://ey.nicolike.cn

[R03] 只读变量
来源：http://zi.panjiajie.cn

readonly PI=3.14
来源：http://tj.jctech888.com.cn

[R04] 位置参数
来源：http://td.shxzukj.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://nv.nicolike.cn

[R05] 参数默认值
来源：http://ph.bookmarksfly.cn

name="${1:-default}"
来源：http://av.szxytkj.cn

[R06] 判断命令是否存在
来源：http://sz.yuntaijiaju.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ru.lnxyls.cn

[R07] if 判断文件
来源：http://ra.colortex.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://og.haigaiapp.cn

[R08] 数值比较
来源：http://ud.huixiangedu.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://kh.jctech888.com.cn

[R09] 字符串比较
来源：http://ri.9csxet.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ge.panjiajie.cn

[R10] 正则匹配
来源：http://gj.yuntaijiaju.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://gv.lnxyls.cn

[R11] case 多分支
来源：http://ga.huixinmuqiang.cn

case "$1" in
来源：http://cd.panjiajie.cn

start) echo "启动" ;;
来源：http://gh.szxytkj.cn

stop)  echo "停止" ;;
来源：http://oh.shtwfgs.cn

*)     echo "未知命令" ;;
来源：http://ao.lnxyls.cn

esac
来源：http://xd.hahajie.cn

[R12] for 遍历文件
来源：http://to.jctech888.com.cn

for f in *.txt; do echo "$f"; done
来源：http://py.521024.cn

[R13] for 计数循环
来源：http://vc.panjiajie.cn

for i in {1..10}; do echo "$i"; done
来源：http://hj.jianghongdianzi.cn

[R14] C 风格 for
来源：http://nq.shtwfgs.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://gl.9csxet.cn

[R15] while 逐行读文件
来源：http://yv.hahajie.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://jj.lnxyls.cn

[R16] until 等待条件
来源：http://ki.colortex.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://nj.colortex.cn

[R17] 数组定义与取值
来源：http://ad.yuntaijiaju.cn

arr=(a b c); echo "${arr[0]}"
来源：http://yb.szsharing.cn

[R18] 遍历数组
来源：http://id.hnjuh.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://cy.521024.cn

[R19] 数组长度
来源：http://on.521024.cn

echo "${#arr[@]}"
来源：http://ui.haigaiapp.cn

[R20] 关联数组（字典）
来源：http://bc.shxzukj.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://oc.asd995.cn

[R21] 字符串长度
来源：http://zv.szsharing.cn

echo "${#s}"
来源：http://jg.gzmigu.cn

[R22] 截取子串
来源：http://dd.gzmigu.cn

echo "${s:0:5}"
来源：http://ht.bjjhwx.cn

[R23] 字符串替换
来源：http://da.nszjky.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://tg.jianghongdianzi.cn

[R24] 大小写转换
来源：http://en.shxzukj.cn

echo "${s^^}"; echo "${s,,}"
来源：http://hf.shtwfgs.cn

[R25] 去后缀 / 去前缀
来源：http://li.nszjky.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://mi.shtwfgs.cn

[R26] 命令替换
来源：http://ec.shtwfgs.cn

now=$(date +%F); echo "$now"
来源：http://vj.shtwfgs.cn

[R27] 算术展开
来源：http://qc.huanxung.cn

echo $((1 + 2 * 3))
来源：http://ci.jctech888.com.cn

[R28] 浮点运算
来源：http://em.panjiajie.cn

echo "scale=2; 10/3" | bc
来源：http://ax.bookmarksfly.cn

[R29] 定义函数
来源：http://ah.hnjuh.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ct.huixinmuqiang.cn

[R30] 函数返回状态码
来源：http://dg.colortex.cn

f() { return 0; }; f || echo "失败了"
来源：http://bh.521024.cn

[R31] 局部变量
来源：http://bm.lnxyls.cn

f() { local x=1; echo "$x"; }
来源：http://fs.haigaiapp.cn

[R32] 参数个数校验
来源：http://ch.huanxung.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://tn.huixiangedu.cn

[R33] 捕获错误并提示行号
来源：http://da.bjjhwx.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ag.9csxet.cn

[R34] 退出时清理
来源：http://ko.huixiangedu.cn

trap 'rm -f "$tmp"' EXIT
来源：http://fa.chemitech.net.cn

[R35] 后台执行并等待
来源：http://mz.haigaiapp.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://yw.lnxyls.cn

[R36] 并发执行多个任务
来源：http://af.yuexingan06.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://qo.9csxet.cn

[R37] 把输出赋给变量
来源：http://gi.asd995.cn

files=$(ls -1)
来源：http://pn.chemitech.net.cn

[R38] 管道串联
来源：http://mr.yuexingan06.cn

cat a.txt | grep -i error | wc -l
来源：http://jn.huixinmuqiang.cn

[R39] 重定向标准输出与错误
来源：http://yh.shtwfgs.cn

cmd > out.log 2>&1
来源：http://op.szsharing.cn

[R40] 追加写日志
来源：http://mn.nicolike.cn

echo "log" >> out.log
来源：http://gu.yuntaijiaju.cn

[R41] 丢弃输出
来源：http://lq.yuexingan06.cn

cmd >/dev/null 2>&1
来源：http://pn.hnjuh.cn

[R42] 输入重定向
来源：http://ks.jctech888.com.cn

wc -l < a.txt
来源：http://uy.shxzskj.cn

[R43] 按名字查找文件
来源：http://id.bookmarksfly.cn

find . -name "*.log" -type f
来源：http://eg.asd995.cn

[R44] 按修改时间查找
来源：http://ul.lnxyls.cn

find . -mtime -7 -type f
来源：http://rh.wgjwhj.cn

[R45] 批量删除
来源：http://gp.hahajie.cn

find . -name "*.tmp" -delete
来源：http://le.hahajie.cn

[R46] 递归替换文件内容
来源：http://zn.jianghongdianzi.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://cm.yuexingan06.cn

[R47] sed 单行替换
来源：http://uh.shxzukj.cn

sed -i 's/foo/bar/g' a.txt
来源：http://sp.szxytkj.cn

[R48] awk 取指定列
来源：http://rm.jianghongdianzi.cn

awk '{print $1, $3}' a.txt
来源：http://te.haigaiapp.cn

[R49] awk 带条件
来源：http://na.nicolike.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://jt.jctech888.com.cn

[R50] awk 求和
来源：http://bb.gzmigu.cn

awk '{s += $2} END {print s}' a.txt
来源：http://yn.muxihuayi.cn

[R51] 排序去重取前几
来源：http://iu.szsharing.cn


<!-- 参考信息 -->