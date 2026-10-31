代发 wailian999

INSERT INTO users (name) VALUES ('C');
来源：http://jh.haigaiapp.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ae.shxzskj.cn

[Q13] 忽略重复插入
来源：http://jv.muxihuayi.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://no.shxzskj.cn

[Q14] 存在则更新（upsert）
来源：http://va.9csxet.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://dy.shxzukj.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://fw.colortex.cn

[Q15] 查询全部
来源：http://rx.chemitech.net.cn

SELECT * FROM users;
来源：http://of.huanxung.cn

[Q16] 查询指定列
来源：http://aa.haigaiapp.cn

SELECT id, name FROM users;
来源：http://cv.bjjhwx.cn

[Q17] 条件查询
来源：http://ys.nszjky.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://dr.shtwfgs.cn

[Q18] 模糊匹配
来源：http://rb.lnxyls.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wv.shtwfgs.cn

[Q19] 范围查询
来源：http://fa.bookmarksfly.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://vd.newstarts.cn

[Q20] IN 列表
来源：http://vx.szsharing.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://dm.lnxyls.cn

[Q21] 空值判断
来源：http://av.hahajie.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://qn.panjiajie.cn

[Q22] 排序
来源：http://nn.muxihuayi.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://fn.yuntaijiaju.cn

[Q23] 分页
来源：http://nc.hahajie.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://sk.bjjhwx.cn

[Q24] 去重
来源：http://zl.yuexingan06.cn

SELECT DISTINCT city FROM users;
来源：http://id.521024.cn

[Q25] 只取前 N 条
来源：http://sz.asd995.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ay.szsharing.cn

[Q26] 计数
来源：http://td.yuexingan06.cn

SELECT COUNT(*) FROM users;
来源：http://st.shtwfgs.cn

[Q27] 条件计数
来源：http://om.szxytkj.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://gn.panjiajie.cn

[Q28] 求和与平均
来源：http://wc.haigaiapp.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://bb.huixiangedu.cn

[Q29] 最大最小值
来源：http://yr.shxzukj.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://lh.asd995.cn

[Q30] 分组统计
来源：http://wk.shxzukj.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://nz.yuntaijiaju.cn

[Q31] 分组后过滤
来源：http://xz.muxihuayi.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://vy.newstarts.cn

[Q32] 分组拼接字符串
来源：http://nb.yuntaijiaju.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wr.gzmigu.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://so.asd995.cn

[Q33] 多列分组
来源：http://mu.jctech888.com.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://fs.yuntaijiaju.cn

[Q34] 每组取第一条
来源：http://hj.wgjwhj.cn

SELECT * FROM (
来源：http://ga.jctech888.com.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://uq.szxytkj.cn

) t WHERE rn = 1;
来源：http://qp.yuexingan06.cn

[Q35] 内连接
来源：http://bc.colortex.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://rx.wgjwhj.cn

[Q36] 左连接
来源：http://rd.panjiajie.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wj.jctech888.com.cn

[Q37] 右连接
来源：http://nq.jianghongdianzi.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://dv.521024.cn

[Q38] 全外连接（PostgreSQL）
来源：http://rq.hnjuh.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mq.nicolike.cn

[Q39] 自连接（查上下级）
来源：http://cq.gzmigu.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://dc.9csxet.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ly.panjiajie.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://fo.huanxung.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://kk.521024.cn

[Q41] 多表连接
来源：http://sl.yuexingan06.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://qo.9csxet.cn

JOIN users u ON u.id = o.user_id
来源：http://bx.shxzskj.cn

JOIN products p ON p.id = o.product_id;
来源：http://do.bjjhwx.cn

[Q42] 连接条件附加过滤
来源：http://en.jianghongdianzi.cn

SELECT u.name, o.amount FROM users u
来源：http://yo.huixiangedu.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://tw.huanxung.cn

[Q43] 标量子查询
来源：http://kw.9csxet.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://kl.hnjuh.cn

[Q44] IN 子查询
来源：http://gm.huixinmuqiang.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ov.muxihuayi.cn

[Q45] EXISTS 判断存在
来源：http://qo.jctech888.com.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://gd.wgjwhj.cn

[Q46] NOT EXISTS 判断不存在
来源：http://fv.szxytkj.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ta.shtwfgs.cn

[Q47] 与平均值比较
来源：http://tp.panjiajie.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://gb.jianghongdianzi.cn

[Q48] CTE 公用表表达式
来源：http://cj.huixiangedu.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://xy.521024.cn

