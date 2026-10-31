代发 wailian999

[Q14] 存在则更新（upsert）
来源：http://mu.nszjky.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://gx.shtwfgs.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mi.jctech888.com.cn

[Q15] 查询全部
来源：http://hx.nszjky.cn

SELECT * FROM users;
来源：http://nz.newstarts.cn

[Q16] 查询指定列
来源：http://rc.jianghongdianzi.cn

SELECT id, name FROM users;
来源：http://aw.9csxet.cn

[Q17] 条件查询
来源：http://bt.jianghongdianzi.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://de.muxihuayi.cn

[Q18] 模糊匹配
来源：http://io.shxzskj.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://fk.hnjuh.cn

[Q19] 范围查询
来源：http://ha.jianghongdianzi.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://iv.asd995.cn

[Q20] IN 列表
来源：http://qc.shxzskj.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://zh.wgjwhj.cn

[Q21] 空值判断
来源：http://gm.gzmigu.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://bm.colortex.cn

[Q22] 排序
来源：http://dm.asd995.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://fe.asd995.cn

[Q23] 分页
来源：http://al.nicolike.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://dq.huixinmuqiang.cn

[Q24] 去重
来源：http://as.hnjuh.cn

SELECT DISTINCT city FROM users;
来源：http://gz.nicolike.cn

[Q25] 只取前 N 条
来源：http://je.lnxyls.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ji.jianghongdianzi.cn

[Q26] 计数
来源：http://bp.panjiajie.cn

SELECT COUNT(*) FROM users;
来源：http://fu.colortex.cn

[Q27] 条件计数
来源：http://vy.haigaiapp.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://kk.huixinmuqiang.cn

[Q28] 求和与平均
来源：http://ag.gzmigu.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://vq.hnjuh.cn

[Q29] 最大最小值
来源：http://lu.panjiajie.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://gj.asd995.cn

[Q30] 分组统计
来源：http://ij.yuntaijiaju.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hc.newstarts.cn

[Q31] 分组后过滤
来源：http://ut.gzmigu.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://xh.asd995.cn

[Q32] 分组拼接字符串
来源：http://yw.wgjwhj.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://iq.colortex.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ik.9csxet.cn

[Q33] 多列分组
来源：http://be.yuntaijiaju.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://bm.gzmigu.cn

[Q34] 每组取第一条
来源：http://fa.jctech888.com.cn

SELECT * FROM (
来源：http://ek.szxytkj.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://qr.panjiajie.cn

) t WHERE rn = 1;
来源：http://lj.colortex.cn

[Q35] 内连接
来源：http://le.nszjky.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://cp.nicolike.cn

[Q36] 左连接
来源：http://ho.jctech888.com.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://xr.muxihuayi.cn

[Q37] 右连接
来源：http://at.yuntaijiaju.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ts.wgjwhj.cn

[Q38] 全外连接（PostgreSQL）
来源：http://xx.yuntaijiaju.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://gl.shtwfgs.cn

[Q39] 自连接（查上下级）
来源：http://gz.521024.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://qd.asd995.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://uk.jianghongdianzi.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://gm.bjjhwx.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://xi.9csxet.cn

[Q41] 多表连接
来源：http://pf.nszjky.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://mo.chemitech.net.cn

JOIN users u ON u.id = o.user_id
来源：http://ze.yuexingan06.cn

JOIN products p ON p.id = o.product_id;
来源：http://ck.szxytkj.cn

[Q42] 连接条件附加过滤
来源：http://ea.yuexingan06.cn

SELECT u.name, o.amount FROM users u
来源：http://tn.shxzskj.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ed.huanxung.cn

[Q43] 标量子查询
来源：http://ai.wgjwhj.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://dl.newstarts.cn

[Q44] IN 子查询
来源：http://xg.huixinmuqiang.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://gs.jctech888.com.cn

[Q45] EXISTS 判断存在
来源：http://xj.chemitech.net.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://gb.yuexingan06.cn

[Q46] NOT EXISTS 判断不存在
来源：http://rj.521024.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://yj.jianghongdianzi.cn

[Q47] 与平均值比较
来源：http://tb.newstarts.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://fv.shxzskj.cn

[Q48] CTE 公用表表达式
来源：http://xq.shxzskj.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://yw.newstarts.cn

SELECT * FROM t WHERE c > 5;
来源：http://ov.shtwfgs.cn

[Q49] 更新单行
来源：http://oz.haigaiapp.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://se.yuexingan06.cn

