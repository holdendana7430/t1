代发 wailian999

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://sc.hnjuh.cn

[Q05] 重命名列
来源：http://rf.huixiangedu.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://bx.shxzskj.cn

[Q06] 删除列
来源：http://bt.szsharing.cn

ALTER TABLE users DROP COLUMN age;
来源：http://vv.colortex.cn

[Q07] 删除表
来源：http://wf.521024.cn

DROP TABLE IF EXISTS orders;
来源：http://jy.bookmarksfly.cn

[Q08] 创建普通索引
来源：http://lk.haigaiapp.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://wo.wgjwhj.cn

[Q09] 创建唯一索引
来源：http://tu.lnxyls.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://yi.shtwfgs.cn

[Q10] 插入单行
来源：http://nr.shxzskj.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://de.nszjky.cn

[Q11] 一次插入多行
来源：http://ws.huixiangedu.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://zy.huixiangedu.cn

[Q12] 插入后取自增 ID
来源：http://jv.bjjhwx.cn

INSERT INTO users (name) VALUES ('C');
来源：http://rg.haigaiapp.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hn.wgjwhj.cn

[Q13] 忽略重复插入
来源：http://vk.muxihuayi.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://co.shxzskj.cn

[Q14] 存在则更新（upsert）
来源：http://iw.nszjky.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://uk.haigaiapp.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://bi.shxzukj.cn

[Q15] 查询全部
来源：http://ep.bjjhwx.cn

SELECT * FROM users;
来源：http://qq.gzmigu.cn

[Q16] 查询指定列
来源：http://bb.gzmigu.cn

SELECT id, name FROM users;
来源：http://ls.bjjhwx.cn

[Q17] 条件查询
来源：http://bz.9csxet.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://jk.521024.cn

[Q18] 模糊匹配
来源：http://ml.wgjwhj.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mq.nicolike.cn

[Q19] 范围查询
来源：http://jj.jianghongdianzi.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://iy.nszjky.cn

[Q20] IN 列表
来源：http://bc.shtwfgs.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://fa.haigaiapp.cn

[Q21] 空值判断
来源：http://xp.nszjky.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://wc.huixinmuqiang.cn

[Q22] 排序
来源：http://qu.panjiajie.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ja.hnjuh.cn

[Q23] 分页
来源：http://wt.hnjuh.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://bx.gzmigu.cn

[Q24] 去重
来源：http://md.yuntaijiaju.cn

SELECT DISTINCT city FROM users;
来源：http://kf.nicolike.cn

[Q25] 只取前 N 条
来源：http://cx.hnjuh.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://gc.szxytkj.cn

[Q26] 计数
来源：http://uy.muxihuayi.cn

SELECT COUNT(*) FROM users;
来源：http://bs.panjiajie.cn

[Q27] 条件计数
来源：http://ec.jianghongdianzi.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://zq.szxytkj.cn

[Q28] 求和与平均
来源：http://va.huanxung.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://fv.521024.cn

[Q29] 最大最小值
来源：http://du.bjjhwx.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://jq.521024.cn

[Q30] 分组统计
来源：http://gx.bjjhwx.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://vm.szsharing.cn

[Q31] 分组后过滤
来源：http://mv.nicolike.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ri.yuexingan06.cn

[Q32] 分组拼接字符串
来源：http://gs.hnjuh.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ng.9csxet.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ob.panjiajie.cn

[Q33] 多列分组
来源：http://ww.jctech888.com.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://bm.shxzukj.cn

[Q34] 每组取第一条
来源：http://vg.jianghongdianzi.cn

SELECT * FROM (
来源：http://ju.shtwfgs.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://yo.chemitech.net.cn

) t WHERE rn = 1;
来源：http://oe.nicolike.cn

[Q35] 内连接
来源：http://ln.nicolike.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://kf.nszjky.cn

[Q36] 左连接
来源：http://rl.lnxyls.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ae.9csxet.cn

[Q37] 右连接
来源：http://so.yuntaijiaju.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wv.szxytkj.cn

[Q38] 全外连接（PostgreSQL）
来源：http://jd.haigaiapp.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wv.521024.cn

[Q39] 自连接（查上下级）
来源：http://pc.bjjhwx.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://np.wgjwhj.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://rz.9csxet.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://hi.newstarts.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://bq.huanxung.cn

[Q41] 多表连接
来源：http://qy.muxihuayi.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://ti.szxytkj.cn

JOIN users u ON u.id = o.user_id
来源：http://yj.wgjwhj.cn