SELECT * FROM t WHERE c > 5;
来源：http://xe.huanxung.cn

[Q49] 更新单行
来源：http://wr.jctech888.com.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://it.9csxet.cn

[Q50] 批量更新
来源：http://om.jianghongdianzi.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://tb.colortex.cn

[Q51] 用子查询更新
来源：http://ly.shxzukj.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://zq.hnjuh.cn

[Q52] 删除指定行
来源：http://ep.asd995.cn

DELETE FROM users WHERE id = 10;
来源：http://zw.nicolike.cn

[Q53] 按条件删除
来源：http://hy.jctech888.com.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hn.asd995.cn

[Q54] 清空表
来源：http://tw.yuexingan06.cn

TRUNCATE TABLE logs;
来源：http://ll.asd995.cn

[Q55] 排名（并列占位）
来源：http://tj.huixiangedu.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ti.nicolike.cn

[Q56] 密集排名（并列不占位）
来源：http://dg.chemitech.net.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mk.nszjky.cn

[Q57] 行号
来源：http://se.muxihuayi.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ib.asd995.cn

[Q58] 累计求和
来源：http://uj.bjjhwx.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mp.jianghongdianzi.cn

[Q59] 分组内累计
来源：http://ue.nicolike.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://cl.521024.cn

[Q60] 取上一行 / 下一行
来源：http://ll.bjjhwx.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://aq.hahajie.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://gh.wgjwhj.cn

[Q61] 移动平均
来源：http://ps.wgjwhj.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://gr.yuntaijiaju.cn

[Q62] 分组占比
来源：http://so.panjiajie.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://tl.shxzskj.cn

[Q63] 开启事务
来源：http://rb.wgjwhj.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://gu.nicolike.cn

[Q64] 提交事务
来源：http://az.nszjky.cn

COMMIT;
来源：http://wr.yuexingan06.cn

[Q65] 回滚事务
来源：http://xt.shxzukj.cn

ROLLBACK;
来源：http://gk.colortex.cn

[Q66] 行锁查询
来源：http://gx.newstarts.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://au.lnxyls.cn

[Q67] 设置隔离级别
来源：http://qw.yuntaijiaju.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://pr.wgjwhj.cn

[Q68] 保存点
来源：http://en.nszjky.cn

SAVEPOINT sp1;
来源：http://ac.hahajie.cn

ROLLBACK TO sp1;
来源：http://gc.szxytkj.cn

[Q69] 查看执行计划
来源：http://hp.shtwfgs.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://di.gzmigu.cn

[Q70] 更新统计信息
来源：http://zs.shxzukj.cn

ANALYZE TABLE users;
来源：http://es.nszjky.cn

[Q71] 查看建表语句
来源：http://vn.hnjuh.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://eh.wgjwhj.cn

[Q72] 查看索引
来源：http://wv.jianghongdianzi.cn

SHOW INDEX FROM users;
来源：http://tw.yuntaijiaju.cn

[Q73] 查看表状态
来源：http://xr.muxihuayi.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://tg.9csxet.cn

[Q74] 强制使用索引
来源：http://dm.huanxung.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://er.huixiangedu.cn

[Q75] 日期格式化
来源：http://pb.haigaiapp.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://tv.yuntaijiaju.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://in.chemitech.net.cn

[Q76] 按天统计
来源：http://ks.jctech888.com.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ts.huixiangedu.cn

[Q77] 时间加减
来源：http://hz.chemitech.net.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://pm.521024.cn

[Q78] 当前时间
来源：http://ub.hnjuh.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://no.jianghongdianzi.cn

[Q79] 字符串拼接
来源：http://bc.shtwfgs.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://nt.panjiajie.cn

[Q80] 字符串截取
来源：http://zf.huixinmuqiang.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://pn.huixiangedu.cn

[Q81] 字符串替换
来源：http://cd.gzmigu.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://rv.huixiangedu.cn

[Q82] 字符长度与字节长度
来源：http://cc.shtwfgs.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://pc.jianghongdianzi.cn

[Q83] 大小写转换
来源：http://yl.bjjhwx.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://nx.gzmigu.cn

[Q84] 去除首尾空格
来源：http://pb.shxzskj.cn

SELECT TRIM(name) FROM users;
来源：http://ys.shtwfgs.cn

[Q85] 数值取整
来源：http://wj.521024.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://qc.chemitech.net.cn

