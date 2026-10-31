代发 wailian999

);
来源：http://rs.szsharing.cn

[Q03] 增加列
来源：http://aw.shxzskj.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://uw.shxzskj.cn

[Q04] 修改列类型
来源：http://eb.huanxung.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://br.huanxung.cn

[Q05] 重命名列
来源：http://hc.bjjhwx.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://of.lnxyls.cn

[Q06] 删除列
来源：http://gv.9csxet.cn

ALTER TABLE users DROP COLUMN age;
来源：http://na.bookmarksfly.cn

[Q07] 删除表
来源：http://is.szxytkj.cn

DROP TABLE IF EXISTS orders;
来源：http://nh.haigaiapp.cn

[Q08] 创建普通索引
来源：http://mk.jctech888.com.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://hb.hahajie.cn

[Q09] 创建唯一索引
来源：http://rs.shxzukj.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://kv.huixinmuqiang.cn

[Q10] 插入单行
来源：http://ge.bookmarksfly.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://fk.panjiajie.cn

[Q11] 一次插入多行
来源：http://zo.jctech888.com.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://zj.shxzukj.cn

[Q12] 插入后取自增 ID
来源：http://rm.521024.cn

INSERT INTO users (name) VALUES ('C');
来源：http://wq.muxihuayi.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://lj.asd995.cn

[Q13] 忽略重复插入
来源：http://re.9csxet.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ci.muxihuayi.cn

[Q14] 存在则更新（upsert）
来源：http://zu.haigaiapp.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://le.muxihuayi.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mh.lnxyls.cn

[Q15] 查询全部
来源：http://ss.muxihuayi.cn

SELECT * FROM users;
来源：http://cj.chemitech.net.cn

[Q16] 查询指定列
来源：http://nw.gzmigu.cn

SELECT id, name FROM users;
来源：http://ti.hahajie.cn

[Q17] 条件查询
来源：http://gw.colortex.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://xx.szsharing.cn

[Q18] 模糊匹配
来源：http://dt.jianghongdianzi.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://jo.yuexingan06.cn

[Q19] 范围查询
来源：http://mf.yuntaijiaju.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://za.nszjky.cn

[Q20] IN 列表
来源：http://rl.yuexingan06.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://fs.521024.cn

[Q21] 空值判断
来源：http://we.panjiajie.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://om.wgjwhj.cn

[Q22] 排序
来源：http://xd.jctech888.com.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://uh.huanxung.cn

[Q23] 分页
来源：http://dc.shtwfgs.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mz.jctech888.com.cn

[Q24] 去重
来源：http://fa.newstarts.cn

SELECT DISTINCT city FROM users;
来源：http://zg.wgjwhj.cn

[Q25] 只取前 N 条
来源：http://ow.shxzukj.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://rc.haigaiapp.cn

[Q26] 计数
来源：http://mi.wgjwhj.cn

SELECT COUNT(*) FROM users;
来源：http://gd.yuntaijiaju.cn

[Q27] 条件计数
来源：http://by.wgjwhj.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ve.hnjuh.cn

[Q28] 求和与平均
来源：http://zl.jctech888.com.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://rf.shtwfgs.cn

[Q29] 最大最小值
来源：http://ex.521024.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://ql.nszjky.cn

[Q30] 分组统计
来源：http://vm.521024.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://uc.wgjwhj.cn

[Q31] 分组后过滤
来源：http://ui.asd995.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://sm.wgjwhj.cn

[Q32] 分组拼接字符串
来源：http://or.yuntaijiaju.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://pr.huanxung.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://fp.huixinmuqiang.cn

[Q33] 多列分组
来源：http://ot.chemitech.net.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://my.huixinmuqiang.cn

[Q34] 每组取第一条
来源：http://yo.shxzskj.cn

SELECT * FROM (
来源：http://xo.shtwfgs.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://zo.gzmigu.cn

) t WHERE rn = 1;
来源：http://xx.wgjwhj.cn

[Q35] 内连接
来源：http://sr.hnjuh.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://se.jianghongdianzi.cn

[Q36] 左连接
来源：http://hv.hnjuh.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://iu.jianghongdianzi.cn

[Q37] 右连接
来源：http://vv.szsharing.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://rq.wgjwhj.cn

[Q38] 全外连接（PostgreSQL）
来源：http://ti.szxytkj.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://nm.lnxyls.cn

[Q39] 自连接（查上下级）
来源：http://oz.wgjwhj.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://ts.asd995.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ty.hahajie.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://wy.hahajie.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hf.jctech888.com.cn

