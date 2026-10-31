代发 wailian999

ALTER TABLE users DROP COLUMN age;
来源：http://nx.hnjuh.cn

[Q07] 删除表
来源：http://fo.chemitech.net.cn

DROP TABLE IF EXISTS orders;
来源：http://wl.huixiangedu.cn

[Q08] 创建普通索引
来源：http://vx.chemitech.net.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://du.gzmigu.cn

[Q09] 创建唯一索引
来源：http://zh.shxzskj.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://yp.colortex.cn

[Q10] 插入单行
来源：http://pp.hahajie.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://zt.nicolike.cn

[Q11] 一次插入多行
来源：http://ql.bjjhwx.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://lz.wgjwhj.cn

[Q12] 插入后取自增 ID
来源：http://hk.chemitech.net.cn

INSERT INTO users (name) VALUES ('C');
来源：http://wl.panjiajie.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://gc.yuntaijiaju.cn

[Q13] 忽略重复插入
来源：http://ib.yuexingan06.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ux.shxzukj.cn

[Q14] 存在则更新（upsert）
来源：http://oi.chemitech.net.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://bq.muxihuayi.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://sg.jianghongdianzi.cn

[Q15] 查询全部
来源：http://lf.szxytkj.cn

SELECT * FROM users;
来源：http://bi.bookmarksfly.cn

[Q16] 查询指定列
来源：http://ld.huixinmuqiang.cn

SELECT id, name FROM users;
来源：http://pl.huanxung.cn

[Q17] 条件查询
来源：http://co.shtwfgs.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://zn.521024.cn

[Q18] 模糊匹配
来源：http://kj.521024.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ku.shxzukj.cn

[Q19] 范围查询
来源：http://xe.shxzskj.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ss.hahajie.cn

[Q20] IN 列表
来源：http://el.nszjky.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://tr.lnxyls.cn

[Q21] 空值判断
来源：http://cy.nicolike.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://qf.hnjuh.cn

[Q22] 排序
来源：http://pe.jctech888.com.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://aj.huanxung.cn

[Q23] 分页
来源：http://ss.huixinmuqiang.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://xi.lnxyls.cn

[Q24] 去重
来源：http://ok.huixiangedu.cn

SELECT DISTINCT city FROM users;
来源：http://lt.yuntaijiaju.cn

[Q25] 只取前 N 条
来源：http://zm.huixiangedu.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://bz.bookmarksfly.cn

[Q26] 计数
来源：http://iu.hahajie.cn

SELECT COUNT(*) FROM users;
来源：http://uy.szsharing.cn

[Q27] 条件计数
来源：http://ld.haigaiapp.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://va.huixinmuqiang.cn

[Q28] 求和与平均
来源：http://qy.haigaiapp.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://vg.gzmigu.cn

[Q29] 最大最小值
来源：http://ss.521024.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://xt.asd995.cn

[Q30] 分组统计
来源：http://dl.huixinmuqiang.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mc.yuntaijiaju.cn

[Q31] 分组后过滤
来源：http://mq.yuexingan06.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://he.haigaiapp.cn

[Q32] 分组拼接字符串
来源：http://xd.newstarts.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://sl.hahajie.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://yh.hnjuh.cn

[Q33] 多列分组
来源：http://wi.bookmarksfly.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ho.shxzskj.cn

[Q34] 每组取第一条
来源：http://tw.shxzskj.cn

SELECT * FROM (
来源：http://tw.yuntaijiaju.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://au.wgjwhj.cn

) t WHERE rn = 1;
来源：http://hs.yuntaijiaju.cn

[Q35] 内连接
来源：http://rl.shxzukj.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://xm.wgjwhj.cn

[Q36] 左连接
来源：http://iy.colortex.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hq.yuexingan06.cn

[Q37] 右连接
来源：http://xc.bjjhwx.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hh.hnjuh.cn

[Q38] 全外连接（PostgreSQL）
来源：http://dd.szsharing.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ae.haigaiapp.cn

[Q39] 自连接（查上下级）
来源：http://qh.szxytkj.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://mo.huixiangedu.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://dy.gzmigu.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://ta.panjiajie.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ue.newstarts.cn

[Q41] 多表连接
来源：http://ax.wgjwhj.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://iz.nszjky.cn

JOIN users u ON u.id = o.user_id
来源：http://ni.colortex.cn

JOIN products p ON p.id = o.product_id;
来源：http://kk.panjiajie.cn

[Q42] 连接条件附加过滤
来源：http://zc.yuexingan06.cn