[Q50] 批量更新
来源：http://uv.wgjwhj.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hk.shxzskj.cn

[Q51] 用子查询更新
来源：http://tq.bjjhwx.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://qv.bookmarksfly.cn

[Q52] 删除指定行
来源：http://fz.huixinmuqiang.cn

DELETE FROM users WHERE id = 10;
来源：http://gc.gzmigu.cn

[Q53] 按条件删除
来源：http://sg.chemitech.net.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://cc.haigaiapp.cn

[Q54] 清空表
来源：http://wf.nszjky.cn

TRUNCATE TABLE logs;
来源：http://mr.asd995.cn

[Q55] 排名（并列占位）
来源：http://ep.chemitech.net.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://kb.asd995.cn

[Q56] 密集排名（并列不占位）
来源：http://br.jctech888.com.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://tf.nicolike.cn

[Q57] 行号
来源：http://rz.huixinmuqiang.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://dq.yuexingan06.cn

[Q58] 累计求和
来源：http://kn.asd995.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hf.9csxet.cn

[Q59] 分组内累计
来源：http://xu.szsharing.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://tg.wgjwhj.cn

[Q60] 取上一行 / 下一行
来源：http://pt.bjjhwx.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://df.bookmarksfly.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://gh.yuexingan06.cn

[Q61] 移动平均
来源：http://ur.huixinmuqiang.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://kq.nicolike.cn

[Q62] 分组占比
来源：http://nz.gzmigu.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://tb.yuexingan06.cn

[Q63] 开启事务
来源：http://hj.yuexingan06.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://tr.bjjhwx.cn

[Q64] 提交事务
来源：http://hr.lnxyls.cn

COMMIT;
来源：http://qc.muxihuayi.cn

[Q65] 回滚事务
来源：http://rn.hnjuh.cn

ROLLBACK;
来源：http://ix.521024.cn

[Q66] 行锁查询
来源：http://py.szsharing.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wh.hnjuh.cn

[Q67] 设置隔离级别
来源：http://im.haigaiapp.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://pw.nszjky.cn

[Q68] 保存点
来源：http://jq.shxzskj.cn

SAVEPOINT sp1;
来源：http://fw.9csxet.cn

ROLLBACK TO sp1;
来源：http://tp.9csxet.cn

[Q69] 查看执行计划
来源：http://yw.hahajie.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ti.chemitech.net.cn

[Q70] 更新统计信息
来源：http://yw.szsharing.cn

ANALYZE TABLE users;
来源：http://qf.asd995.cn

[Q71] 查看建表语句
来源：http://ry.shtwfgs.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mu.shxzskj.cn

[Q72] 查看索引
来源：http://mi.nszjky.cn

SHOW INDEX FROM users;
来源：http://ki.yuntaijiaju.cn

[Q73] 查看表状态
来源：http://bs.chemitech.net.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://ng.nicolike.cn

[Q74] 强制使用索引
来源：http://ec.panjiajie.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wu.shxzskj.cn

[Q75] 日期格式化
来源：http://ne.haigaiapp.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ye.lnxyls.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://we.521024.cn

[Q76] 按天统计
来源：http://gq.hnjuh.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://tz.nicolike.cn

[Q77] 时间加减
来源：http://sw.521024.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hq.huixinmuqiang.cn

[Q78] 当前时间
来源：http://vd.gzmigu.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ue.chemitech.net.cn

[Q79] 字符串拼接
来源：http://gt.huanxung.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://uw.shxzukj.cn

[Q80] 字符串截取
来源：http://wa.521024.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://kg.chemitech.net.cn

[Q81] 字符串替换
来源：http://zm.nicolike.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://jx.jctech888.com.cn

[Q82] 字符长度与字节长度
来源：http://ta.gzmigu.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://yl.huixiangedu.cn

[Q83] 大小写转换
来源：http://bf.muxihuayi.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://bx.colortex.cn

[Q84] 去除首尾空格
来源：http://sb.newstarts.cn

SELECT TRIM(name) FROM users;
来源：http://ng.hahajie.cn

[Q85] 数值取整
来源：http://xz.nszjky.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ow.bjjhwx.cn

[Q86] 读取 JSON 字段
来源：http://oy.szsharing.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://zt.hnjuh.cn

[Q87] JSON 字段做条件
来源：http://oa.lnxyls.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://us.bookmarksfly.cn

