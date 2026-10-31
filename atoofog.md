代发 wailian999

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ru.huixiangedu.cn

[Q11] 一次插入多行
来源：http://kt.521024.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://jb.hahajie.cn

[Q12] 插入后取自增 ID
来源：http://ij.shxzskj.cn

INSERT INTO users (name) VALUES ('C');
来源：http://nt.szsharing.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hc.chemitech.net.cn

[Q13] 忽略重复插入
来源：http://ae.hnjuh.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ur.asd995.cn

[Q14] 存在则更新（upsert）
来源：http://oa.bookmarksfly.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://tq.haigaiapp.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://qq.lnxyls.cn

[Q15] 查询全部
来源：http://em.nicolike.cn

SELECT * FROM users;
来源：http://ko.shtwfgs.cn

[Q16] 查询指定列
来源：http://qm.huanxung.cn

SELECT id, name FROM users;
来源：http://ww.jianghongdianzi.cn

[Q17] 条件查询
来源：http://qu.gzmigu.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://xf.newstarts.cn

[Q18] 模糊匹配
来源：http://vs.jctech888.com.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hk.jianghongdianzi.cn

[Q19] 范围查询
来源：http://ig.jctech888.com.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wv.yuexingan06.cn

[Q20] IN 列表
来源：http://tb.yuexingan06.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ge.hahajie.cn

[Q21] 空值判断
来源：http://lf.huanxung.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://mm.wgjwhj.cn

[Q22] 排序
来源：http://xy.bookmarksfly.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mh.521024.cn

[Q23] 分页
来源：http://pi.hnjuh.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://qp.bjjhwx.cn

[Q24] 去重
来源：http://jr.jctech888.com.cn

SELECT DISTINCT city FROM users;
来源：http://eb.szxytkj.cn

[Q25] 只取前 N 条
来源：http://hn.szxytkj.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ij.lnxyls.cn

[Q26] 计数
来源：http://zm.bookmarksfly.cn

SELECT COUNT(*) FROM users;
来源：http://ky.hahajie.cn

[Q27] 条件计数
来源：http://cp.colortex.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://sv.panjiajie.cn

[Q28] 求和与平均
来源：http://bx.panjiajie.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://st.chemitech.net.cn

[Q29] 最大最小值
来源：http://cf.bjjhwx.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://ii.szsharing.cn

[Q30] 分组统计
来源：http://qv.asd995.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://uz.521024.cn

[Q31] 分组后过滤
来源：http://yz.9csxet.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mo.haigaiapp.cn

[Q32] 分组拼接字符串
来源：http://bq.szsharing.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ld.shxzukj.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ki.colortex.cn

[Q33] 多列分组
来源：http://ax.nszjky.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ud.9csxet.cn

[Q34] 每组取第一条
来源：http://tm.colortex.cn

SELECT * FROM (
来源：http://ck.huixiangedu.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://cn.panjiajie.cn

) t WHERE rn = 1;
来源：http://km.huixiangedu.cn

[Q35] 内连接
来源：http://dt.shtwfgs.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://aa.newstarts.cn

[Q36] 左连接
来源：http://xw.bookmarksfly.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://fx.huixiangedu.cn

[Q37] 右连接
来源：http://gp.huixinmuqiang.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ls.newstarts.cn

[Q38] 全外连接（PostgreSQL）
来源：http://jj.panjiajie.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://gf.lnxyls.cn

[Q39] 自连接（查上下级）
来源：http://lk.colortex.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://el.bookmarksfly.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://kr.huixinmuqiang.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://lo.hnjuh.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ua.haigaiapp.cn

[Q41] 多表连接
来源：http://ml.panjiajie.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://tj.nicolike.cn

JOIN users u ON u.id = o.user_id
来源：http://qf.huixiangedu.cn

JOIN products p ON p.id = o.product_id;
来源：http://hb.chemitech.net.cn

[Q42] 连接条件附加过滤
来源：http://on.521024.cn

SELECT u.name, o.amount FROM users u
来源：http://hg.shxzskj.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ij.chemitech.net.cn

[Q43] 标量子查询
来源：http://fl.colortex.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://qt.huixiangedu.cn

[Q44] IN 子查询
来源：http://lf.huanxung.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mu.jctech888.com.cn

[Q45] EXISTS 判断存在
来源：http://ry.muxihuayi.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ra.colortex.cn

[Q46] NOT EXISTS 判断不存在
来源：http://tu.huixiangedu.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ir.yuexingan06.cn

