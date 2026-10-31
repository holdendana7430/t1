代发 wailian999

[Q14] 存在则更新（upsert）
来源：http://rf.asd995.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://oh.bjjhwx.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://yj.shxzskj.cn

[Q15] 查询全部
来源：http://oy.jianghongdianzi.cn

SELECT * FROM users;
来源：http://wp.haigaiapp.cn

[Q16] 查询指定列
来源：http://ry.hnjuh.cn

SELECT id, name FROM users;
来源：http://uh.shxzskj.cn

[Q17] 条件查询
来源：http://ov.szxytkj.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://aw.colortex.cn

[Q18] 模糊匹配
来源：http://ew.jianghongdianzi.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://qh.bjjhwx.cn

[Q19] 范围查询
来源：http://rp.huanxung.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://vy.lnxyls.cn

[Q20] IN 列表
来源：http://cn.colortex.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://qm.szxytkj.cn

[Q21] 空值判断
来源：http://wn.521024.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://tm.colortex.cn

[Q22] 排序
来源：http://bl.szsharing.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://kk.szxytkj.cn

[Q23] 分页
来源：http://ur.9csxet.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ar.yuexingan06.cn

[Q24] 去重
来源：http://cy.huixinmuqiang.cn

SELECT DISTINCT city FROM users;
来源：http://ux.huixinmuqiang.cn

[Q25] 只取前 N 条
来源：http://cj.hnjuh.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://bc.shxzskj.cn

[Q26] 计数
来源：http://do.nszjky.cn

SELECT COUNT(*) FROM users;
来源：http://nm.newstarts.cn

[Q27] 条件计数
来源：http://id.nszjky.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ci.asd995.cn

[Q28] 求和与平均
来源：http://xh.hahajie.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hi.colortex.cn

[Q29] 最大最小值
来源：http://xh.yuexingan06.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://uu.shxzukj.cn

[Q30] 分组统计
来源：http://oi.shtwfgs.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://qw.haigaiapp.cn

[Q31] 分组后过滤
来源：http://vu.lnxyls.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://uh.szxytkj.cn

[Q32] 分组拼接字符串
来源：http://df.shxzukj.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://tf.jctech888.com.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ed.hahajie.cn

[Q33] 多列分组
来源：http://yo.jctech888.com.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ix.yuexingan06.cn

[Q34] 每组取第一条
来源：http://vb.bookmarksfly.cn

SELECT * FROM (
来源：http://ev.bookmarksfly.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mb.jianghongdianzi.cn

) t WHERE rn = 1;
来源：http://au.haigaiapp.cn

[Q35] 内连接
来源：http://uc.huixinmuqiang.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://du.lnxyls.cn

[Q36] 左连接
来源：http://ay.colortex.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://yt.huixiangedu.cn

[Q37] 右连接
来源：http://sz.muxihuayi.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ck.bjjhwx.cn

[Q38] 全外连接（PostgreSQL）
来源：http://uf.9csxet.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ji.yuexingan06.cn

[Q39] 自连接（查上下级）
来源：http://my.chemitech.net.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://ds.jianghongdianzi.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wg.haigaiapp.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://qd.yuntaijiaju.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://pe.yuexingan06.cn

[Q41] 多表连接
来源：http://fz.hahajie.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://ci.bjjhwx.cn

JOIN users u ON u.id = o.user_id
来源：http://to.newstarts.cn

JOIN products p ON p.id = o.product_id;
来源：http://gx.huanxung.cn

[Q42] 连接条件附加过滤
来源：http://uv.yuntaijiaju.cn

SELECT u.name, o.amount FROM users u
来源：http://ca.bookmarksfly.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://rc.yuntaijiaju.cn

[Q43] 标量子查询
来源：http://nt.wgjwhj.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://co.szxytkj.cn

[Q44] IN 子查询
来源：http://vc.521024.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ew.muxihuayi.cn

[Q45] EXISTS 判断存在
来源：http://sa.hnjuh.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://vo.yuntaijiaju.cn

[Q46] NOT EXISTS 判断不存在
来源：http://tl.hahajie.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://xb.9csxet.cn

[Q47] 与平均值比较
来源：http://ap.huixinmuqiang.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://gg.yuexingan06.cn

[Q48] CTE 公用表表达式
来源：http://cj.haigaiapp.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://pc.9csxet.cn

SELECT * FROM t WHERE c > 5;
来源：http://ki.shtwfgs.cn

[Q49] 更新单行
来源：http://kt.9csxet.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hl.huixinmuqiang.cn

