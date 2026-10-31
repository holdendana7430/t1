代发 wailian999

INSERT INTO users (name) VALUES ('C');
来源：http://pb.hnjuh.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://tj.gzmigu.cn

[Q13] 忽略重复插入
来源：http://sn.hnjuh.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://iz.yuexingan06.cn

[Q14] 存在则更新（upsert）
来源：http://qd.shxzskj.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://cs.jianghongdianzi.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://dx.muxihuayi.cn

[Q15] 查询全部
来源：http://wg.chemitech.net.cn

SELECT * FROM users;
来源：http://yw.nszjky.cn

[Q16] 查询指定列
来源：http://ln.9csxet.cn

SELECT id, name FROM users;
来源：http://me.jctech888.com.cn

[Q17] 条件查询
来源：http://fa.bookmarksfly.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mo.gzmigu.cn

[Q18] 模糊匹配
来源：http://wj.521024.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://et.huixinmuqiang.cn

[Q19] 范围查询
来源：http://gp.shtwfgs.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://lz.gzmigu.cn

[Q20] IN 列表
来源：http://sa.hnjuh.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://kx.9csxet.cn

[Q21] 空值判断
来源：http://yi.colortex.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://gs.gzmigu.cn

[Q22] 排序
来源：http://np.huixiangedu.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ey.asd995.cn

[Q23] 分页
来源：http://nc.gzmigu.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://pm.nicolike.cn

[Q24] 去重
来源：http://tl.huixiangedu.cn

SELECT DISTINCT city FROM users;
来源：http://wp.huanxung.cn

[Q25] 只取前 N 条
来源：http://mn.panjiajie.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://no.szxytkj.cn

[Q26] 计数
来源：http://ka.bookmarksfly.cn

SELECT COUNT(*) FROM users;
来源：http://st.nicolike.cn

[Q27] 条件计数
来源：http://do.gzmigu.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://eo.gzmigu.cn

[Q28] 求和与平均
来源：http://ja.9csxet.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wg.bjjhwx.cn

[Q29] 最大最小值
来源：http://so.jctech888.com.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://xv.haigaiapp.cn

[Q30] 分组统计
来源：http://bf.hahajie.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://tn.hahajie.cn

[Q31] 分组后过滤
来源：http://kj.asd995.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://sp.bookmarksfly.cn

[Q32] 分组拼接字符串
来源：http://mb.yuntaijiaju.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://pe.nicolike.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://je.muxihuayi.cn

[Q33] 多列分组
来源：http://zv.nicolike.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://dq.yuntaijiaju.cn

[Q34] 每组取第一条
来源：http://bk.colortex.cn

SELECT * FROM (
来源：http://bu.asd995.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://pj.asd995.cn

) t WHERE rn = 1;
来源：http://rj.9csxet.cn

[Q35] 内连接
来源：http://vp.jctech888.com.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://qa.bjjhwx.cn

[Q36] 左连接
来源：http://yx.chemitech.net.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://yh.huixinmuqiang.cn

[Q37] 右连接
来源：http://rf.huixiangedu.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://dd.521024.cn

[Q38] 全外连接（PostgreSQL）
来源：http://lz.wgjwhj.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ud.panjiajie.cn

[Q39] 自连接（查上下级）
来源：http://rd.huixiangedu.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://se.jianghongdianzi.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://sg.nszjky.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://yy.lnxyls.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://jg.521024.cn

[Q41] 多表连接
来源：http://xc.9csxet.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://qj.wgjwhj.cn

JOIN users u ON u.id = o.user_id
来源：http://px.gzmigu.cn

JOIN products p ON p.id = o.product_id;
来源：http://lu.shxzukj.cn

[Q42] 连接条件附加过滤
来源：http://wx.huanxung.cn

SELECT u.name, o.amount FROM users u
来源：http://cd.shxzskj.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://uw.yuexingan06.cn

[Q43] 标量子查询
来源：http://cw.huanxung.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://jm.lnxyls.cn

[Q44] IN 子查询
来源：http://ar.yuexingan06.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://cf.newstarts.cn

[Q45] EXISTS 判断存在
来源：http://cl.chemitech.net.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ja.panjiajie.cn

[Q46] NOT EXISTS 判断不存在
来源：http://og.nszjky.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://nj.hahajie.cn

[Q47] 与平均值比较
来源：http://lh.gzmigu.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://zl.521024.cn

