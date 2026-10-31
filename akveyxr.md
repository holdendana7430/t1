代发 wailian999

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ps.shxzskj.cn

[Q11] 一次插入多行
来源：http://ty.szxytkj.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://jz.521024.cn

[Q12] 插入后取自增 ID
来源：http://ny.bookmarksfly.cn

INSERT INTO users (name) VALUES ('C');
来源：http://uz.bjjhwx.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mx.shxzukj.cn

[Q13] 忽略重复插入
来源：http://tu.shxzukj.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://sk.shxzskj.cn

[Q14] 存在则更新（upsert）
来源：http://fn.shxzukj.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mf.haigaiapp.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://qn.szsharing.cn

[Q15] 查询全部
来源：http://np.yuexingan06.cn

SELECT * FROM users;
来源：http://hn.yuexingan06.cn

[Q16] 查询指定列
来源：http://ka.bookmarksfly.cn

SELECT id, name FROM users;
来源：http://mj.muxihuayi.cn

[Q17] 条件查询
来源：http://cv.hnjuh.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://lm.lnxyls.cn

[Q18] 模糊匹配
来源：http://wu.yuntaijiaju.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://eb.wgjwhj.cn

[Q19] 范围查询
来源：http://ps.szxytkj.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://pu.hnjuh.cn

[Q20] IN 列表
来源：http://zb.panjiajie.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://po.huixinmuqiang.cn

[Q21] 空值判断
来源：http://vq.hnjuh.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://dy.lnxyls.cn

[Q22] 排序
来源：http://ga.shxzukj.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://fz.asd995.cn

[Q23] 分页
来源：http://lx.shxzskj.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://yr.bjjhwx.cn

[Q24] 去重
来源：http://fb.lnxyls.cn

SELECT DISTINCT city FROM users;
来源：http://ns.huixinmuqiang.cn

[Q25] 只取前 N 条
来源：http://fx.yuntaijiaju.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://yu.huixiangedu.cn

[Q26] 计数
来源：http://ge.9csxet.cn

SELECT COUNT(*) FROM users;
来源：http://tk.haigaiapp.cn

[Q27] 条件计数
来源：http://va.shxzukj.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://tm.bookmarksfly.cn

[Q28] 求和与平均
来源：http://kx.huixiangedu.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://bw.yuntaijiaju.cn

[Q29] 最大最小值
来源：http://ns.chemitech.net.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://rd.shtwfgs.cn

[Q30] 分组统计
来源：http://mh.newstarts.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://jh.jctech888.com.cn

[Q31] 分组后过滤
来源：http://bs.chemitech.net.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://tk.wgjwhj.cn

[Q32] 分组拼接字符串
来源：http://ue.nszjky.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://jb.wgjwhj.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ob.yuexingan06.cn

[Q33] 多列分组
来源：http://qy.yuntaijiaju.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wa.huanxung.cn

[Q34] 每组取第一条
来源：http://ri.lnxyls.cn

SELECT * FROM (
来源：http://wf.szsharing.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://lq.panjiajie.cn

) t WHERE rn = 1;
来源：http://uv.colortex.cn

[Q35] 内连接
来源：http://me.bjjhwx.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://fr.huixinmuqiang.cn

[Q36] 左连接
来源：http://yk.panjiajie.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ys.jianghongdianzi.cn

[Q37] 右连接
来源：http://er.asd995.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://iq.9csxet.cn

[Q38] 全外连接（PostgreSQL）
来源：http://zv.huixiangedu.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ex.yuntaijiaju.cn

[Q39] 自连接（查上下级）
来源：http://dl.nicolike.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://bz.hahajie.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://lk.huanxung.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://yi.shxzskj.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://bh.yuexingan06.cn

[Q41] 多表连接
来源：http://ah.shtwfgs.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://gp.hahajie.cn

JOIN users u ON u.id = o.user_id
来源：http://qf.nszjky.cn

JOIN products p ON p.id = o.product_id;
来源：http://vq.yuntaijiaju.cn

[Q42] 连接条件附加过滤
来源：http://ca.yuntaijiaju.cn

SELECT u.name, o.amount FROM users u
来源：http://fy.nszjky.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://nk.newstarts.cn

[Q43] 标量子查询
来源：http://vg.nicolike.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://nu.bjjhwx.cn

[Q44] IN 子查询
来源：http://bx.muxihuayi.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://bo.newstarts.cn

[Q45] EXISTS 判断存在
来源：http://sm.9csxet.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ob.lnxyls.cn

