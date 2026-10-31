代发 wailian999

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://bn.shxzukj.cn

[Q05] 重命名列
来源：http://hx.newstarts.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://zk.panjiajie.cn

[Q06] 删除列
来源：http://zg.chemitech.net.cn

ALTER TABLE users DROP COLUMN age;
来源：http://bk.chemitech.net.cn

[Q07] 删除表
来源：http://we.nszjky.cn

DROP TABLE IF EXISTS orders;
来源：http://au.bookmarksfly.cn

[Q08] 创建普通索引
来源：http://gi.wgjwhj.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://gv.hahajie.cn

[Q09] 创建唯一索引
来源：http://uh.hahajie.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://yh.yuexingan06.cn

[Q10] 插入单行
来源：http://vl.newstarts.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ni.jctech888.com.cn

[Q11] 一次插入多行
来源：http://xx.panjiajie.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hn.bookmarksfly.cn

[Q12] 插入后取自增 ID
来源：http://lp.yuntaijiaju.cn

INSERT INTO users (name) VALUES ('C');
来源：http://pw.shtwfgs.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://zu.jianghongdianzi.cn

[Q13] 忽略重复插入
来源：http://er.muxihuayi.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ox.panjiajie.cn

[Q14] 存在则更新（upsert）
来源：http://ap.nicolike.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ia.newstarts.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://xd.jctech888.com.cn

[Q15] 查询全部
来源：http://gx.nszjky.cn

SELECT * FROM users;
来源：http://jp.huixiangedu.cn

[Q16] 查询指定列
来源：http://im.yuntaijiaju.cn

SELECT id, name FROM users;
来源：http://jt.yuexingan06.cn

[Q17] 条件查询
来源：http://th.nicolike.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://cu.bookmarksfly.cn

[Q18] 模糊匹配
来源：http://us.gzmigu.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://dr.bookmarksfly.cn

[Q19] 范围查询
来源：http://cp.bookmarksfly.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ae.szsharing.cn

[Q20] IN 列表
来源：http://er.9csxet.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://vh.shxzukj.cn

[Q21] 空值判断
来源：http://lk.521024.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://aq.muxihuayi.cn

[Q22] 排序
来源：http://vi.hnjuh.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wb.shtwfgs.cn

[Q23] 分页
来源：http://dq.bjjhwx.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://oz.colortex.cn

[Q24] 去重
来源：http://nf.hnjuh.cn

SELECT DISTINCT city FROM users;
来源：http://ru.asd995.cn

[Q25] 只取前 N 条
来源：http://oo.asd995.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://tl.shtwfgs.cn

[Q26] 计数
来源：http://sp.huixinmuqiang.cn

SELECT COUNT(*) FROM users;
来源：http://ef.jctech888.com.cn

[Q27] 条件计数
来源：http://wj.muxihuayi.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://sq.yuexingan06.cn

[Q28] 求和与平均
来源：http://yq.gzmigu.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://xf.colortex.cn

[Q29] 最大最小值
来源：http://wq.gzmigu.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://vk.jianghongdianzi.cn

[Q30] 分组统计
来源：http://xf.nszjky.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ud.shxzskj.cn

[Q31] 分组后过滤
来源：http://ha.chemitech.net.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ra.nszjky.cn

[Q32] 分组拼接字符串
来源：http://jw.bjjhwx.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wv.chemitech.net.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://yk.shtwfgs.cn

[Q33] 多列分组
来源：http://en.lnxyls.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://is.panjiajie.cn

[Q34] 每组取第一条
来源：http://yg.nszjky.cn

SELECT * FROM (
来源：http://jp.nszjky.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://kn.newstarts.cn

) t WHERE rn = 1;
来源：http://zh.hnjuh.cn

[Q35] 内连接
来源：http://bv.panjiajie.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://qz.newstarts.cn

[Q36] 左连接
来源：http://uo.huixiangedu.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://yc.shtwfgs.cn

[Q37] 右连接
来源：http://in.szxytkj.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://lk.shxzukj.cn

[Q38] 全外连接（PostgreSQL）
来源：http://xd.newstarts.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://tz.haigaiapp.cn

[Q39] 自连接（查上下级）
来源：http://px.9csxet.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://mt.huixiangedu.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://uz.huixiangedu.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://tz.muxihuayi.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://as.asd995.cn

[Q41] 多表连接
来源：http://si.shxzskj.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://wm.newstarts.cn

JOIN users u ON u.id = o.user_id
来源：http://zl.haigaiapp.cn