[Q48] CTE 公用表表达式
来源：http://ok.9csxet.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://rr.yuntaijiaju.cn

SELECT * FROM t WHERE c > 5;
来源：http://jn.bjjhwx.cn

[Q49] 更新单行
来源：http://hr.huanxung.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://zq.asd995.cn

[Q50] 批量更新
来源：http://zp.huixiangedu.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mc.panjiajie.cn

[Q51] 用子查询更新
来源：http://xu.bookmarksfly.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://ib.hnjuh.cn

[Q52] 删除指定行
来源：http://ce.yuntaijiaju.cn

DELETE FROM users WHERE id = 10;
来源：http://ay.nszjky.cn

[Q53] 按条件删除
来源：http://vd.szxytkj.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://me.huanxung.cn

[Q54] 清空表
来源：http://oh.huanxung.cn

TRUNCATE TABLE logs;
来源：http://sz.huixinmuqiang.cn

[Q55] 排名（并列占位）
来源：http://td.shxzukj.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://fn.jctech888.com.cn

[Q56] 密集排名（并列不占位）
来源：http://bo.yuntaijiaju.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hf.newstarts.cn

[Q57] 行号
来源：http://jr.shxzukj.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://qk.panjiajie.cn

[Q58] 累计求和
来源：http://ah.muxihuayi.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://xj.jctech888.com.cn

[Q59] 分组内累计
来源：http://ks.huixinmuqiang.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://qx.nicolike.cn

[Q60] 取上一行 / 下一行
来源：http://ri.newstarts.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hr.nszjky.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://uf.wgjwhj.cn

[Q61] 移动平均
来源：http://kz.asd995.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://sj.colortex.cn

[Q62] 分组占比
来源：http://uq.jctech888.com.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ba.lnxyls.cn

[Q63] 开启事务
来源：http://cd.shtwfgs.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://op.nicolike.cn

[Q64] 提交事务
来源：http://wr.newstarts.cn

COMMIT;
来源：http://ca.asd995.cn

[Q65] 回滚事务
来源：http://dx.haigaiapp.cn

ROLLBACK;
来源：http://dw.szxytkj.cn

[Q66] 行锁查询
来源：http://dv.newstarts.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mt.huanxung.cn

[Q67] 设置隔离级别
来源：http://eq.nicolike.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://cb.newstarts.cn

[Q68] 保存点
来源：http://ce.lnxyls.cn

SAVEPOINT sp1;
来源：http://wy.asd995.cn

ROLLBACK TO sp1;
来源：http://yh.newstarts.cn

[Q69] 查看执行计划
来源：http://wb.nicolike.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://lt.hahajie.cn

[Q70] 更新统计信息
来源：http://uo.9csxet.cn

ANALYZE TABLE users;
来源：http://xc.colortex.cn

[Q71] 查看建表语句
来源：http://oj.haigaiapp.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://zg.huanxung.cn

[Q72] 查看索引
来源：http://nf.newstarts.cn

SHOW INDEX FROM users;
来源：http://pn.bookmarksfly.cn

[Q73] 查看表状态
来源：http://vt.colortex.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://hy.shxzukj.cn

[Q74] 强制使用索引
来源：http://ty.colortex.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://bt.muxihuayi.cn

[Q75] 日期格式化
来源：http://me.szxytkj.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://jv.huixiangedu.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://gg.yuntaijiaju.cn

[Q76] 按天统计
来源：http://jw.chemitech.net.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://rw.jctech888.com.cn

[Q77] 时间加减
来源：http://kx.lnxyls.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mc.jianghongdianzi.cn

[Q78] 当前时间
来源：http://mu.newstarts.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://jb.lnxyls.cn

[Q79] 字符串拼接
来源：http://rs.shtwfgs.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mz.huanxung.cn

[Q80] 字符串截取
来源：http://md.szxytkj.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ku.lnxyls.cn

[Q81] 字符串替换
来源：http://vc.newstarts.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mj.asd995.cn

[Q82] 字符长度与字节长度
来源：http://px.shxzskj.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://lv.yuntaijiaju.cn

[Q83] 大小写转换
来源：http://hx.hahajie.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ui.nicolike.cn

[Q84] 去除首尾空格
来源：http://hd.newstarts.cn

SELECT TRIM(name) FROM users;
来源：http://my.yuntaijiaju.cn

[Q85] 数值取整
来源：http://fb.gzmigu.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://jp.asd995.cn