[Q47] 与平均值比较
来源：http://ai.yuntaijiaju.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hj.jctech888.com.cn

[Q48] CTE 公用表表达式
来源：http://gi.haigaiapp.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://dj.jctech888.com.cn

SELECT * FROM t WHERE c > 5;
来源：http://ki.nszjky.cn

[Q49] 更新单行
来源：http://ir.bookmarksfly.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://df.chemitech.net.cn

[Q50] 批量更新
来源：http://rt.gzmigu.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://xp.panjiajie.cn

[Q51] 用子查询更新
来源：http://ve.muxihuayi.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://rg.yuexingan06.cn

[Q52] 删除指定行
来源：http://za.colortex.cn

DELETE FROM users WHERE id = 10;
来源：http://iz.bookmarksfly.cn

[Q53] 按条件删除
来源：http://hm.huanxung.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://bz.nicolike.cn

[Q54] 清空表
来源：http://de.521024.cn

TRUNCATE TABLE logs;
来源：http://pw.9csxet.cn

[Q55] 排名（并列占位）
来源：http://tb.gzmigu.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://im.huixinmuqiang.cn

[Q56] 密集排名（并列不占位）
来源：http://rb.newstarts.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://cr.521024.cn

[Q57] 行号
来源：http://fi.chemitech.net.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ei.gzmigu.cn

[Q58] 累计求和
来源：http://vs.asd995.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://xk.colortex.cn

[Q59] 分组内累计
来源：http://eu.lnxyls.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://cy.9csxet.cn

[Q60] 取上一行 / 下一行
来源：http://xk.yuexingan06.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://lp.wgjwhj.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://cf.gzmigu.cn

[Q61] 移动平均
来源：http://ez.asd995.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://qo.shxzskj.cn

[Q62] 分组占比
来源：http://vi.haigaiapp.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://yg.nszjky.cn

[Q63] 开启事务
来源：http://eg.shtwfgs.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://dh.521024.cn

[Q64] 提交事务
来源：http://xm.haigaiapp.cn

COMMIT;
来源：http://il.haigaiapp.cn

[Q65] 回滚事务
来源：http://yf.bjjhwx.cn

ROLLBACK;
来源：http://hb.szxytkj.cn

[Q66] 行锁查询
来源：http://ms.nicolike.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ay.huixinmuqiang.cn

[Q67] 设置隔离级别
来源：http://cm.shxzskj.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://oj.gzmigu.cn

[Q68] 保存点
来源：http://yl.shtwfgs.cn

SAVEPOINT sp1;
来源：http://ox.jctech888.com.cn

ROLLBACK TO sp1;
来源：http://qy.muxihuayi.cn

[Q69] 查看执行计划
来源：http://jb.panjiajie.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://zr.colortex.cn

[Q70] 更新统计信息
来源：http://gx.szxytkj.cn

ANALYZE TABLE users;
来源：http://dz.shxzskj.cn

[Q71] 查看建表语句
来源：http://tk.newstarts.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://fv.shxzukj.cn

[Q72] 查看索引
来源：http://yu.huanxung.cn

SHOW INDEX FROM users;
来源：http://dd.bookmarksfly.cn

[Q73] 查看表状态
来源：http://lj.huixiangedu.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://pl.shxzskj.cn

[Q74] 强制使用索引
来源：http://fw.nszjky.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://jf.hnjuh.cn

[Q75] 日期格式化
来源：http://fn.9csxet.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wk.nicolike.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ol.szsharing.cn

[Q76] 按天统计
来源：http://yj.bjjhwx.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://dz.colortex.cn

[Q77] 时间加减
来源：http://ln.jianghongdianzi.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://kr.hahajie.cn

[Q78] 当前时间
来源：http://ij.huixiangedu.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wu.colortex.cn

[Q79] 字符串拼接
来源：http://bo.jctech888.com.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mj.shxzskj.cn

[Q80] 字符串截取
来源：http://dl.chemitech.net.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://oh.yuexingan06.cn

[Q81] 字符串替换
来源：http://ji.bookmarksfly.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://et.bookmarksfly.cn

[Q82] 字符长度与字节长度
来源：http://ka.521024.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://gw.521024.cn

[Q83] 大小写转换
来源：http://ch.szxytkj.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://rd.newstarts.cn

[Q84] 去除首尾空格
来源：http://md.asd995.cn

SELECT TRIM(name) FROM users;
来源：http://qq.szsharing.cn