SELECT u.name, o.amount FROM users u
来源：http://mj.huixinmuqiang.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://om.wgjwhj.cn

[Q43] 标量子查询
来源：http://vj.shxzukj.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://va.yuntaijiaju.cn

[Q44] IN 子查询
来源：http://xk.panjiajie.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://nd.nicolike.cn

[Q45] EXISTS 判断存在
来源：http://ck.hnjuh.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://pe.chemitech.net.cn

[Q46] NOT EXISTS 判断不存在
来源：http://zz.huixinmuqiang.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ls.bookmarksfly.cn

[Q47] 与平均值比较
来源：http://rj.huixiangedu.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://gv.chemitech.net.cn

[Q48] CTE 公用表表达式
来源：http://rm.yuntaijiaju.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://fk.huixiangedu.cn

SELECT * FROM t WHERE c > 5;
来源：http://se.yuntaijiaju.cn

[Q49] 更新单行
来源：http://ly.shxzskj.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ah.szxytkj.cn

[Q50] 批量更新
来源：http://ws.nszjky.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://xe.szxytkj.cn

[Q51] 用子查询更新
来源：http://zv.nicolike.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://em.szxytkj.cn

[Q52] 删除指定行
来源：http://tf.muxihuayi.cn

DELETE FROM users WHERE id = 10;
来源：http://mc.wgjwhj.cn

[Q53] 按条件删除
来源：http://co.shxzukj.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ez.szsharing.cn

[Q54] 清空表
来源：http://oj.jianghongdianzi.cn

TRUNCATE TABLE logs;
来源：http://td.panjiajie.cn

[Q55] 排名（并列占位）
来源：http://oq.shxzskj.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ha.asd995.cn

[Q56] 密集排名（并列不占位）
来源：http://vv.colortex.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://tt.szxytkj.cn

[Q57] 行号
来源：http://xn.yuntaijiaju.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://sn.huanxung.cn

[Q58] 累计求和
来源：http://jf.muxihuayi.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://zn.521024.cn

[Q59] 分组内累计
来源：http://xt.nicolike.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://op.shxzukj.cn

[Q60] 取上一行 / 下一行
来源：http://vd.newstarts.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://vz.huixinmuqiang.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://qj.gzmigu.cn

[Q61] 移动平均
来源：http://sy.muxihuayi.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://zt.huixiangedu.cn

[Q62] 分组占比
来源：http://vv.lnxyls.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ku.nszjky.cn

[Q63] 开启事务
来源：http://lc.colortex.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://bk.shxzskj.cn

[Q64] 提交事务
来源：http://kg.jctech888.com.cn

COMMIT;
来源：http://yo.asd995.cn

[Q65] 回滚事务
来源：http://gb.colortex.cn

ROLLBACK;
来源：http://dt.hnjuh.cn

[Q66] 行锁查询
来源：http://ld.shtwfgs.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wi.hnjuh.cn

[Q67] 设置隔离级别
来源：http://zo.panjiajie.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://te.huanxung.cn

[Q68] 保存点
来源：http://qq.nszjky.cn

SAVEPOINT sp1;
来源：http://kw.nszjky.cn

ROLLBACK TO sp1;
来源：http://ym.hnjuh.cn

[Q69] 查看执行计划
来源：http://qb.szxytkj.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://yg.wgjwhj.cn

[Q70] 更新统计信息
来源：http://eq.szsharing.cn

ANALYZE TABLE users;
来源：http://lw.shxzskj.cn

[Q71] 查看建表语句
来源：http://qw.shxzskj.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wu.nicolike.cn

[Q72] 查看索引
来源：http://xw.szxytkj.cn

SHOW INDEX FROM users;
来源：http://ro.nicolike.cn

[Q73] 查看表状态
来源：http://oi.muxihuayi.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://uq.yuntaijiaju.cn

[Q74] 强制使用索引
来源：http://aj.shxzskj.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ry.yuntaijiaju.cn

[Q75] 日期格式化
来源：http://lw.wgjwhj.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://pk.yuexingan06.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://if.hnjuh.cn

[Q76] 按天统计
来源：http://eb.jianghongdianzi.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://eh.huanxung.cn

[Q77] 时间加减
来源：http://zc.yuexingan06.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mf.lnxyls.cn

[Q78] 当前时间
来源：http://nr.hahajie.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://kb.huanxung.cn

[Q79] 字符串拼接
来源：http://ar.szxytkj.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ou.szsharing.cn