[Q46] NOT EXISTS 判断不存在
来源：http://ba.yuexingan06.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ol.shxzskj.cn

[Q47] 与平均值比较
来源：http://aq.yuntaijiaju.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://pc.521024.cn

[Q48] CTE 公用表表达式
来源：http://hq.lnxyls.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://vj.nicolike.cn

SELECT * FROM t WHERE c > 5;
来源：http://wl.huanxung.cn

[Q49] 更新单行
来源：http://vl.panjiajie.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://sj.bookmarksfly.cn

[Q50] 批量更新
来源：http://sm.hnjuh.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://pu.muxihuayi.cn

[Q51] 用子查询更新
来源：http://cw.nicolike.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://ar.szsharing.cn

[Q52] 删除指定行
来源：http://wm.shxzukj.cn

DELETE FROM users WHERE id = 10;
来源：http://sv.9csxet.cn

[Q53] 按条件删除
来源：http://zs.szsharing.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ue.wgjwhj.cn

[Q54] 清空表
来源：http://dw.colortex.cn

TRUNCATE TABLE logs;
来源：http://kg.muxihuayi.cn

[Q55] 排名（并列占位）
来源：http://hy.muxihuayi.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://er.jianghongdianzi.cn

[Q56] 密集排名（并列不占位）
来源：http://ii.bjjhwx.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ii.wgjwhj.cn

[Q57] 行号
来源：http://ao.szsharing.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://lu.yuntaijiaju.cn

[Q58] 累计求和
来源：http://ee.9csxet.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://vd.521024.cn

[Q59] 分组内累计
来源：http://lp.lnxyls.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ur.hahajie.cn

[Q60] 取上一行 / 下一行
来源：http://nn.hnjuh.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hn.huixiangedu.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ny.jctech888.com.cn

[Q61] 移动平均
来源：http://rp.newstarts.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ws.colortex.cn

[Q62] 分组占比
来源：http://ez.bookmarksfly.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hh.yuexingan06.cn

[Q63] 开启事务
来源：http://eg.jianghongdianzi.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://nn.huanxung.cn

[Q64] 提交事务
来源：http://yf.szxytkj.cn

COMMIT;
来源：http://tt.huixiangedu.cn

[Q65] 回滚事务
来源：http://wg.bjjhwx.cn

ROLLBACK;
来源：http://uk.gzmigu.cn

[Q66] 行锁查询
来源：http://de.nicolike.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://lz.521024.cn

[Q67] 设置隔离级别
来源：http://tu.bookmarksfly.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://gi.szsharing.cn

[Q68] 保存点
来源：http://lq.9csxet.cn

SAVEPOINT sp1;
来源：http://fd.jctech888.com.cn

ROLLBACK TO sp1;
来源：http://hb.panjiajie.cn

[Q69] 查看执行计划
来源：http://tz.yuexingan06.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://zu.lnxyls.cn

[Q70] 更新统计信息
来源：http://kx.szsharing.cn

ANALYZE TABLE users;
来源：http://pm.nicolike.cn

[Q71] 查看建表语句
来源：http://wg.chemitech.net.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://xa.jctech888.com.cn

[Q72] 查看索引
来源：http://pk.bjjhwx.cn

SHOW INDEX FROM users;
来源：http://cn.yuexingan06.cn

[Q73] 查看表状态
来源：http://dp.jianghongdianzi.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://jp.colortex.cn

[Q74] 强制使用索引
来源：http://zm.chemitech.net.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://pw.nszjky.cn

[Q75] 日期格式化
来源：http://ot.wgjwhj.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://sp.nicolike.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://bt.521024.cn

[Q76] 按天统计
来源：http://hp.lnxyls.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://gw.yuexingan06.cn

[Q77] 时间加减
来源：http://fj.hnjuh.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://md.nszjky.cn

[Q78] 当前时间
来源：http://pw.huixiangedu.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ir.bookmarksfly.cn

[Q79] 字符串拼接
来源：http://mk.gzmigu.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ce.bjjhwx.cn

[Q80] 字符串截取
来源：http://oq.panjiajie.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mw.wgjwhj.cn

[Q81] 字符串替换
来源：http://vb.nszjky.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://pl.521024.cn

[Q82] 字符长度与字节长度
来源：http://ax.newstarts.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://cw.shxzukj.cn

[Q83] 大小写转换
来源：http://sc.bjjhwx.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://vm.9csxet.cn