[Q50] 批量更新
来源：http://at.9csxet.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://ox.shxzukj.cn

[Q51] 用子查询更新
来源：http://mo.colortex.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://jy.asd995.cn

[Q52] 删除指定行
来源：http://xu.shxzskj.cn

DELETE FROM users WHERE id = 10;
来源：http://qb.521024.cn

[Q53] 按条件删除
来源：http://tg.hnjuh.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://xv.haigaiapp.cn

[Q54] 清空表
来源：http://ct.panjiajie.cn

TRUNCATE TABLE logs;
来源：http://kc.shtwfgs.cn

[Q55] 排名（并列占位）
来源：http://ny.nszjky.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://nq.yuntaijiaju.cn

[Q56] 密集排名（并列不占位）
来源：http://wy.hnjuh.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://yh.newstarts.cn

[Q57] 行号
来源：http://tb.haigaiapp.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://sg.haigaiapp.cn

[Q58] 累计求和
来源：http://az.szsharing.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ts.shxzskj.cn

[Q59] 分组内累计
来源：http://ya.bjjhwx.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://vk.yuexingan06.cn

[Q60] 取上一行 / 下一行
来源：http://rj.asd995.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ic.szxytkj.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ky.shxzukj.cn

[Q61] 移动平均
来源：http://iq.wgjwhj.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://jc.gzmigu.cn

[Q62] 分组占比
来源：http://bo.huixiangedu.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://bn.nszjky.cn

[Q63] 开启事务
来源：http://dp.nszjky.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://io.newstarts.cn

[Q64] 提交事务
来源：http://an.bjjhwx.cn

COMMIT;
来源：http://wo.9csxet.cn

[Q65] 回滚事务
来源：http://yp.szxytkj.cn

ROLLBACK;
来源：http://bu.chemitech.net.cn

[Q66] 行锁查询
来源：http://kk.521024.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://du.521024.cn

[Q67] 设置隔离级别
来源：http://si.yuntaijiaju.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://pj.chemitech.net.cn

[Q68] 保存点
来源：http://pd.lnxyls.cn

SAVEPOINT sp1;
来源：http://uf.newstarts.cn

ROLLBACK TO sp1;
来源：http://qf.nicolike.cn

[Q69] 查看执行计划
来源：http://ns.yuntaijiaju.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://jo.asd995.cn

[Q70] 更新统计信息
来源：http://qz.hnjuh.cn

ANALYZE TABLE users;
来源：http://vd.jctech888.com.cn

[Q71] 查看建表语句
来源：http://yg.nicolike.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://kd.newstarts.cn

[Q72] 查看索引
来源：http://nc.muxihuayi.cn

SHOW INDEX FROM users;
来源：http://pw.colortex.cn

[Q73] 查看表状态
来源：http://pn.jianghongdianzi.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://tc.szxytkj.cn

[Q74] 强制使用索引
来源：http://pk.yuexingan06.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ik.wgjwhj.cn

[Q75] 日期格式化
来源：http://gv.9csxet.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://cy.yuntaijiaju.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://me.bjjhwx.cn

[Q76] 按天统计
来源：http://xn.bookmarksfly.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://jp.huanxung.cn

[Q77] 时间加减
来源：http://hz.shxzskj.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://yt.jctech888.com.cn

[Q78] 当前时间
来源：http://gc.lnxyls.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://jf.9csxet.cn

[Q79] 字符串拼接
来源：http://al.hnjuh.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hb.wgjwhj.cn

[Q80] 字符串截取
来源：http://va.nicolike.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ee.muxihuayi.cn

[Q81] 字符串替换
来源：http://rv.jianghongdianzi.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://tw.9csxet.cn

[Q82] 字符长度与字节长度
来源：http://fu.szxytkj.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://eq.chemitech.net.cn

[Q83] 大小写转换
来源：http://td.521024.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://kl.chemitech.net.cn

[Q84] 去除首尾空格
来源：http://za.huanxung.cn

SELECT TRIM(name) FROM users;
来源：http://cw.9csxet.cn

[Q85] 数值取整
来源：http://tc.huixinmuqiang.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://al.shtwfgs.cn

[Q86] 读取 JSON 字段
来源：http://gd.hahajie.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://uo.jianghongdianzi.cn

[Q87] JSON 字段做条件
来源：http://er.muxihuayi.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://fh.jianghongdianzi.cn

[Q88] 行转列（条件聚合）
来源：http://ff.huixiangedu.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ld.jianghongdianzi.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://dh.haigaiapp.cn