[Q80] 字符串截取
来源：http://rr.gzmigu.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://af.shxzskj.cn

[Q81] 字符串替换
来源：http://nu.521024.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ru.nicolike.cn

[Q82] 字符长度与字节长度
来源：http://gl.newstarts.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://pf.9csxet.cn

[Q83] 大小写转换
来源：http://bd.colortex.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://up.jianghongdianzi.cn

[Q84] 去除首尾空格
来源：http://ji.huanxung.cn

SELECT TRIM(name) FROM users;
来源：http://qu.yuexingan06.cn

[Q85] 数值取整
来源：http://ss.9csxet.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://lq.hnjuh.cn

[Q86] 读取 JSON 字段
来源：http://xz.muxihuayi.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://li.huanxung.cn

[Q87] JSON 字段做条件
来源：http://je.shxzukj.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://zo.asd995.cn

[Q88] 行转列（条件聚合）
来源：http://aa.haigaiapp.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://nu.hnjuh.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mq.jctech888.com.cn

[Q89] 判断表是否存在
来源：http://fl.haigaiapp.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://xv.gzmigu.cn

[Q90] 生成序号列
来源：http://ju.colortex.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wc.szxytkj.cn

================================================================================
来源：http://br.shxzukj.cn

R. Bash 专题
来源：http://ub.huanxung.cn

================================================================================
来源：http://sc.szsharing.cn

[R01] shebang 与严格模式
来源：http://il.521024.cn

#!/usr/bin/env bash
来源：http://bv.colortex.cn

set -euo pipefail
来源：http://zw.huanxung.cn

[R02] 变量赋值与使用
来源：http://jl.newstarts.cn

name="Tom"; echo "$name"
来源：http://tm.bookmarksfly.cn

[R03] 只读变量
来源：http://dl.bjjhwx.cn

readonly PI=3.14
来源：http://rz.bjjhwx.cn

[R04] 位置参数
来源：http://nm.nszjky.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://xx.shxzukj.cn

[R05] 参数默认值
来源：http://gc.bookmarksfly.cn

name="${1:-default}"
来源：http://iu.lnxyls.cn

[R06] 判断命令是否存在
来源：http://ps.lnxyls.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://qy.panjiajie.cn

[R07] if 判断文件
来源：http://ot.newstarts.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ok.nicolike.cn

[R08] 数值比较
来源：http://fr.lnxyls.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://op.colortex.cn

[R09] 字符串比较
来源：http://ac.jianghongdianzi.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://xs.yuexingan06.cn

[R10] 正则匹配
来源：http://nh.shtwfgs.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://cw.asd995.cn

[R11] case 多分支
来源：http://kd.huixiangedu.cn

case "$1" in
来源：http://gk.shxzskj.cn

start) echo "启动" ;;
来源：http://ca.szsharing.cn

stop)  echo "停止" ;;
来源：http://gr.shtwfgs.cn

*)     echo "未知命令" ;;
来源：http://ag.panjiajie.cn

esac
来源：http://wi.yuexingan06.cn

[R12] for 遍历文件
来源：http://vj.colortex.cn

for f in *.txt; do echo "$f"; done
来源：http://df.colortex.cn

[R13] for 计数循环
来源：http://yj.bjjhwx.cn

for i in {1..10}; do echo "$i"; done
来源：http://sm.521024.cn

[R14] C 风格 for
来源：http://wk.huixinmuqiang.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://kh.yuntaijiaju.cn

[R15] while 逐行读文件
来源：http://lt.9csxet.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hw.yuexingan06.cn

[R16] until 等待条件
来源：http://je.nszjky.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://fg.lnxyls.cn

[R17] 数组定义与取值
来源：http://km.hnjuh.cn

arr=(a b c); echo "${arr[0]}"
来源：http://pm.jctech888.com.cn

[R18] 遍历数组
来源：http://je.huixinmuqiang.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://oc.shxzskj.cn

[R19] 数组长度
来源：http://bk.gzmigu.cn

echo "${#arr[@]}"
来源：http://sz.haigaiapp.cn

[R20] 关联数组（字典）
来源：http://sf.jianghongdianzi.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://qz.wgjwhj.cn

[R21] 字符串长度
来源：http://is.asd995.cn

echo "${#s}"
来源：http://zn.shxzskj.cn

[R22] 截取子串
来源：http://dl.nszjky.cn

echo "${s:0:5}"
来源：http://pk.bjjhwx.cn