[Q41] 多表连接
来源：http://ci.yuexingan06.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://vf.shxzukj.cn

JOIN users u ON u.id = o.user_id
来源：http://kl.szxytkj.cn

JOIN products p ON p.id = o.product_id;
来源：http://tq.nicolike.cn

[Q42] 连接条件附加过滤
来源：http://wx.bjjhwx.cn

SELECT u.name, o.amount FROM users u
来源：http://qr.szxytkj.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mo.521024.cn

[Q43] 标量子查询
来源：http://nd.9csxet.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://sf.jctech888.com.cn

[Q44] IN 子查询
来源：http://yc.panjiajie.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://uj.gzmigu.cn

[Q45] EXISTS 判断存在
来源：http://nk.yuntaijiaju.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://gi.jianghongdianzi.cn

[Q46] NOT EXISTS 判断不存在
来源：http://vd.hahajie.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://iy.gzmigu.cn

[Q47] 与平均值比较
来源：http://ep.bookmarksfly.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://st.wgjwhj.cn

[Q48] CTE 公用表表达式
来源：http://aq.hahajie.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://cu.gzmigu.cn

SELECT * FROM t WHERE c > 5;
来源：http://od.huanxung.cn

[Q49] 更新单行
来源：http://nm.chemitech.net.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://zi.panjiajie.cn

[Q50] 批量更新
来源：http://dj.bookmarksfly.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wh.huixiangedu.cn

[Q51] 用子查询更新
来源：http://lv.nszjky.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://xd.colortex.cn

[Q52] 删除指定行
来源：http://eg.huanxung.cn

DELETE FROM users WHERE id = 10;
来源：http://tq.panjiajie.cn

[Q53] 按条件删除
来源：http://qu.nszjky.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://si.nszjky.cn

[Q54] 清空表
来源：http://vc.gzmigu.cn

TRUNCATE TABLE logs;
来源：http://xi.yuntaijiaju.cn

[Q55] 排名（并列占位）
来源：http://gb.gzmigu.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wh.muxihuayi.cn

[Q56] 密集排名（并列不占位）
来源：http://lb.lnxyls.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://fz.yuntaijiaju.cn

[Q57] 行号
来源：http://mk.shtwfgs.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://uj.szxytkj.cn

[Q58] 累计求和
来源：http://ok.yuntaijiaju.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hl.shxzukj.cn

[Q59] 分组内累计
来源：http://gh.muxihuayi.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://zy.panjiajie.cn

[Q60] 取上一行 / 下一行
来源：http://md.jctech888.com.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://vb.shxzskj.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://oj.muxihuayi.cn

[Q61] 移动平均
来源：http://ku.colortex.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://rw.bookmarksfly.cn

[Q62] 分组占比
来源：http://bn.wgjwhj.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://vc.panjiajie.cn

[Q63] 开启事务
来源：http://cw.bjjhwx.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://rd.asd995.cn

[Q64] 提交事务
来源：http://vz.szsharing.cn

COMMIT;
来源：http://ed.panjiajie.cn

[Q65] 回滚事务
来源：http://ig.gzmigu.cn

ROLLBACK;
来源：http://cn.asd995.cn

[Q66] 行锁查询
来源：http://et.shtwfgs.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://fe.asd995.cn

[Q67] 设置隔离级别
来源：http://qf.shxzukj.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://fd.szxytkj.cn

[Q68] 保存点
来源：http://ab.yuexingan06.cn

SAVEPOINT sp1;
来源：http://bd.nszjky.cn

ROLLBACK TO sp1;
来源：http://cv.yuexingan06.cn

[Q69] 查看执行计划
来源：http://ta.hnjuh.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://nr.nicolike.cn

[Q70] 更新统计信息
来源：http://nq.haigaiapp.cn

ANALYZE TABLE users;
来源：http://uv.yuntaijiaju.cn

[Q71] 查看建表语句
来源：http://ga.asd995.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://pg.panjiajie.cn

[Q72] 查看索引
来源：http://mt.bookmarksfly.cn

SHOW INDEX FROM users;
来源：http://af.jctech888.com.cn

[Q73] 查看表状态
来源：http://zn.jianghongdianzi.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://vk.9csxet.cn

[Q74] 强制使用索引
来源：http://wv.bookmarksfly.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hj.jianghongdianzi.cn

[Q75] 日期格式化
来源：http://ba.chemitech.net.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://od.9csxet.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://yp.panjiajie.cn