[Q86] 读取 JSON 字段
来源：http://zp.jctech888.com.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ct.bookmarksfly.cn

[Q87] JSON 字段做条件
来源：http://ix.huanxung.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ts.asd995.cn

[Q88] 行转列（条件聚合）
来源：http://pn.panjiajie.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mp.shxzukj.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://tc.szxytkj.cn

[Q89] 判断表是否存在
来源：http://ll.hahajie.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://fn.hahajie.cn

[Q90] 生成序号列
来源：http://ti.shxzskj.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://cs.shtwfgs.cn

================================================================================
来源：http://hw.yuexingan06.cn

R. Bash 专题
来源：http://ol.521024.cn

================================================================================
来源：http://gi.huixiangedu.cn

[R01] shebang 与严格模式
来源：http://lw.yuexingan06.cn

#!/usr/bin/env bash
来源：http://in.nszjky.cn

set -euo pipefail
来源：http://xh.nszjky.cn

[R02] 变量赋值与使用
来源：http://cc.nszjky.cn

name="Tom"; echo "$name"
来源：http://pm.hnjuh.cn

[R03] 只读变量
来源：http://hs.521024.cn

readonly PI=3.14
来源：http://zs.521024.cn

[R04] 位置参数
来源：http://ka.huixinmuqiang.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://zj.huanxung.cn

[R05] 参数默认值
来源：http://rg.jianghongdianzi.cn

name="${1:-default}"
来源：http://vc.yuexingan06.cn

[R06] 判断命令是否存在
来源：http://ac.muxihuayi.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://xg.colortex.cn

[R07] if 判断文件
来源：http://qu.521024.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://yu.huixiangedu.cn

[R08] 数值比较
来源：http://ag.nicolike.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://do.bookmarksfly.cn

[R09] 字符串比较
来源：http://cb.asd995.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ou.521024.cn

[R10] 正则匹配
来源：http://qp.hahajie.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://rv.nicolike.cn

[R11] case 多分支
来源：http://hp.yuntaijiaju.cn

case "$1" in
来源：http://bk.shxzskj.cn

start) echo "启动" ;;
来源：http://nf.huixinmuqiang.cn

stop)  echo "停止" ;;
来源：http://fl.huanxung.cn

*)     echo "未知命令" ;;
来源：http://wd.newstarts.cn

esac
来源：http://zo.nicolike.cn

[R12] for 遍历文件
来源：http://re.nszjky.cn

for f in *.txt; do echo "$f"; done
来源：http://jr.huanxung.cn

[R13] for 计数循环
来源：http://nf.huanxung.cn

for i in {1..10}; do echo "$i"; done
来源：http://cf.colortex.cn

[R14] C 风格 for
来源：http://zu.bookmarksfly.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://jq.jctech888.com.cn

[R15] while 逐行读文件
来源：http://wb.jctech888.com.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://xv.nicolike.cn

[R16] until 等待条件
来源：http://ij.panjiajie.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ld.panjiajie.cn

[R17] 数组定义与取值
来源：http://il.colortex.cn

arr=(a b c); echo "${arr[0]}"
来源：http://rj.gzmigu.cn

[R18] 遍历数组
来源：http://nl.yuntaijiaju.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://dw.haigaiapp.cn

[R19] 数组长度
来源：http://pv.muxihuayi.cn

echo "${#arr[@]}"
来源：http://do.yuntaijiaju.cn

[R20] 关联数组（字典）
来源：http://ga.szxytkj.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://am.shtwfgs.cn

[R21] 字符串长度
来源：http://uu.huixiangedu.cn

echo "${#s}"
来源：http://hq.panjiajie.cn

[R22] 截取子串
来源：http://lg.hnjuh.cn

echo "${s:0:5}"
来源：http://sg.hnjuh.cn

[R23] 字符串替换
来源：http://ls.haigaiapp.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wr.yuexingan06.cn

[R24] 大小写转换
来源：http://nm.bjjhwx.cn

echo "${s^^}"; echo "${s,,}"
来源：http://by.huixinmuqiang.cn

[R25] 去后缀 / 去前缀
来源：http://aw.bjjhwx.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://bq.lnxyls.cn

[R26] 命令替换
来源：http://ny.huanxung.cn

now=$(date +%F); echo "$now"
来源：http://eq.haigaiapp.cn

[R27] 算术展开
来源：http://qe.shxzukj.cn

echo $((1 + 2 * 3))
来源：http://qv.shtwfgs.cn