JOIN products p ON p.id = o.product_id;
来源：http://fz.huanxung.cn

[Q42] 连接条件附加过滤
来源：http://bg.9csxet.cn

SELECT u.name, o.amount FROM users u
来源：http://xp.panjiajie.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://dq.asd995.cn

[Q43] 标量子查询
来源：http://iw.haigaiapp.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://fc.asd995.cn

[Q44] IN 子查询
来源：http://id.jianghongdianzi.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://me.shxzukj.cn

[Q45] EXISTS 判断存在
来源：http://ao.jctech888.com.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wo.szxytkj.cn

[Q46] NOT EXISTS 判断不存在
来源：http://ox.hnjuh.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://fc.jctech888.com.cn

[Q47] 与平均值比较
来源：http://yd.shtwfgs.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ke.shxzukj.cn

[Q48] CTE 公用表表达式
来源：http://tz.gzmigu.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://co.shtwfgs.cn

SELECT * FROM t WHERE c > 5;
来源：http://yx.yuexingan06.cn

[Q49] 更新单行
来源：http://mx.wgjwhj.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://bk.chemitech.net.cn

[Q50] 批量更新
来源：http://ap.huixinmuqiang.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://je.szsharing.cn

[Q51] 用子查询更新
来源：http://mg.lnxyls.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://xm.szsharing.cn

[Q52] 删除指定行
来源：http://ir.nicolike.cn

DELETE FROM users WHERE id = 10;
来源：http://pf.chemitech.net.cn

[Q53] 按条件删除
来源：http://ga.gzmigu.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://sl.hahajie.cn

[Q54] 清空表
来源：http://lb.nicolike.cn

TRUNCATE TABLE logs;
来源：http://zi.gzmigu.cn

[Q55] 排名（并列占位）
来源：http://kz.shxzskj.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://vv.panjiajie.cn

[Q56] 密集排名（并列不占位）
来源：http://vz.wgjwhj.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://re.jianghongdianzi.cn

[Q57] 行号
来源：http://vq.huixinmuqiang.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://bh.9csxet.cn

[Q58] 累计求和
来源：http://jf.huixinmuqiang.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://km.yuexingan06.cn

[Q59] 分组内累计
来源：http://yh.lnxyls.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://fy.chemitech.net.cn

[Q60] 取上一行 / 下一行
来源：http://hq.panjiajie.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://lj.yuntaijiaju.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://xf.yuexingan06.cn

[Q61] 移动平均
来源：http://ga.huixiangedu.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://zq.szsharing.cn

[Q62] 分组占比
来源：http://lq.panjiajie.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://zl.nszjky.cn

[Q63] 开启事务
来源：http://bt.huixiangedu.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://zt.shxzskj.cn

[Q64] 提交事务
来源：http://ho.lnxyls.cn

COMMIT;
来源：http://nc.bookmarksfly.cn

[Q65] 回滚事务
来源：http://bq.wgjwhj.cn

ROLLBACK;
来源：http://vj.hahajie.cn

[Q66] 行锁查询
来源：http://wr.shxzukj.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://xp.muxihuayi.cn

[Q67] 设置隔离级别
来源：http://ie.nszjky.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://yo.szxytkj.cn

[Q68] 保存点
来源：http://oc.huixiangedu.cn

SAVEPOINT sp1;
来源：http://be.newstarts.cn

ROLLBACK TO sp1;
来源：http://cx.huixinmuqiang.cn

[Q69] 查看执行计划
来源：http://ds.huanxung.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://eq.huixiangedu.cn

[Q70] 更新统计信息
来源：http://pr.bjjhwx.cn

ANALYZE TABLE users;
来源：http://ka.wgjwhj.cn

[Q71] 查看建表语句
来源：http://pk.521024.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://fi.gzmigu.cn

[Q72] 查看索引
来源：http://ho.hnjuh.cn

SHOW INDEX FROM users;
来源：http://bh.bjjhwx.cn

[Q73] 查看表状态
来源：http://as.colortex.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://ax.muxihuayi.cn

[Q74] 强制使用索引
来源：http://mr.huanxung.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://nw.huanxung.cn

[Q75] 日期格式化
来源：http://ia.colortex.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://bp.huixiangedu.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://an.colortex.cn

[Q76] 按天统计
来源：http://gy.chemitech.net.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://pr.hnjuh.cn

[Q77] 时间加减
来源：http://jo.shtwfgs.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://od.bookmarksfly.cn