[Q76] 按天统计
来源：http://xh.huanxung.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://yp.panjiajie.cn

[Q77] 时间加减
来源：http://an.szsharing.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://gw.chemitech.net.cn

[Q78] 当前时间
来源：http://hz.huixiangedu.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://na.yuntaijiaju.cn

[Q79] 字符串拼接
来源：http://yw.nszjky.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mt.szxytkj.cn

[Q80] 字符串截取
来源：http://og.haigaiapp.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://za.szxytkj.cn

[Q81] 字符串替换
来源：http://pp.bookmarksfly.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://pr.bookmarksfly.cn

[Q82] 字符长度与字节长度
来源：http://ub.gzmigu.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://xn.jctech888.com.cn

[Q83] 大小写转换
来源：http://cw.hnjuh.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://od.bjjhwx.cn

[Q84] 去除首尾空格
来源：http://vz.huixiangedu.cn

SELECT TRIM(name) FROM users;
来源：http://vg.muxihuayi.cn

[Q85] 数值取整
来源：http://of.asd995.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://kh.shtwfgs.cn

[Q86] 读取 JSON 字段
来源：http://ym.haigaiapp.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://af.bjjhwx.cn

[Q87] JSON 字段做条件
来源：http://kc.shxzukj.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://es.muxihuayi.cn

[Q88] 行转列（条件聚合）
来源：http://ao.521024.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://pg.panjiajie.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://fm.huanxung.cn

[Q89] 判断表是否存在
来源：http://vg.yuntaijiaju.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ua.muxihuayi.cn

[Q90] 生成序号列
来源：http://pi.chemitech.net.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://oj.newstarts.cn

================================================================================
来源：http://gd.hahajie.cn

R. Bash 专题
来源：http://zw.shtwfgs.cn

================================================================================
来源：http://vn.wgjwhj.cn

[R01] shebang 与严格模式
来源：http://uh.wgjwhj.cn

#!/usr/bin/env bash
来源：http://as.huanxung.cn

set -euo pipefail
来源：http://lm.szxytkj.cn

[R02] 变量赋值与使用
来源：http://gd.hnjuh.cn

name="Tom"; echo "$name"
来源：http://ln.huixiangedu.cn

[R03] 只读变量
来源：http://qg.hnjuh.cn

readonly PI=3.14
来源：http://dl.bjjhwx.cn

[R04] 位置参数
来源：http://ph.wgjwhj.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://av.huixiangedu.cn

[R05] 参数默认值
来源：http://cy.huixiangedu.cn

name="${1:-default}"
来源：http://bq.9csxet.cn

[R06] 判断命令是否存在
来源：http://gr.shxzukj.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://py.nicolike.cn

[R07] if 判断文件
来源：http://fq.gzmigu.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ch.szxytkj.cn

[R08] 数值比较
来源：http://rf.bookmarksfly.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://iz.yuntaijiaju.cn

[R09] 字符串比较
来源：http://ff.huixinmuqiang.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://xc.yuexingan06.cn

[R10] 正则匹配
来源：http://cp.yuexingan06.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ce.chemitech.net.cn

[R11] case 多分支
来源：http://ov.shxzukj.cn

case "$1" in
来源：http://ga.szsharing.cn

start) echo "启动" ;;
来源：http://sy.huixinmuqiang.cn

stop)  echo "停止" ;;
来源：http://ai.bjjhwx.cn

*)     echo "未知命令" ;;
来源：http://ss.shxzukj.cn

esac
来源：http://cs.bjjhwx.cn

[R12] for 遍历文件
来源：http://td.yuexingan06.cn

for f in *.txt; do echo "$f"; done
来源：http://tq.shtwfgs.cn

[R13] for 计数循环
来源：http://qt.newstarts.cn

for i in {1..10}; do echo "$i"; done
来源：http://aj.huixinmuqiang.cn

[R14] C 风格 for
来源：http://xb.hnjuh.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://cx.shxzukj.cn

[R15] while 逐行读文件
来源：http://nu.yuexingan06.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://yh.nicolike.cn

[R16] until 等待条件
来源：http://si.panjiajie.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://tj.szxytkj.cn

[R17] 数组定义与取值
来源：http://kl.yuntaijiaju.cn

arr=(a b c); echo "${arr[0]}"
来源：http://mp.yuntaijiaju.cn

[R18] 遍历数组
来源：http://qy.bjjhwx.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ch.lnxyls.cn