[Q85] 数值取整
来源：http://nj.asd995.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ew.huanxung.cn

[Q86] 读取 JSON 字段
来源：http://di.yuntaijiaju.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://lx.bjjhwx.cn

[Q87] JSON 字段做条件
来源：http://no.jctech888.com.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ye.chemitech.net.cn

[Q88] 行转列（条件聚合）
来源：http://zu.hahajie.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://zi.bookmarksfly.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://yl.szxytkj.cn

[Q89] 判断表是否存在
来源：http://pa.huixiangedu.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://dj.muxihuayi.cn

[Q90] 生成序号列
来源：http://uo.lnxyls.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://dc.panjiajie.cn

================================================================================
来源：http://hg.bjjhwx.cn

R. Bash 专题
来源：http://rf.hahajie.cn

================================================================================
来源：http://dm.muxihuayi.cn

[R01] shebang 与严格模式
来源：http://lt.wgjwhj.cn

#!/usr/bin/env bash
来源：http://gj.szsharing.cn

set -euo pipefail
来源：http://es.szsharing.cn

[R02] 变量赋值与使用
来源：http://ue.521024.cn

name="Tom"; echo "$name"
来源：http://ev.muxihuayi.cn

[R03] 只读变量
来源：http://fi.yuexingan06.cn

readonly PI=3.14
来源：http://kz.haigaiapp.cn

[R04] 位置参数
来源：http://nq.nicolike.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://cp.szsharing.cn

[R05] 参数默认值
来源：http://gx.huanxung.cn

name="${1:-default}"
来源：http://or.hahajie.cn

[R06] 判断命令是否存在
来源：http://xq.yuexingan06.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://tp.chemitech.net.cn

[R07] if 判断文件
来源：http://lg.gzmigu.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://sq.shxzskj.cn

[R08] 数值比较
来源：http://pn.shxzukj.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://cz.nszjky.cn

[R09] 字符串比较
来源：http://lm.szxytkj.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://lt.lnxyls.cn

[R10] 正则匹配
来源：http://xa.hnjuh.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://vk.asd995.cn

[R11] case 多分支
来源：http://dv.521024.cn

case "$1" in
来源：http://cn.szsharing.cn

start) echo "启动" ;;
来源：http://hx.yuexingan06.cn

stop)  echo "停止" ;;
来源：http://dd.bjjhwx.cn

*)     echo "未知命令" ;;
来源：http://qk.lnxyls.cn

esac
来源：http://ia.huanxung.cn

[R12] for 遍历文件
来源：http://qf.bookmarksfly.cn

for f in *.txt; do echo "$f"; done
来源：http://yb.asd995.cn

[R13] for 计数循环
来源：http://pf.nszjky.cn

for i in {1..10}; do echo "$i"; done
来源：http://bh.bjjhwx.cn

[R14] C 风格 for
来源：http://ox.bjjhwx.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://nh.hahajie.cn

[R15] while 逐行读文件
来源：http://zy.lnxyls.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://zx.shxzukj.cn

[R16] until 等待条件
来源：http://vi.9csxet.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://tf.bjjhwx.cn

[R17] 数组定义与取值
来源：http://nj.bookmarksfly.cn

arr=(a b c); echo "${arr[0]}"
来源：http://sc.panjiajie.cn

[R18] 遍历数组
来源：http://gi.chemitech.net.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://zb.huixiangedu.cn

[R19] 数组长度
来源：http://uh.521024.cn

echo "${#arr[@]}"
来源：http://un.shxzukj.cn

[R20] 关联数组（字典）
来源：http://gp.huixinmuqiang.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://xs.huanxung.cn

[R21] 字符串长度
来源：http://vl.chemitech.net.cn

echo "${#s}"
来源：http://eh.colortex.cn

[R22] 截取子串
来源：http://bg.chemitech.net.cn

echo "${s:0:5}"
来源：http://oz.yuntaijiaju.cn

[R23] 字符串替换
来源：http://ch.hnjuh.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://jr.muxihuayi.cn

[R24] 大小写转换
来源：http://ck.huixinmuqiang.cn

echo "${s^^}"; echo "${s,,}"
来源：http://mm.newstarts.cn

[R25] 去后缀 / 去前缀
来源：http://xx.bjjhwx.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://mj.yuexingan06.cn

[R26] 命令替换
来源：http://lj.jianghongdianzi.cn