[Q89] 判断表是否存在
来源：http://tp.panjiajie.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://tu.huixinmuqiang.cn

[Q90] 生成序号列
来源：http://gk.huixiangedu.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://bl.nszjky.cn

================================================================================
来源：http://qv.colortex.cn

R. Bash 专题
来源：http://hq.9csxet.cn

================================================================================
来源：http://pv.szxytkj.cn

[R01] shebang 与严格模式
来源：http://kw.szxytkj.cn

#!/usr/bin/env bash
来源：http://qi.huixiangedu.cn

set -euo pipefail
来源：http://fg.shxzukj.cn

[R02] 变量赋值与使用
来源：http://fj.9csxet.cn

name="Tom"; echo "$name"
来源：http://kj.szxytkj.cn

[R03] 只读变量
来源：http://pt.lnxyls.cn

readonly PI=3.14
来源：http://ld.huixinmuqiang.cn

[R04] 位置参数
来源：http://dx.muxihuayi.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://az.wgjwhj.cn

[R05] 参数默认值
来源：http://nu.hahajie.cn

name="${1:-default}"
来源：http://bq.gzmigu.cn

[R06] 判断命令是否存在
来源：http://id.chemitech.net.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://yl.shxzukj.cn

[R07] if 判断文件
来源：http://fx.gzmigu.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://yq.newstarts.cn

[R08] 数值比较
来源：http://gv.newstarts.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://ky.nszjky.cn

[R09] 字符串比较
来源：http://rn.shxzskj.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ic.521024.cn

[R10] 正则匹配
来源：http://pw.bookmarksfly.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ua.asd995.cn

[R11] case 多分支
来源：http://ie.asd995.cn

case "$1" in
来源：http://wg.szxytkj.cn

start) echo "启动" ;;
来源：http://yb.huixinmuqiang.cn

stop)  echo "停止" ;;
来源：http://sk.nicolike.cn

*)     echo "未知命令" ;;
来源：http://iw.jctech888.com.cn

esac
来源：http://vj.yuexingan06.cn

[R12] for 遍历文件
来源：http://le.szsharing.cn

for f in *.txt; do echo "$f"; done
来源：http://ic.nszjky.cn

[R13] for 计数循环
来源：http://lg.shtwfgs.cn

for i in {1..10}; do echo "$i"; done
来源：http://zm.jianghongdianzi.cn

[R14] C 风格 for
来源：http://pf.szxytkj.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://jf.hnjuh.cn

[R15] while 逐行读文件
来源：http://ay.yuntaijiaju.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ig.szsharing.cn

[R16] until 等待条件
来源：http://up.asd995.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://pe.chemitech.net.cn

[R17] 数组定义与取值
来源：http://vv.jianghongdianzi.cn

arr=(a b c); echo "${arr[0]}"
来源：http://cb.szxytkj.cn

[R18] 遍历数组
来源：http://lj.9csxet.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ut.huanxung.cn

[R19] 数组长度
来源：http://rk.szxytkj.cn

echo "${#arr[@]}"
来源：http://ze.hahajie.cn

[R20] 关联数组（字典）
来源：http://fq.jianghongdianzi.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mz.colortex.cn

[R21] 字符串长度
来源：http://wb.muxihuayi.cn

echo "${#s}"
来源：http://ku.shxzukj.cn

[R22] 截取子串
来源：http://qi.muxihuayi.cn

echo "${s:0:5}"
来源：http://ph.jianghongdianzi.cn

[R23] 字符串替换
来源：http://ll.hnjuh.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://tf.szxytkj.cn

[R24] 大小写转换
来源：http://ph.hnjuh.cn

echo "${s^^}"; echo "${s,,}"
来源：http://zj.szsharing.cn

[R25] 去后缀 / 去前缀
来源：http://oh.521024.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://gr.wgjwhj.cn

[R26] 命令替换
来源：http://ao.szxytkj.cn

now=$(date +%F); echo "$now"
来源：http://cr.wgjwhj.cn

[R27] 算术展开
来源：http://xy.521024.cn

echo $((1 + 2 * 3))
来源：http://gy.hahajie.cn

[R28] 浮点运算
来源：http://sh.yuntaijiaju.cn

echo "scale=2; 10/3" | bc
来源：http://mj.yuexingan06.cn

[R29] 定义函数
来源：http://zt.huanxung.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://gp.gzmigu.cn

[R30] 函数返回状态码
来源：http://mi.szxytkj.cn