[Q86] 读取 JSON 字段
来源：http://xo.wgjwhj.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://lk.muxihuayi.cn

[Q87] JSON 字段做条件
来源：http://gp.521024.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://fl.huixiangedu.cn

[Q88] 行转列（条件聚合）
来源：http://zz.jctech888.com.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://jv.szxytkj.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://kc.521024.cn

[Q89] 判断表是否存在
来源：http://rr.huixiangedu.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ry.nszjky.cn

[Q90] 生成序号列
来源：http://li.gzmigu.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://qq.521024.cn

================================================================================
来源：http://pg.huixinmuqiang.cn

R. Bash 专题
来源：http://zx.gzmigu.cn

================================================================================
来源：http://si.bjjhwx.cn

[R01] shebang 与严格模式
来源：http://ih.newstarts.cn

#!/usr/bin/env bash
来源：http://ts.huixiangedu.cn

set -euo pipefail
来源：http://tk.hahajie.cn

[R02] 变量赋值与使用
来源：http://uv.hahajie.cn

name="Tom"; echo "$name"
来源：http://zq.yuntaijiaju.cn

[R03] 只读变量
来源：http://ov.shxzukj.cn

readonly PI=3.14
来源：http://nb.haigaiapp.cn

[R04] 位置参数
来源：http://lm.jctech888.com.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wc.asd995.cn

[R05] 参数默认值
来源：http://an.9csxet.cn

name="${1:-default}"
来源：http://wz.szxytkj.cn

[R06] 判断命令是否存在
来源：http://zr.muxihuayi.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ow.hahajie.cn

[R07] if 判断文件
来源：http://jb.szxytkj.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://cs.gzmigu.cn

[R08] 数值比较
来源：http://rk.muxihuayi.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://sg.shxzskj.cn

[R09] 字符串比较
来源：http://az.9csxet.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hi.nszjky.cn

[R10] 正则匹配
来源：http://qu.huanxung.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mq.yuexingan06.cn

[R11] case 多分支
来源：http://nd.panjiajie.cn

case "$1" in
来源：http://jk.colortex.cn

start) echo "启动" ;;
来源：http://nb.nicolike.cn

stop)  echo "停止" ;;
来源：http://wd.9csxet.cn

*)     echo "未知命令" ;;
来源：http://df.nszjky.cn

esac
来源：http://fl.nicolike.cn

[R12] for 遍历文件
来源：http://vn.szxytkj.cn

for f in *.txt; do echo "$f"; done
来源：http://bq.panjiajie.cn

[R13] for 计数循环
来源：http://kl.hahajie.cn

for i in {1..10}; do echo "$i"; done
来源：http://zs.szsharing.cn

[R14] C 风格 for
来源：http://de.szsharing.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://cb.hahajie.cn

[R15] while 逐行读文件
来源：http://as.asd995.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mr.huixinmuqiang.cn

[R16] until 等待条件
来源：http://hk.9csxet.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://va.huixiangedu.cn

[R17] 数组定义与取值
来源：http://ws.panjiajie.cn

arr=(a b c); echo "${arr[0]}"
来源：http://ju.hahajie.cn

[R18] 遍历数组
来源：http://nc.haigaiapp.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://oc.521024.cn

[R19] 数组长度
来源：http://dt.yuexingan06.cn

echo "${#arr[@]}"
来源：http://gu.nszjky.cn

[R20] 关联数组（字典）
来源：http://am.asd995.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://cs.hahajie.cn

[R21] 字符串长度
来源：http://fy.chemitech.net.cn

echo "${#s}"
来源：http://py.huixiangedu.cn

[R22] 截取子串
来源：http://vi.shtwfgs.cn

echo "${s:0:5}"
来源：http://pi.nicolike.cn

[R23] 字符串替换
来源：http://gh.szsharing.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ri.colortex.cn

[R24] 大小写转换
来源：http://vr.huixinmuqiang.cn

echo "${s^^}"; echo "${s,,}"
来源：http://bo.yuntaijiaju.cn

[R25] 去后缀 / 去前缀
来源：http://fd.bookmarksfly.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://at.szsharing.cn

[R26] 命令替换
来源：http://lh.szxytkj.cn

now=$(date +%F); echo "$now"
来源：http://cz.haigaiapp.cn

[R27] 算术展开
来源：http://nn.huixiangedu.cn

echo $((1 + 2 * 3))
来源：http://ma.yuntaijiaju.cn