[R23] 字符串替换
来源：http://tp.bookmarksfly.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mt.wgjwhj.cn

[R24] 大小写转换
来源：http://na.gzmigu.cn

echo "${s^^}"; echo "${s,,}"
来源：http://tf.huanxung.cn

[R25] 去后缀 / 去前缀
来源：http://hz.huixinmuqiang.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://od.szsharing.cn

[R26] 命令替换
来源：http://ve.chemitech.net.cn

now=$(date +%F); echo "$now"
来源：http://mu.haigaiapp.cn

[R27] 算术展开
来源：http://ak.szsharing.cn

echo $((1 + 2 * 3))
来源：http://hq.huixinmuqiang.cn

[R28] 浮点运算
来源：http://uw.szsharing.cn

echo "scale=2; 10/3" | bc
来源：http://sb.bookmarksfly.cn

[R29] 定义函数
来源：http://dx.shxzukj.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://nr.szsharing.cn

[R30] 函数返回状态码
来源：http://po.yuntaijiaju.cn

f() { return 0; }; f || echo "失败了"
来源：http://fj.huixinmuqiang.cn

[R31] 局部变量
来源：http://xz.lnxyls.cn

f() { local x=1; echo "$x"; }
来源：http://ph.huixinmuqiang.cn

[R32] 参数个数校验
来源：http://og.wgjwhj.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://vo.muxihuayi.cn

[R33] 捕获错误并提示行号
来源：http://bq.jctech888.com.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://my.yuntaijiaju.cn

[R34] 退出时清理
来源：http://fo.panjiajie.cn

trap 'rm -f "$tmp"' EXIT
来源：http://la.yuexingan06.cn

[R35] 后台执行并等待
来源：http://rl.shtwfgs.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://hf.521024.cn

[R36] 并发执行多个任务
来源：http://mj.521024.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ua.newstarts.cn

[R37] 把输出赋给变量
来源：http://ll.huixinmuqiang.cn

files=$(ls -1)
来源：http://ky.9csxet.cn

[R38] 管道串联
来源：http://xk.huanxung.cn

cat a.txt | grep -i error | wc -l
来源：http://zd.szxytkj.cn

[R39] 重定向标准输出与错误
来源：http://ug.wgjwhj.cn

cmd > out.log 2>&1
来源：http://nt.nszjky.cn

[R40] 追加写日志
来源：http://ds.asd995.cn

echo "log" >> out.log
来源：http://jw.panjiajie.cn

[R41] 丢弃输出
来源：http://zo.muxihuayi.cn

cmd >/dev/null 2>&1
来源：http://uq.nicolike.cn

[R42] 输入重定向
来源：http://kx.shxzskj.cn

wc -l < a.txt
来源：http://jb.lnxyls.cn

[R43] 按名字查找文件
来源：http://mf.yuntaijiaju.cn

find . -name "*.log" -type f
来源：http://lt.shxzskj.cn

[R44] 按修改时间查找
来源：http://qo.shxzskj.cn

find . -mtime -7 -type f
来源：http://wu.muxihuayi.cn

[R45] 批量删除
来源：http://id.huixiangedu.cn

find . -name "*.tmp" -delete
来源：http://nw.muxihuayi.cn

[R46] 递归替换文件内容
来源：http://zo.bookmarksfly.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ay.hnjuh.cn

[R47] sed 单行替换
来源：http://ri.asd995.cn

sed -i 's/foo/bar/g' a.txt
来源：http://oz.shtwfgs.cn

[R48] awk 取指定列
来源：http://wr.muxihuayi.cn

awk '{print $1, $3}' a.txt
来源：http://ai.muxihuayi.cn

[R49] awk 带条件
来源：http://bi.nicolike.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ol.panjiajie.cn

[R50] awk 求和
来源：http://hy.yuntaijiaju.cn

awk '{s += $2} END {print s}' a.txt
来源：http://jp.yuexingan06.cn

[R51] 排序去重取前几
来源：http://un.wgjwhj.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://tq.chemitech.net.cn

[R52] 统计行数
来源：http://ab.wgjwhj.cn

wc -l a.txt
来源：http://dj.muxihuayi.cn

[R53] 查看文件头与实时尾
来源：http://rm.wgjwhj.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://xu.521024.cn

[R54] 比较两个文件
来源：http://jb.shtwfgs.cn

diff a.txt b.txt
来源：http://cb.huanxung.cn

[R55] 压缩与解压
来源：http://wt.colortex.cn


<!-- 参考信息 -->