f() { return 0; }; f || echo "失败了"
来源：http://no.hahajie.cn

[R31] 局部变量
来源：http://qc.lnxyls.cn

f() { local x=1; echo "$x"; }
来源：http://oc.szsharing.cn

[R32] 参数个数校验
来源：http://kc.shtwfgs.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hl.nicolike.cn

[R33] 捕获错误并提示行号
来源：http://vw.yuexingan06.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ht.yuntaijiaju.cn

[R34] 退出时清理
来源：http://fc.colortex.cn

trap 'rm -f "$tmp"' EXIT
来源：http://uu.szxytkj.cn

[R35] 后台执行并等待
来源：http://au.huixiangedu.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://vs.9csxet.cn

[R36] 并发执行多个任务
来源：http://sn.shxzukj.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://jk.hnjuh.cn

[R37] 把输出赋给变量
来源：http://wq.panjiajie.cn

files=$(ls -1)
来源：http://vr.9csxet.cn

[R38] 管道串联
来源：http://ix.yuntaijiaju.cn

cat a.txt | grep -i error | wc -l
来源：http://dy.szsharing.cn

[R39] 重定向标准输出与错误
来源：http://wh.huixinmuqiang.cn

cmd > out.log 2>&1
来源：http://ys.newstarts.cn

[R40] 追加写日志
来源：http://rt.wgjwhj.cn

echo "log" >> out.log
来源：http://yw.huixiangedu.cn

[R41] 丢弃输出
来源：http://xk.szxytkj.cn

cmd >/dev/null 2>&1
来源：http://no.yuntaijiaju.cn

[R42] 输入重定向
来源：http://lv.bookmarksfly.cn

wc -l < a.txt
来源：http://io.newstarts.cn

[R43] 按名字查找文件
来源：http://xz.hahajie.cn

find . -name "*.log" -type f
来源：http://rp.yuntaijiaju.cn

[R44] 按修改时间查找
来源：http://ep.yuexingan06.cn

find . -mtime -7 -type f
来源：http://no.nszjky.cn

[R45] 批量删除
来源：http://zr.nicolike.cn

find . -name "*.tmp" -delete
来源：http://ut.hnjuh.cn

[R46] 递归替换文件内容
来源：http://it.muxihuayi.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://zt.szxytkj.cn

[R47] sed 单行替换
来源：http://xl.panjiajie.cn

sed -i 's/foo/bar/g' a.txt
来源：http://jc.lnxyls.cn

[R48] awk 取指定列
来源：http://uh.wgjwhj.cn

awk '{print $1, $3}' a.txt
来源：http://ak.hnjuh.cn

[R49] awk 带条件
来源：http://xf.panjiajie.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ni.haigaiapp.cn

[R50] awk 求和
来源：http://cs.szxytkj.cn

awk '{s += $2} END {print s}' a.txt
来源：http://go.colortex.cn

[R51] 排序去重取前几
来源：http://mv.wgjwhj.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://yo.asd995.cn

[R52] 统计行数
来源：http://xm.newstarts.cn

wc -l a.txt
来源：http://su.bjjhwx.cn

[R53] 查看文件头与实时尾
来源：http://hm.szxytkj.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://cn.muxihuayi.cn

[R54] 比较两个文件
来源：http://dr.colortex.cn

diff a.txt b.txt
来源：http://go.yuntaijiaju.cn

[R55] 压缩与解压
来源：http://tf.bookmarksfly.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://sf.huanxung.cn

[R56] 远程拷贝
来源：http://jc.9csxet.cn

scp file user@host:/path/
来源：http://rt.huixiangedu.cn

[R57] 远程执行命令
来源：http://bt.yuexingan06.cn

ssh user@host 'uptime'
来源：http://en.muxihuayi.cn

[R58] 下载文件
来源：http://kv.panjiajie.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.hahajie.cn

[R59] 发 POST JSON
来源：http://lt.521024.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://je.huixiangedu.cn

[R60] 只看 HTTP 状态码
来源：http://hu.9csxet.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://nv.newstarts.cn

[R61] 磁盘占用
来源：http://aw.yuexingan06.cn

df -h;  du -sh *
来源：http://mu.huanxung.cn

[R62] 找最占空间的文件
来源：http://ri.newstarts.cn

du -ah . | sort -rh | head -10
来源：http://gq.shxzukj.cn

[R63] 内存与进程
来源：http://fd.jianghongdianzi.cn


<!-- 参考信息 -->