JOIN products p ON p.id = o.product_id;
来源：http://vn.huixinmuqiang.cn

[Q42] 连接条件附加过滤
来源：http://fe.muxihuayi.cn

SELECT u.name, o.amount FROM users u
来源：http://mr.lnxyls.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://nh.jianghongdianzi.cn

[Q43] 标量子查询
来源：http://jn.521024.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://kz.huanxung.cn

[Q44] IN 子查询
来源：http://si.muxihuayi.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://jx.chemitech.net.cn

[Q45] EXISTS 判断存在
来源：http://jp.shxzskj.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ti.newstarts.cn

[Q46] NOT EXISTS 判断不存在
来源：http://az.bookmarksfly.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wg.nicolike.cn

[Q47] 与平均值比较
来源：http://su.newstarts.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://at.nszjky.cn

[Q48] CTE 公用表表达式
来源：http://pr.muxihuayi.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hm.yuntaijiaju.cn

SELECT * FROM t WHERE c > 5;
来源：http://fv.bookmarksfly.cn

[Q49] 更新单行
来源：http://xd.gzmigu.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://pb.chemitech.net.cn

[Q50] 批量更新
来源：http://xk.hnjuh.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://tv.shxzskj.cn

[Q51] 用子查询更新
来源：http://dh.gzmigu.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wh.huixiangedu.cn

[Q52] 删除指定行
来源：http://ht.panjiajie.cn

DELETE FROM users WHERE id = 10;
来源：http://zn.haigaiapp.cn

[Q53] 按条件删除
来源：http://le.hnjuh.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mt.yuexingan06.cn

[Q54] 清空表
来源：http://ft.asd995.cn

TRUNCATE TABLE logs;
来源：http://dw.muxihuayi.cn

[Q55] 排名（并列占位）
来源：http://sz.wgjwhj.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://kn.wgjwhj.cn

[Q56] 密集排名（并列不占位）
来源：http://kp.shxzskj.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://gw.gzmigu.cn

[Q57] 行号
来源：http://ys.bjjhwx.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ey.nicolike.cn

[Q58] 累计求和
来源：http://aq.haigaiapp.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://jc.shxzukj.cn

[Q59] 分组内累计
来源：http://kq.nszjky.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://pi.asd995.cn

[Q60] 取上一行 / 下一行
来源：http://fk.hahajie.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://kc.wgjwhj.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://xf.jianghongdianzi.cn

[Q61] 移动平均
来源：http://wm.haigaiapp.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://qx.shxzskj.cn

[Q62] 分组占比
来源：http://bu.hnjuh.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://jj.shtwfgs.cn

[Q63] 开启事务
来源：http://fj.colortex.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://aa.521024.cn

[Q64] 提交事务
来源：http://wz.huixinmuqiang.cn

COMMIT;
来源：http://qm.bookmarksfly.cn

[Q65] 回滚事务
来源：http://fv.shxzskj.cn

ROLLBACK;
来源：http://eo.huanxung.cn

[Q66] 行锁查询
来源：http://hy.521024.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://zp.gzmigu.cn

[Q67] 设置隔离级别
来源：http://ds.nicolike.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://iz.yuexingan06.cn

[Q68] 保存点
来源：http://be.gzmigu.cn

SAVEPOINT sp1;
来源：http://ul.asd995.cn

ROLLBACK TO sp1;
来源：http://am.panjiajie.cn

[Q69] 查看执行计划
来源：http://op.jctech888.com.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://pe.panjiajie.cn

[Q70] 更新统计信息
来源：http://uu.huanxung.cn

ANALYZE TABLE users;
来源：http://yr.shxzskj.cn

[Q71] 查看建表语句
来源：http://ag.asd995.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://tf.huixinmuqiang.cn

[Q72] 查看索引
来源：http://bg.newstarts.cn

SHOW INDEX FROM users;
来源：http://rs.shxzskj.cn

[Q73] 查看表状态
来源：http://ws.colortex.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://wp.lnxyls.cn

[Q74] 强制使用索引
来源：http://pj.huixinmuqiang.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://dy.huixinmuqiang.cn

[Q75] 日期格式化
来源：http://wy.bjjhwx.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://vw.9csxet.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://lw.szsharing.cn

[Q76] 按天统计
来源：http://iu.haigaiapp.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mp.chemitech.net.cn

[Q77] 时间加减
来源：http://cq.hnjuh.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hm.bookmarksfly.cn