[R28] 浮点运算
来源：http://jq.szsharing.cn

echo "scale=2; 10/3" | bc
来源：http://fv.nicolike.cn

[R29] 定义函数
来源：http://ig.asd995.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hc.521024.cn

[R30] 函数返回状态码
来源：http://kb.lnxyls.cn

f() { return 0; }; f || echo "失败了"
来源：http://vm.bookmarksfly.cn

[R31] 局部变量
来源：http://qs.9csxet.cn

f() { local x=1; echo "$x"; }
来源：http://bi.huixiangedu.cn

[R32] 参数个数校验
来源：http://sv.shtwfgs.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ju.nicolike.cn

[R33] 捕获错误并提示行号
来源：http://om.szxytkj.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://qf.nszjky.cn

[R34] 退出时清理
来源：http://kr.szxytkj.cn

trap 'rm -f "$tmp"' EXIT
来源：http://fb.yuntaijiaju.cn

[R35] 后台执行并等待
来源：http://ry.nicolike.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://oi.lnxyls.cn

[R36] 并发执行多个任务
来源：http://df.hnjuh.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://df.asd995.cn

[R37] 把输出赋给变量
来源：http://dr.chemitech.net.cn

files=$(ls -1)
来源：http://ze.nszjky.cn

[R38] 管道串联
来源：http://zy.shxzukj.cn

cat a.txt | grep -i error | wc -l
来源：http://yg.huixiangedu.cn

[R39] 重定向标准输出与错误
来源：http://mz.lnxyls.cn

cmd > out.log 2>&1
来源：http://lc.shxzskj.cn

[R40] 追加写日志
来源：http://lb.wgjwhj.cn

echo "log" >> out.log
来源：http://sf.nszjky.cn

[R41] 丢弃输出
来源：http://ck.szsharing.cn

cmd >/dev/null 2>&1
来源：http://ck.nszjky.cn

[R42] 输入重定向
来源：http://lk.bjjhwx.cn

wc -l < a.txt
来源：http://ma.hahajie.cn

[R43] 按名字查找文件
来源：http://ve.9csxet.cn

find . -name "*.log" -type f
来源：http://gg.huixinmuqiang.cn

[R44] 按修改时间查找
来源：http://ly.nszjky.cn

find . -mtime -7 -type f
来源：http://ei.wgjwhj.cn

[R45] 批量删除
来源：http://yb.huixiangedu.cn

find . -name "*.tmp" -delete
来源：http://hu.bjjhwx.cn

[R46] 递归替换文件内容
来源：http://sa.jctech888.com.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://vk.wgjwhj.cn

[R47] sed 单行替换
来源：http://ym.lnxyls.cn

sed -i 's/foo/bar/g' a.txt
来源：http://ex.yuntaijiaju.cn

[R48] awk 取指定列
来源：http://nf.nszjky.cn

awk '{print $1, $3}' a.txt
来源：http://tz.hnjuh.cn

[R49] awk 带条件
来源：http://us.9csxet.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ba.asd995.cn

[R50] awk 求和
来源：http://es.jianghongdianzi.cn

awk '{s += $2} END {print s}' a.txt
来源：http://bu.shtwfgs.cn

[R51] 排序去重取前几
来源：http://kf.9csxet.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://xd.521024.cn

[R52] 统计行数
来源：http://vl.newstarts.cn

wc -l a.txt
来源：http://gd.newstarts.cn

[R53] 查看文件头与实时尾
来源：http://fp.hahajie.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://jj.jianghongdianzi.cn

[R54] 比较两个文件
来源：http://je.gzmigu.cn

diff a.txt b.txt
来源：http://hh.nicolike.cn

[R55] 压缩与解压
来源：http://pe.newstarts.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://il.huixiangedu.cn

[R56] 远程拷贝
来源：http://tc.haigaiapp.cn

scp file user@host:/path/
来源：http://tg.bjjhwx.cn

[R57] 远程执行命令
来源：http://dt.hnjuh.cn

ssh user@host 'uptime'
来源：http://dl.jctech888.com.cn

[R58] 下载文件
来源：http://ab.jctech888.com.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wh.newstarts.cn

[R59] 发 POST JSON
来源：http://zn.jctech888.com.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://zk.panjiajie.cn

[R60] 只看 HTTP 状态码
来源：http://cr.colortex.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://he.hnjuh.cn

[R61] 磁盘占用
来源：http://jz.shxzukj.cn


<!-- 参考信息 -->