[R28] 浮点运算
来源：http://mx.shxzukj.cn

echo "scale=2; 10/3" | bc
来源：http://ne.asd995.cn

[R29] 定义函数
来源：http://nr.nszjky.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mc.gzmigu.cn

[R30] 函数返回状态码
来源：http://wb.szsharing.cn

f() { return 0; }; f || echo "失败了"
来源：http://fd.yuexingan06.cn

[R31] 局部变量
来源：http://gb.nicolike.cn

f() { local x=1; echo "$x"; }
来源：http://bi.nicolike.cn

[R32] 参数个数校验
来源：http://xy.hahajie.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://vu.gzmigu.cn

[R33] 捕获错误并提示行号
来源：http://yy.yuexingan06.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://tz.haigaiapp.cn

[R34] 退出时清理
来源：http://zy.9csxet.cn

trap 'rm -f "$tmp"' EXIT
来源：http://ua.nicolike.cn

[R35] 后台执行并等待
来源：http://vp.newstarts.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://co.nszjky.cn

[R36] 并发执行多个任务
来源：http://fx.szsharing.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://xs.haigaiapp.cn

[R37] 把输出赋给变量
来源：http://qp.yuntaijiaju.cn

files=$(ls -1)
来源：http://vi.shtwfgs.cn

[R38] 管道串联
来源：http://ji.bjjhwx.cn

cat a.txt | grep -i error | wc -l
来源：http://po.bookmarksfly.cn

[R39] 重定向标准输出与错误
来源：http://sm.lnxyls.cn

cmd > out.log 2>&1
来源：http://up.hnjuh.cn

[R40] 追加写日志
来源：http://wc.shxzukj.cn

echo "log" >> out.log
来源：http://ca.panjiajie.cn

[R41] 丢弃输出
来源：http://ul.shxzukj.cn

cmd >/dev/null 2>&1
来源：http://gs.newstarts.cn

[R42] 输入重定向
来源：http://pq.shtwfgs.cn

wc -l < a.txt
来源：http://hc.nszjky.cn

[R43] 按名字查找文件
来源：http://fh.gzmigu.cn

find . -name "*.log" -type f
来源：http://jp.nicolike.cn

[R44] 按修改时间查找
来源：http://hj.gzmigu.cn

find . -mtime -7 -type f
来源：http://zm.newstarts.cn

[R45] 批量删除
来源：http://vu.haigaiapp.cn

find . -name "*.tmp" -delete
来源：http://bk.9csxet.cn

[R46] 递归替换文件内容
来源：http://uk.asd995.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://gi.newstarts.cn

[R47] sed 单行替换
来源：http://dk.huixinmuqiang.cn

sed -i 's/foo/bar/g' a.txt
来源：http://kn.colortex.cn

[R48] awk 取指定列
来源：http://to.gzmigu.cn

awk '{print $1, $3}' a.txt
来源：http://jn.nszjky.cn

[R49] awk 带条件
来源：http://cq.shxzukj.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://nu.huixinmuqiang.cn

[R50] awk 求和
来源：http://fc.nszjky.cn

awk '{s += $2} END {print s}' a.txt
来源：http://ww.nszjky.cn

[R51] 排序去重取前几
来源：http://dv.9csxet.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://xc.nicolike.cn

[R52] 统计行数
来源：http://gb.colortex.cn

wc -l a.txt
来源：http://zo.bookmarksfly.cn

[R53] 查看文件头与实时尾
来源：http://nb.newstarts.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://yg.nszjky.cn

[R54] 比较两个文件
来源：http://af.nicolike.cn

diff a.txt b.txt
来源：http://ig.szsharing.cn

[R55] 压缩与解压
来源：http://ii.jctech888.com.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ym.yuntaijiaju.cn

[R56] 远程拷贝
来源：http://dw.huixiangedu.cn

scp file user@host:/path/
来源：http://mj.huixiangedu.cn

[R57] 远程执行命令
来源：http://tp.huixinmuqiang.cn

ssh user@host 'uptime'
来源：http://qn.wgjwhj.cn

[R58] 下载文件
来源：http://gy.asd995.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wq.muxihuayi.cn

[R59] 发 POST JSON
来源：http://yr.nicolike.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ni.9csxet.cn

[R60] 只看 HTTP 状态码
来源：http://bu.bookmarksfly.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://zt.nszjky.cn

[R61] 磁盘占用
来源：http://ll.shxzukj.cn


<!-- 参考信息 -->