[R19] 数组长度
来源：http://rs.panjiajie.cn

echo "${#arr[@]}"
来源：http://nu.gzmigu.cn

[R20] 关联数组（字典）
来源：http://au.wgjwhj.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://yp.chemitech.net.cn

[R21] 字符串长度
来源：http://vx.jctech888.com.cn

echo "${#s}"
来源：http://jk.szxytkj.cn

[R22] 截取子串
来源：http://ih.521024.cn

echo "${s:0:5}"
来源：http://zd.shtwfgs.cn

[R23] 字符串替换
来源：http://im.wgjwhj.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://um.nszjky.cn

[R24] 大小写转换
来源：http://cl.521024.cn

echo "${s^^}"; echo "${s,,}"
来源：http://tw.yuexingan06.cn

[R25] 去后缀 / 去前缀
来源：http://cu.asd995.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://iv.9csxet.cn

[R26] 命令替换
来源：http://yo.szsharing.cn

now=$(date +%F); echo "$now"
来源：http://ed.newstarts.cn

[R27] 算术展开
来源：http://lc.jctech888.com.cn

echo $((1 + 2 * 3))
来源：http://iz.haigaiapp.cn

[R28] 浮点运算
来源：http://lk.lnxyls.cn

echo "scale=2; 10/3" | bc
来源：http://ad.asd995.cn

[R29] 定义函数
来源：http://ub.nszjky.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://zj.asd995.cn

[R30] 函数返回状态码
来源：http://jw.jianghongdianzi.cn

f() { return 0; }; f || echo "失败了"
来源：http://qp.yuexingan06.cn

[R31] 局部变量
来源：http://wj.szsharing.cn

f() { local x=1; echo "$x"; }
来源：http://qa.nszjky.cn

[R32] 参数个数校验
来源：http://vn.nszjky.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ws.wgjwhj.cn

[R33] 捕获错误并提示行号
来源：http://en.bookmarksfly.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://yv.521024.cn

[R34] 退出时清理
来源：http://bm.yuntaijiaju.cn

trap 'rm -f "$tmp"' EXIT
来源：http://fc.szxytkj.cn

[R35] 后台执行并等待
来源：http://bv.gzmigu.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://qy.asd995.cn

[R36] 并发执行多个任务
来源：http://yt.haigaiapp.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://aw.jctech888.com.cn

[R37] 把输出赋给变量
来源：http://cw.9csxet.cn

files=$(ls -1)
来源：http://hd.bjjhwx.cn

[R38] 管道串联
来源：http://zv.yuexingan06.cn

cat a.txt | grep -i error | wc -l
来源：http://mz.szxytkj.cn

[R39] 重定向标准输出与错误
来源：http://ed.muxihuayi.cn

cmd > out.log 2>&1
来源：http://kk.hnjuh.cn

[R40] 追加写日志
来源：http://tx.szsharing.cn

echo "log" >> out.log
来源：http://oi.panjiajie.cn

[R41] 丢弃输出
来源：http://vq.chemitech.net.cn

cmd >/dev/null 2>&1
来源：http://je.muxihuayi.cn

[R42] 输入重定向
来源：http://hc.nszjky.cn

wc -l < a.txt
来源：http://ej.shxzukj.cn

[R43] 按名字查找文件
来源：http://if.yuexingan06.cn

find . -name "*.log" -type f
来源：http://pf.bookmarksfly.cn

[R44] 按修改时间查找
来源：http://by.panjiajie.cn

find . -mtime -7 -type f
来源：http://fp.newstarts.cn

[R45] 批量删除
来源：http://qr.nszjky.cn

find . -name "*.tmp" -delete
来源：http://vz.haigaiapp.cn

[R46] 递归替换文件内容
来源：http://rs.yuexingan06.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://pd.haigaiapp.cn

[R47] sed 单行替换
来源：http://ul.colortex.cn

sed -i 's/foo/bar/g' a.txt
来源：http://ie.muxihuayi.cn

[R48] awk 取指定列
来源：http://cy.huanxung.cn

awk '{print $1, $3}' a.txt
来源：http://at.huixiangedu.cn

[R49] awk 带条件
来源：http://gh.wgjwhj.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://sn.jianghongdianzi.cn

[R50] awk 求和
来源：http://js.asd995.cn

awk '{s += $2} END {print s}' a.txt
来源：http://ml.muxihuayi.cn

[R51] 排序去重取前几
来源：http://jb.wgjwhj.cn


<!-- 参考信息 -->