[Q88] 行转列（条件聚合）
来源：http://oq.nicolike.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hc.hnjuh.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://dt.hnjuh.cn

[Q89] 判断表是否存在
来源：http://yw.hnjuh.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://kr.shxzukj.cn

[Q90] 生成序号列
来源：http://ry.muxihuayi.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://js.huixinmuqiang.cn

================================================================================
来源：http://yx.nicolike.cn

R. Bash 专题
来源：http://gr.lnxyls.cn

================================================================================
来源：http://ey.hnjuh.cn

[R01] shebang 与严格模式
来源：http://ok.jctech888.com.cn

#!/usr/bin/env bash
来源：http://yw.jctech888.com.cn

set -euo pipefail
来源：http://gh.haigaiapp.cn

[R02] 变量赋值与使用
来源：http://ub.nszjky.cn

name="Tom"; echo "$name"
来源：http://en.hnjuh.cn

[R03] 只读变量
来源：http://sz.colortex.cn

readonly PI=3.14
来源：http://eo.jctech888.com.cn

[R04] 位置参数
来源：http://jt.shxzskj.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://rl.bookmarksfly.cn

[R05] 参数默认值
来源：http://zj.huanxung.cn

name="${1:-default}"
来源：http://yy.hahajie.cn

[R06] 判断命令是否存在
来源：http://lz.shxzukj.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hh.lnxyls.cn

[R07] if 判断文件
来源：http://sr.shtwfgs.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ux.huixiangedu.cn

[R08] 数值比较
来源：http://fs.szsharing.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://kc.lnxyls.cn

[R09] 字符串比较
来源：http://cq.shxzukj.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ox.521024.cn

[R10] 正则匹配
来源：http://qg.nszjky.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://fj.szxytkj.cn

[R11] case 多分支
来源：http://bm.asd995.cn

case "$1" in
来源：http://ai.yuexingan06.cn

start) echo "启动" ;;
来源：http://pl.wgjwhj.cn

stop)  echo "停止" ;;
来源：http://lm.shxzskj.cn

*)     echo "未知命令" ;;
来源：http://in.shxzskj.cn

esac
来源：http://tm.szxytkj.cn

[R12] for 遍历文件
来源：http://kq.colortex.cn

for f in *.txt; do echo "$f"; done
来源：http://jw.newstarts.cn

[R13] for 计数循环
来源：http://wg.szsharing.cn

for i in {1..10}; do echo "$i"; done
来源：http://ht.newstarts.cn

[R14] C 风格 for
来源：http://ga.colortex.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mz.asd995.cn

[R15] while 逐行读文件
来源：http://nr.lnxyls.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ap.asd995.cn

[R16] until 等待条件
来源：http://hb.521024.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://si.chemitech.net.cn

[R17] 数组定义与取值
来源：http://to.huanxung.cn

arr=(a b c); echo "${arr[0]}"
来源：http://gz.huixiangedu.cn

[R18] 遍历数组
来源：http://gc.huixinmuqiang.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://vu.shxzukj.cn

[R19] 数组长度
来源：http://uk.szsharing.cn

echo "${#arr[@]}"
来源：http://ig.bookmarksfly.cn

[R20] 关联数组（字典）
来源：http://rz.yuntaijiaju.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mi.muxihuayi.cn

[R21] 字符串长度
来源：http://dh.nicolike.cn

echo "${#s}"
来源：http://je.bjjhwx.cn

[R22] 截取子串
来源：http://di.gzmigu.cn

echo "${s:0:5}"
来源：http://jx.panjiajie.cn

[R23] 字符串替换
来源：http://li.bjjhwx.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://xg.szxytkj.cn

[R24] 大小写转换
来源：http://cf.bookmarksfly.cn

echo "${s^^}"; echo "${s,,}"
来源：http://xq.newstarts.cn

[R25] 去后缀 / 去前缀
来源：http://yq.521024.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://rs.9csxet.cn

[R26] 命令替换
来源：http://yi.bookmarksfly.cn

now=$(date +%F); echo "$now"
来源：http://gw.huanxung.cn

[R27] 算术展开
来源：http://ze.asd995.cn

echo $((1 + 2 * 3))
来源：http://mw.muxihuayi.cn

[R28] 浮点运算
来源：http://hx.colortex.cn

echo "scale=2; 10/3" | bc
来源：http://nc.colortex.cn

[R29] 定义函数
来源：http://ki.nicolike.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://yj.newstarts.cn

[R30] 函数返回状态码
来源：http://tk.shxzukj.cn