now=$(date +%F); echo "$now"
来源：http://am.shtwfgs.cn

[R27] 算术展开
来源：http://zl.panjiajie.cn

echo $((1 + 2 * 3))
来源：http://mt.521024.cn

[R28] 浮点运算
来源：http://db.shxzskj.cn

echo "scale=2; 10/3" | bc
来源：http://ds.lnxyls.cn

[R29] 定义函数
来源：http://we.newstarts.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ap.huixinmuqiang.cn

[R30] 函数返回状态码
来源：http://jx.521024.cn

f() { return 0; }; f || echo "失败了"
来源：http://ds.lnxyls.cn

[R31] 局部变量
来源：http://pn.huixinmuqiang.cn

f() { local x=1; echo "$x"; }
来源：http://wk.asd995.cn

[R32] 参数个数校验
来源：http://pv.521024.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ov.shtwfgs.cn

[R33] 捕获错误并提示行号
来源：http://ax.newstarts.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://td.yuexingan06.cn

[R34] 退出时清理
来源：http://vn.521024.cn

trap 'rm -f "$tmp"' EXIT
来源：http://gp.jctech888.com.cn

[R35] 后台执行并等待
来源：http://zc.muxihuayi.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://iv.bookmarksfly.cn

[R36] 并发执行多个任务
来源：http://bq.shtwfgs.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://md.521024.cn

[R37] 把输出赋给变量
来源：http://px.521024.cn

files=$(ls -1)
来源：http://zm.szxytkj.cn

[R38] 管道串联
来源：http://hh.muxihuayi.cn

cat a.txt | grep -i error | wc -l
来源：http://wo.nicolike.cn

[R39] 重定向标准输出与错误
来源：http://nj.shxzukj.cn

cmd > out.log 2>&1
来源：http://db.bjjhwx.cn

[R40] 追加写日志
来源：http://zo.chemitech.net.cn

echo "log" >> out.log
来源：http://qc.shtwfgs.cn

[R41] 丢弃输出
来源：http://xf.haigaiapp.cn

cmd >/dev/null 2>&1
来源：http://ti.wgjwhj.cn

[R42] 输入重定向
来源：http://wj.bjjhwx.cn

wc -l < a.txt
来源：http://xh.shtwfgs.cn

[R43] 按名字查找文件
来源：http://if.huanxung.cn

find . -name "*.log" -type f
来源：http://et.wgjwhj.cn

[R44] 按修改时间查找
来源：http://xg.yuntaijiaju.cn

find . -mtime -7 -type f
来源：http://la.asd995.cn

[R45] 批量删除
来源：http://ea.newstarts.cn

find . -name "*.tmp" -delete
来源：http://jp.newstarts.cn

[R46] 递归替换文件内容
来源：http://nx.wgjwhj.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ge.wgjwhj.cn

[R47] sed 单行替换
来源：http://ki.asd995.cn

sed -i 's/foo/bar/g' a.txt
来源：http://pe.szsharing.cn

[R48] awk 取指定列
来源：http://tq.haigaiapp.cn

awk '{print $1, $3}' a.txt
来源：http://yy.yuexingan06.cn

[R49] awk 带条件
来源：http://ob.nszjky.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://vh.panjiajie.cn

[R50] awk 求和
来源：http://af.hahajie.cn

awk '{s += $2} END {print s}' a.txt
来源：http://mi.shtwfgs.cn

[R51] 排序去重取前几
来源：http://uv.yuexingan06.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://ll.521024.cn

[R52] 统计行数
来源：http://bm.yuexingan06.cn

wc -l a.txt
来源：http://op.huixinmuqiang.cn

[R53] 查看文件头与实时尾
来源：http://lb.newstarts.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://jl.szsharing.cn

[R54] 比较两个文件
来源：http://zw.nszjky.cn

diff a.txt b.txt
来源：http://by.muxihuayi.cn

[R55] 压缩与解压
来源：http://ny.lnxyls.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://cy.gzmigu.cn

[R56] 远程拷贝
来源：http://qx.wgjwhj.cn

scp file user@host:/path/
来源：http://dl.colortex.cn

[R57] 远程执行命令
来源：http://tq.huixinmuqiang.cn

ssh user@host 'uptime'
来源：http://lw.huixinmuqiang.cn

[R58] 下载文件
来源：http://zc.huixiangedu.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://sa.lnxyls.cn

[R59] 发 POST JSON
来源：http://lo.nszjky.cn


<!-- 参考信息 -->