[Q78] 当前时间
来源：http://fo.bookmarksfly.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://oa.lnxyls.cn

[Q79] 字符串拼接
来源：http://fe.jctech888.com.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://uo.haigaiapp.cn

[Q80] 字符串截取
来源：http://aq.jctech888.com.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://so.gzmigu.cn

[Q81] 字符串替换
来源：http://bj.szxytkj.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://vt.shtwfgs.cn

[Q82] 字符长度与字节长度
来源：http://hs.huixiangedu.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://dv.panjiajie.cn

[Q83] 大小写转换
来源：http://am.nszjky.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://sv.jctech888.com.cn

[Q84] 去除首尾空格
来源：http://bg.shtwfgs.cn

SELECT TRIM(name) FROM users;
来源：http://rf.asd995.cn

[Q85] 数值取整
来源：http://oj.szsharing.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ov.jctech888.com.cn

[Q86] 读取 JSON 字段
来源：http://rp.521024.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://et.shxzukj.cn

[Q87] JSON 字段做条件
来源：http://gx.jianghongdianzi.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://iw.shxzskj.cn

[Q88] 行转列（条件聚合）
来源：http://qd.huanxung.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://qr.hahajie.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://uz.colortex.cn

[Q89] 判断表是否存在
来源：http://pp.lnxyls.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://tr.yuntaijiaju.cn

[Q90] 生成序号列
来源：http://lf.chemitech.net.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://sv.gzmigu.cn

================================================================================
来源：http://kv.jianghongdianzi.cn

R. Bash 专题
来源：http://pk.wgjwhj.cn

================================================================================
来源：http://gp.bjjhwx.cn

[R01] shebang 与严格模式
来源：http://mp.hahajie.cn

#!/usr/bin/env bash
来源：http://yz.chemitech.net.cn

set -euo pipefail
来源：http://xt.chemitech.net.cn

[R02] 变量赋值与使用
来源：http://gc.huixinmuqiang.cn

name="Tom"; echo "$name"
来源：http://nu.9csxet.cn

[R03] 只读变量
来源：http://fa.hahajie.cn

readonly PI=3.14
来源：http://zp.shxzukj.cn

[R04] 位置参数
来源：http://ob.9csxet.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://fu.asd995.cn

[R05] 参数默认值
来源：http://ya.szsharing.cn

name="${1:-default}"
来源：http://lw.9csxet.cn

[R06] 判断命令是否存在
来源：http://no.bjjhwx.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://kf.gzmigu.cn

[R07] if 判断文件
来源：http://qj.hnjuh.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://pu.nicolike.cn

[R08] 数值比较
来源：http://ef.bookmarksfly.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://bk.jianghongdianzi.cn

[R09] 字符串比较
来源：http://dm.haigaiapp.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://jp.bjjhwx.cn

[R10] 正则匹配
来源：http://xm.wgjwhj.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://us.hahajie.cn

[R11] case 多分支
来源：http://dt.shtwfgs.cn

case "$1" in
来源：http://mm.jctech888.com.cn

start) echo "启动" ;;
来源：http://dg.asd995.cn

stop)  echo "停止" ;;
来源：http://op.chemitech.net.cn

*)     echo "未知命令" ;;
来源：http://rz.huixiangedu.cn

esac
来源：http://lq.haigaiapp.cn

[R12] for 遍历文件
来源：http://rc.bookmarksfly.cn

for f in *.txt; do echo "$f"; done
来源：http://wz.szxytkj.cn

[R13] for 计数循环
来源：http://nl.chemitech.net.cn

for i in {1..10}; do echo "$i"; done
来源：http://io.yuexingan06.cn

[R14] C 风格 for
来源：http://ju.lnxyls.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://iv.wgjwhj.cn

[R15] while 逐行读文件
来源：http://ys.yuexingan06.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ix.wgjwhj.cn

[R16] until 等待条件
来源：http://de.hnjuh.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mt.shxzukj.cn

[R17] 数组定义与取值
来源：http://fa.shxzukj.cn

arr=(a b c); echo "${arr[0]}"
来源：http://by.hnjuh.cn

[R18] 遍历数组
来源：http://qz.nicolike.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mo.szxytkj.cn

[R19] 数组长度
来源：http://rj.panjiajie.cn

echo "${#arr[@]}"
来源：http://mm.huanxung.cn

[R20] 关联数组（字典）
来源：http://du.asd995.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://iz.lnxyls.cn

[R21] 字符串长度
来源：http://vg.wgjwhj.cn