[Q78] 当前时间
来源：http://um.shxzukj.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hv.shtwfgs.cn

[Q79] 字符串拼接
来源：http://ut.colortex.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://kt.chemitech.net.cn

[Q80] 字符串截取
来源：http://bb.hnjuh.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ef.newstarts.cn

[Q81] 字符串替换
来源：http://ja.gzmigu.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://rv.nszjky.cn

[Q82] 字符长度与字节长度
来源：http://mj.szxytkj.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://le.wgjwhj.cn

[Q83] 大小写转换
来源：http://jg.yuexingan06.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wi.huanxung.cn

[Q84] 去除首尾空格
来源：http://qp.wgjwhj.cn

SELECT TRIM(name) FROM users;
来源：http://hz.szxytkj.cn

[Q85] 数值取整
来源：http://re.yuexingan06.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ja.szsharing.cn

[Q86] 读取 JSON 字段
来源：http://pd.lnxyls.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ea.jctech888.com.cn

[Q87] JSON 字段做条件
来源：http://rs.jianghongdianzi.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://jz.colortex.cn

[Q88] 行转列（条件聚合）
来源：http://zk.lnxyls.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://eb.bookmarksfly.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://it.muxihuayi.cn

[Q89] 判断表是否存在
来源：http://dm.yuexingan06.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://jj.szxytkj.cn

[Q90] 生成序号列
来源：http://yp.haigaiapp.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ve.chemitech.net.cn

================================================================================
来源：http://sm.shtwfgs.cn

R. Bash 专题
来源：http://ml.9csxet.cn

================================================================================
来源：http://jp.hnjuh.cn

[R01] shebang 与严格模式
来源：http://rb.colortex.cn

#!/usr/bin/env bash
来源：http://pu.jctech888.com.cn

set -euo pipefail
来源：http://op.hnjuh.cn

[R02] 变量赋值与使用
来源：http://od.huanxung.cn

name="Tom"; echo "$name"
来源：http://wq.yuntaijiaju.cn

[R03] 只读变量
来源：http://ow.huanxung.cn

readonly PI=3.14
来源：http://di.nszjky.cn

[R04] 位置参数
来源：http://dl.chemitech.net.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://lz.huixiangedu.cn

[R05] 参数默认值
来源：http://dw.muxihuayi.cn

name="${1:-default}"
来源：http://yd.huixinmuqiang.cn

[R06] 判断命令是否存在
来源：http://xk.szsharing.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://kv.hnjuh.cn

[R07] if 判断文件
来源：http://bk.huanxung.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wv.panjiajie.cn

[R08] 数值比较
来源：http://wt.colortex.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://ya.nszjky.cn

[R09] 字符串比较
来源：http://vm.haigaiapp.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hm.jianghongdianzi.cn

[R10] 正则匹配
来源：http://um.lnxyls.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://xm.panjiajie.cn

[R11] case 多分支
来源：http://br.yuexingan06.cn

case "$1" in
来源：http://eo.yuexingan06.cn

start) echo "启动" ;;
来源：http://ej.huixiangedu.cn

stop)  echo "停止" ;;
来源：http://yj.shxzskj.cn

*)     echo "未知命令" ;;
来源：http://gn.hahajie.cn

esac
来源：http://eg.yuexingan06.cn

[R12] for 遍历文件
来源：http://kh.hahajie.cn

for f in *.txt; do echo "$f"; done
来源：http://pn.szxytkj.cn

[R13] for 计数循环
来源：http://qp.hnjuh.cn

for i in {1..10}; do echo "$i"; done
来源：http://ps.hnjuh.cn

[R14] C 风格 for
来源：http://ag.nicolike.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://fx.hahajie.cn

[R15] while 逐行读文件
来源：http://jb.asd995.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://dd.521024.cn

[R16] until 等待条件
来源：http://dx.bookmarksfly.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://tg.jianghongdianzi.cn

[R17] 数组定义与取值
来源：http://fm.nicolike.cn

arr=(a b c); echo "${arr[0]}"
来源：http://oi.bjjhwx.cn

[R18] 遍历数组
来源：http://mf.yuntaijiaju.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://cs.szsharing.cn

[R19] 数组长度
来源：http://bb.asd995.cn

echo "${#arr[@]}"
来源：http://ur.shxzskj.cn

[R20] 关联数组（字典）
来源：http://sd.asd995.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://sv.hnjuh.cn

[R21] 字符串长度
来源：http://rk.lnxyls.cn