[Q84] 去除首尾空格
来源：http://hx.bookmarksfly.cn

SELECT TRIM(name) FROM users;
来源：http://gq.szsharing.cn

[Q85] 数值取整
来源：http://os.nicolike.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.huixiangedu.cn

[Q86] 读取 JSON 字段
来源：http://bm.nszjky.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://xs.jianghongdianzi.cn

[Q87] JSON 字段做条件
来源：http://zr.9csxet.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://se.panjiajie.cn

[Q88] 行转列（条件聚合）
来源：http://zi.colortex.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ci.gzmigu.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://uo.9csxet.cn

[Q89] 判断表是否存在
来源：http://gm.wgjwhj.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ee.nicolike.cn

[Q90] 生成序号列
来源：http://er.wgjwhj.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wo.chemitech.net.cn

================================================================================
来源：http://xn.newstarts.cn

R. Bash 专题
来源：http://qt.yuexingan06.cn

================================================================================
来源：http://wv.521024.cn

[R01] shebang 与严格模式
来源：http://bn.9csxet.cn

#!/usr/bin/env bash
来源：http://le.hnjuh.cn

set -euo pipefail
来源：http://sn.shtwfgs.cn

[R02] 变量赋值与使用
来源：http://ld.huixinmuqiang.cn

name="Tom"; echo "$name"
来源：http://ps.asd995.cn

[R03] 只读变量
来源：http://aj.shxzukj.cn

readonly PI=3.14
来源：http://vq.bjjhwx.cn

[R04] 位置参数
来源：http://jt.chemitech.net.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mc.hnjuh.cn

[R05] 参数默认值
来源：http://qb.9csxet.cn

name="${1:-default}"
来源：http://ef.muxihuayi.cn

[R06] 判断命令是否存在
来源：http://rv.colortex.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ej.yuntaijiaju.cn

[R07] if 判断文件
来源：http://fl.huanxung.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://fc.9csxet.cn

[R08] 数值比较
来源：http://fr.jctech888.com.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://lt.szxytkj.cn

[R09] 字符串比较
来源：http://vx.nszjky.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://as.huanxung.cn

[R10] 正则匹配
来源：http://uh.jctech888.com.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://bd.hnjuh.cn

[R11] case 多分支
来源：http://ih.nicolike.cn

case "$1" in
来源：http://pl.haigaiapp.cn

start) echo "启动" ;;
来源：http://da.lnxyls.cn

stop)  echo "停止" ;;
来源：http://ox.yuntaijiaju.cn

*)     echo "未知命令" ;;
来源：http://bp.chemitech.net.cn

esac
来源：http://sb.asd995.cn

[R12] for 遍历文件
来源：http://va.521024.cn

for f in *.txt; do echo "$f"; done
来源：http://tx.yuntaijiaju.cn

[R13] for 计数循环
来源：http://hd.gzmigu.cn

for i in {1..10}; do echo "$i"; done
来源：http://fj.bookmarksfly.cn

[R14] C 风格 for
来源：http://bt.muxihuayi.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://xc.szsharing.cn

[R15] while 逐行读文件
来源：http://tf.huanxung.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://em.jctech888.com.cn

[R16] until 等待条件
来源：http://lz.huixinmuqiang.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://kn.bjjhwx.cn

[R17] 数组定义与取值
来源：http://gw.yuexingan06.cn

arr=(a b c); echo "${arr[0]}"
来源：http://bt.521024.cn

[R18] 遍历数组
来源：http://ye.huixinmuqiang.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://up.nicolike.cn

[R19] 数组长度
来源：http://vw.yuexingan06.cn

echo "${#arr[@]}"
来源：http://wl.muxihuayi.cn

[R20] 关联数组（字典）
来源：http://rj.shxzukj.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://tj.nicolike.cn

[R21] 字符串长度
来源：http://st.shxzukj.cn

echo "${#s}"
来源：http://sn.asd995.cn

[R22] 截取子串
来源：http://jf.bookmarksfly.cn

echo "${s:0:5}"
来源：http://mo.gzmigu.cn

[R23] 字符串替换
来源：http://lq.shtwfgs.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://gx.nszjky.cn

[R24] 大小写转换
来源：http://by.nszjky.cn

echo "${s^^}"; echo "${s,,}"
来源：http://pk.huanxung.cn

[R25] 去后缀 / 去前缀
来源：http://qe.panjiajie.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://go.jianghongdianzi.cn

[R26] 命令替换
来源：http://ih.521024.cn