echo "${#s}"
来源：http://qu.shxzskj.cn

[R22] 截取子串
来源：http://kf.shxzukj.cn

echo "${s:0:5}"
来源：http://fe.panjiajie.cn

[R23] 字符串替换
来源：http://ne.szxytkj.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://sg.huanxung.cn

[R24] 大小写转换
来源：http://ag.hahajie.cn

echo "${s^^}"; echo "${s,,}"
来源：http://im.shxzskj.cn

[R25] 去后缀 / 去前缀
来源：http://zt.yuntaijiaju.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://cn.nicolike.cn

[R26] 命令替换
来源：http://cu.bjjhwx.cn

now=$(date +%F); echo "$now"
来源：http://fr.szsharing.cn

[R27] 算术展开
来源：http://by.panjiajie.cn

echo $((1 + 2 * 3))
来源：http://rh.shxzukj.cn

[R28] 浮点运算
来源：http://nd.bookmarksfly.cn

echo "scale=2; 10/3" | bc
来源：http://ma.szsharing.cn

[R29] 定义函数
来源：http://ku.colortex.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://cu.haigaiapp.cn

[R30] 函数返回状态码
来源：http://tm.huixiangedu.cn

f() { return 0; }; f || echo "失败了"
来源：http://uc.nszjky.cn

[R31] 局部变量
来源：http://jo.muxihuayi.cn

f() { local x=1; echo "$x"; }
来源：http://np.shxzskj.cn

[R32] 参数个数校验
来源：http://bf.521024.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://dl.nszjky.cn

[R33] 捕获错误并提示行号
来源：http://kr.shtwfgs.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://xs.jctech888.com.cn

[R34] 退出时清理
来源：http://qp.bookmarksfly.cn

trap 'rm -f "$tmp"' EXIT
来源：http://ar.shtwfgs.cn

[R35] 后台执行并等待
来源：http://ay.panjiajie.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://ba.yuntaijiaju.cn

[R36] 并发执行多个任务
来源：http://ip.jctech888.com.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://rx.jianghongdianzi.cn

[R37] 把输出赋给变量
来源：http://bc.panjiajie.cn

files=$(ls -1)
来源：http://vj.szsharing.cn

[R38] 管道串联
来源：http://gx.shtwfgs.cn

cat a.txt | grep -i error | wc -l
来源：http://bg.szxytkj.cn

[R39] 重定向标准输出与错误
来源：http://bg.nicolike.cn

cmd > out.log 2>&1
来源：http://nh.chemitech.net.cn

[R40] 追加写日志
来源：http://hx.hahajie.cn

echo "log" >> out.log
来源：http://mg.asd995.cn

[R41] 丢弃输出
来源：http://se.lnxyls.cn

cmd >/dev/null 2>&1
来源：http://pz.yuntaijiaju.cn

[R42] 输入重定向
来源：http://zv.shxzukj.cn

wc -l < a.txt
来源：http://ca.szxytkj.cn

[R43] 按名字查找文件
来源：http://yn.muxihuayi.cn

find . -name "*.log" -type f
来源：http://ed.panjiajie.cn

[R44] 按修改时间查找
来源：http://tr.bjjhwx.cn

find . -mtime -7 -type f
来源：http://kl.yuntaijiaju.cn

[R45] 批量删除
来源：http://cy.panjiajie.cn

find . -name "*.tmp" -delete
来源：http://yd.bookmarksfly.cn

[R46] 递归替换文件内容
来源：http://gf.colortex.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://rb.shtwfgs.cn

[R47] sed 单行替换
来源：http://xl.lnxyls.cn

sed -i 's/foo/bar/g' a.txt
来源：http://tk.huixiangedu.cn

[R48] awk 取指定列
来源：http://rw.521024.cn

awk '{print $1, $3}' a.txt
来源：http://ci.shtwfgs.cn

[R49] awk 带条件
来源：http://ai.newstarts.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://fg.nicolike.cn

[R50] awk 求和
来源：http://hk.lnxyls.cn

awk '{s += $2} END {print s}' a.txt
来源：http://nj.shtwfgs.cn

[R51] 排序去重取前几
来源：http://xl.huixinmuqiang.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://ht.yuexingan06.cn

[R52] 统计行数
来源：http://gk.bjjhwx.cn

wc -l a.txt
来源：http://eg.shxzukj.cn

[R53] 查看文件头与实时尾
来源：http://hy.newstarts.cn


<!-- 参考信息 -->