echo "${#s}"
来源：http://hj.colortex.cn

[R22] 截取子串
来源：http://uy.shxzskj.cn

echo "${s:0:5}"
来源：http://ud.shtwfgs.cn

[R23] 字符串替换
来源：http://ex.muxihuayi.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://qu.chemitech.net.cn

[R24] 大小写转换
来源：http://lu.asd995.cn

echo "${s^^}"; echo "${s,,}"
来源：http://um.yuexingan06.cn

[R25] 去后缀 / 去前缀
来源：http://dc.bjjhwx.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://tq.huixiangedu.cn

[R26] 命令替换
来源：http://kq.hahajie.cn

now=$(date +%F); echo "$now"
来源：http://hc.jianghongdianzi.cn

[R27] 算术展开
来源：http://zd.szsharing.cn

echo $((1 + 2 * 3))
来源：http://bm.panjiajie.cn

[R28] 浮点运算
来源：http://fz.newstarts.cn

echo "scale=2; 10/3" | bc
来源：http://kq.bookmarksfly.cn

[R29] 定义函数
来源：http://dt.muxihuayi.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://fo.huanxung.cn

[R30] 函数返回状态码
来源：http://hf.huixinmuqiang.cn

f() { return 0; }; f || echo "失败了"
来源：http://wz.hnjuh.cn

[R31] 局部变量
来源：http://rp.hnjuh.cn

f() { local x=1; echo "$x"; }
来源：http://cd.wgjwhj.cn

[R32] 参数个数校验
来源：http://bb.shxzukj.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://lf.521024.cn

[R33] 捕获错误并提示行号
来源：http://qc.jctech888.com.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://bj.bjjhwx.cn

[R34] 退出时清理
来源：http://jq.haigaiapp.cn

trap 'rm -f "$tmp"' EXIT
来源：http://ge.9csxet.cn

[R35] 后台执行并等待
来源：http://fd.newstarts.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://pr.muxihuayi.cn

[R36] 并发执行多个任务
来源：http://ln.bookmarksfly.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mn.asd995.cn

[R37] 把输出赋给变量
来源：http://pn.521024.cn

files=$(ls -1)
来源：http://ow.yuntaijiaju.cn

[R38] 管道串联
来源：http://nj.jctech888.com.cn

cat a.txt | grep -i error | wc -l
来源：http://op.9csxet.cn

[R39] 重定向标准输出与错误
来源：http://pu.huixinmuqiang.cn

cmd > out.log 2>&1
来源：http://vp.yuexingan06.cn

[R40] 追加写日志
来源：http://ur.huixiangedu.cn

echo "log" >> out.log
来源：http://qw.wgjwhj.cn

[R41] 丢弃输出
来源：http://ub.shxzukj.cn

cmd >/dev/null 2>&1
来源：http://oj.hnjuh.cn

[R42] 输入重定向
来源：http://th.shxzskj.cn

wc -l < a.txt
来源：http://ig.newstarts.cn

[R43] 按名字查找文件
来源：http://nf.yuexingan06.cn

find . -name "*.log" -type f
来源：http://cc.shxzskj.cn

[R44] 按修改时间查找
来源：http://fn.wgjwhj.cn

find . -mtime -7 -type f
来源：http://kv.jianghongdianzi.cn

[R45] 批量删除
来源：http://mz.asd995.cn

find . -name "*.tmp" -delete
来源：http://tz.newstarts.cn

[R46] 递归替换文件内容
来源：http://nu.shxzukj.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://jy.wgjwhj.cn

[R47] sed 单行替换
来源：http://qx.9csxet.cn

sed -i 's/foo/bar/g' a.txt
来源：http://ac.newstarts.cn

[R48] awk 取指定列
来源：http://ar.jctech888.com.cn

awk '{print $1, $3}' a.txt
来源：http://kb.colortex.cn

[R49] awk 带条件
来源：http://kn.muxihuayi.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ht.newstarts.cn

[R50] awk 求和
来源：http://ky.yuexingan06.cn

awk '{s += $2} END {print s}' a.txt
来源：http://bo.muxihuayi.cn

[R51] 排序去重取前几
来源：http://pa.muxihuayi.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://ry.yuexingan06.cn

[R52] 统计行数
来源：http://wk.muxihuayi.cn

wc -l a.txt
来源：http://bb.szxytkj.cn

[R53] 查看文件头与实时尾
来源：http://er.nicolike.cn


<!-- 参考信息 -->