now=$(date +%F); echo "$now"
来源：http://nt.asd995.cn

[R27] 算术展开
来源：http://dp.colortex.cn

echo $((1 + 2 * 3))
来源：http://ot.newstarts.cn

[R28] 浮点运算
来源：http://kk.haigaiapp.cn

echo "scale=2; 10/3" | bc
来源：http://ng.nszjky.cn

[R29] 定义函数
来源：http://ju.szsharing.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://qo.nszjky.cn

[R30] 函数返回状态码
来源：http://az.asd995.cn

f() { return 0; }; f || echo "失败了"
来源：http://pp.muxihuayi.cn

[R31] 局部变量
来源：http://vd.panjiajie.cn

f() { local x=1; echo "$x"; }
来源：http://xo.newstarts.cn

[R32] 参数个数校验
来源：http://ea.521024.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://kp.shxzukj.cn

[R33] 捕获错误并提示行号
来源：http://zc.huixinmuqiang.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://jj.shxzskj.cn

[R34] 退出时清理
来源：http://fk.jctech888.com.cn

trap 'rm -f "$tmp"' EXIT
来源：http://bm.yuntaijiaju.cn

[R35] 后台执行并等待
来源：http://qe.bookmarksfly.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://rr.gzmigu.cn

[R36] 并发执行多个任务
来源：http://yo.lnxyls.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://lk.szsharing.cn

[R37] 把输出赋给变量
来源：http://bp.jctech888.com.cn

files=$(ls -1)
来源：http://kj.shxzukj.cn

[R38] 管道串联
来源：http://ez.hnjuh.cn

cat a.txt | grep -i error | wc -l
来源：http://cz.huanxung.cn

[R39] 重定向标准输出与错误
来源：http://yc.shxzskj.cn

cmd > out.log 2>&1
来源：http://gr.huixinmuqiang.cn

[R40] 追加写日志
来源：http://rt.haigaiapp.cn

echo "log" >> out.log
来源：http://ud.szxytkj.cn

[R41] 丢弃输出
来源：http://gn.huixiangedu.cn

cmd >/dev/null 2>&1
来源：http://uj.hahajie.cn

[R42] 输入重定向
来源：http://pp.jctech888.com.cn

wc -l < a.txt
来源：http://go.szxytkj.cn

[R43] 按名字查找文件
来源：http://iy.jianghongdianzi.cn

find . -name "*.log" -type f
来源：http://fd.muxihuayi.cn

[R44] 按修改时间查找
来源：http://ei.hnjuh.cn

find . -mtime -7 -type f
来源：http://gq.muxihuayi.cn

[R45] 批量删除
来源：http://hi.asd995.cn

find . -name "*.tmp" -delete
来源：http://jc.newstarts.cn

[R46] 递归替换文件内容
来源：http://ir.521024.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ye.hahajie.cn

[R47] sed 单行替换
来源：http://wo.haigaiapp.cn

sed -i 's/foo/bar/g' a.txt
来源：http://kw.jctech888.com.cn

[R48] awk 取指定列
来源：http://xk.521024.cn

awk '{print $1, $3}' a.txt
来源：http://hz.521024.cn

[R49] awk 带条件
来源：http://gh.hnjuh.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hk.haigaiapp.cn

[R50] awk 求和
来源：http://rq.yuntaijiaju.cn

awk '{s += $2} END {print s}' a.txt
来源：http://ue.jctech888.com.cn

[R51] 排序去重取前几
来源：http://xv.szxytkj.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://xt.bjjhwx.cn

[R52] 统计行数
来源：http://qf.hahajie.cn

wc -l a.txt
来源：http://sn.9csxet.cn

[R53] 查看文件头与实时尾
来源：http://wo.jctech888.com.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://tw.9csxet.cn

[R54] 比较两个文件
来源：http://hy.wgjwhj.cn

diff a.txt b.txt
来源：http://xy.jctech888.com.cn

[R55] 压缩与解压
来源：http://yi.panjiajie.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://dy.haigaiapp.cn

[R56] 远程拷贝
来源：http://gb.huixiangedu.cn

scp file user@host:/path/
来源：http://nr.newstarts.cn

[R57] 远程执行命令
来源：http://ga.bjjhwx.cn

ssh user@host 'uptime'
来源：http://kn.colortex.cn

[R58] 下载文件
来源：http://zn.hahajie.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://fg.521024.cn

[R59] 发 POST JSON
来源：http://sz.szxytkj.cn


<!-- 参考信息 -->