f() { return 0; }; f || echo "失败了"
来源：http://zy.wgjwhj.cn

[R31] 局部变量
来源：http://nl.9csxet.cn

f() { local x=1; echo "$x"; }
来源：http://gy.521024.cn

[R32] 参数个数校验
来源：http://jc.shtwfgs.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mt.hnjuh.cn

[R33] 捕获错误并提示行号
来源：http://hp.nszjky.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wv.asd995.cn

[R34] 退出时清理
来源：http://rh.shxzukj.cn

trap 'rm -f "$tmp"' EXIT
来源：http://hk.nicolike.cn

[R35] 后台执行并等待
来源：http://sr.szsharing.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://la.lnxyls.cn

[R36] 并发执行多个任务
来源：http://zy.hnjuh.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://du.bjjhwx.cn

[R37] 把输出赋给变量
来源：http://er.newstarts.cn

files=$(ls -1)
来源：http://rc.nszjky.cn

[R38] 管道串联
来源：http://un.521024.cn

cat a.txt | grep -i error | wc -l
来源：http://zy.chemitech.net.cn

[R39] 重定向标准输出与错误
来源：http://vp.bjjhwx.cn

cmd > out.log 2>&1
来源：http://re.chemitech.net.cn

[R40] 追加写日志
来源：http://sa.huixinmuqiang.cn

echo "log" >> out.log
来源：http://mt.hahajie.cn

[R41] 丢弃输出
来源：http://oz.chemitech.net.cn

cmd >/dev/null 2>&1
来源：http://ot.szsharing.cn

[R42] 输入重定向
来源：http://kf.szsharing.cn

wc -l < a.txt
来源：http://qa.newstarts.cn

[R43] 按名字查找文件
来源：http://hq.hahajie.cn

find . -name "*.log" -type f
来源：http://nh.colortex.cn

[R44] 按修改时间查找
来源：http://xn.nicolike.cn

find . -mtime -7 -type f
来源：http://pk.wgjwhj.cn

[R45] 批量删除
来源：http://ew.asd995.cn

find . -name "*.tmp" -delete
来源：http://nc.szxytkj.cn

[R46] 递归替换文件内容
来源：http://mk.jianghongdianzi.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://we.yuntaijiaju.cn

[R47] sed 单行替换
来源：http://si.jctech888.com.cn

sed -i 's/foo/bar/g' a.txt
来源：http://md.huixinmuqiang.cn

[R48] awk 取指定列
来源：http://ii.lnxyls.cn

awk '{print $1, $3}' a.txt
来源：http://pr.huixinmuqiang.cn

[R49] awk 带条件
来源：http://gn.chemitech.net.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://nc.nicolike.cn

[R50] awk 求和
来源：http://fd.muxihuayi.cn

awk '{s += $2} END {print s}' a.txt
来源：http://yj.shxzukj.cn

[R51] 排序去重取前几
来源：http://sr.newstarts.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://go.huanxung.cn

[R52] 统计行数
来源：http://ps.szxytkj.cn

wc -l a.txt
来源：http://dt.asd995.cn

[R53] 查看文件头与实时尾
来源：http://vf.bookmarksfly.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://fc.gzmigu.cn

[R54] 比较两个文件
来源：http://xa.hnjuh.cn

diff a.txt b.txt
来源：http://vl.haigaiapp.cn

[R55] 压缩与解压
来源：http://ix.chemitech.net.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ds.lnxyls.cn

[R56] 远程拷贝
来源：http://er.nszjky.cn

scp file user@host:/path/
来源：http://iq.nszjky.cn

[R57] 远程执行命令
来源：http://cj.nicolike.cn

ssh user@host 'uptime'
来源：http://xx.521024.cn

[R58] 下载文件
来源：http://ur.shxzskj.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ve.huixiangedu.cn

[R59] 发 POST JSON
来源：http://fc.shtwfgs.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://lo.szsharing.cn

[R60] 只看 HTTP 状态码
来源：http://mq.colortex.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://qj.lnxyls.cn

[R61] 磁盘占用
来源：http://eh.521024.cn

df -h;  du -sh *
来源：http://sh.newstarts.cn

[R62] 找最占空间的文件
来源：http://py.nszjky.cn

du -ah . | sort -rh | head -10
来源：http://wp.muxihuayi.cn

[R63] 内存与进程
来源：http://ia.huixinmuqiang.cn


<!-- 参考信息 -->