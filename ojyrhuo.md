代发 wailian999

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://kl.szsharing.cn

[Q20] IN 列表
来源：http://gs.jctech888.com.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://bh.hahajie.cn

[Q21] 空值判断
来源：http://yb.shxzukj.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://je.lnxyls.cn

[Q22] 排序
来源：http://ai.szxytkj.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://fj.shtwfgs.cn

[Q23] 分页
来源：http://dd.asd995.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ok.nszjky.cn

[Q24] 去重
来源：http://tq.muxihuayi.cn

SELECT DISTINCT city FROM users;
来源：http://li.shtwfgs.cn

[Q25] 只取前 N 条
来源：http://ly.jianghongdianzi.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://gd.huanxung.cn

[Q26] 计数
来源：http://rk.yuexingan06.cn

SELECT COUNT(*) FROM users;
来源：http://kk.gzmigu.cn

[Q27] 条件计数
来源：http://pk.bookmarksfly.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://tx.nszjky.cn

[Q28] 求和与平均
来源：http://lu.jctech888.com.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://kv.gzmigu.cn

[Q29] 最大最小值
来源：http://kk.yuexingan06.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://bm.colortex.cn

[Q30] 分组统计
来源：http://ys.521024.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://kb.wgjwhj.cn

[Q31] 分组后过滤
来源：http://ny.shxzskj.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wp.asd995.cn

[Q32] 分组拼接字符串
来源：http://vv.huixiangedu.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://dg.colortex.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://xf.bjjhwx.cn

[Q33] 多列分组
来源：http://cl.jctech888.com.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://gb.yuntaijiaju.cn

[Q34] 每组取第一条
来源：http://wf.bjjhwx.cn

SELECT * FROM (
来源：http://vg.gzmigu.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ze.shtwfgs.cn

) t WHERE rn = 1;
来源：http://cm.shxzukj.cn

[Q35] 内连接
来源：http://xl.521024.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://pt.hnjuh.cn

[Q36] 左连接
来源：http://oc.lnxyls.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hp.521024.cn

[Q37] 右连接
来源：http://ow.shtwfgs.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://tf.huixiangedu.cn

[Q38] 全外连接（PostgreSQL）
来源：http://mr.asd995.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hs.newstarts.cn

[Q39] 自连接（查上下级）
来源：http://ws.haigaiapp.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://iy.nicolike.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://nn.huixiangedu.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://te.huanxung.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://eh.nszjky.cn

[Q41] 多表连接
来源：http://nh.chemitech.net.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://ep.shxzskj.cn

JOIN users u ON u.id = o.user_id
来源：http://py.chemitech.net.cn

JOIN products p ON p.id = o.product_id;
来源：http://uy.huixiangedu.cn

[Q42] 连接条件附加过滤
来源：http://kw.szsharing.cn

SELECT u.name, o.amount FROM users u
来源：http://xr.muxihuayi.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://tn.huanxung.cn

[Q43] 标量子查询
来源：http://gk.haigaiapp.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://ys.nszjky.cn

[Q44] IN 子查询
来源：http://ji.yuntaijiaju.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://bj.gzmigu.cn

[Q45] EXISTS 判断存在
来源：http://fo.nicolike.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://iw.colortex.cn

[Q46] NOT EXISTS 判断不存在
来源：http://ep.bjjhwx.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://dh.wgjwhj.cn

[Q47] 与平均值比较
来源：http://wp.huixiangedu.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://zb.chemitech.net.cn

[Q48] CTE 公用表表达式
来源：http://rx.huixinmuqiang.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://re.chemitech.net.cn

SELECT * FROM t WHERE c > 5;
来源：http://nr.colortex.cn

[Q49] 更新单行
来源：http://xo.lnxyls.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://bj.chemitech.net.cn

[Q50] 批量更新
来源：http://mc.nicolike.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://xk.yuexingan06.cn

[Q51] 用子查询更新
来源：http://bf.hnjuh.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://sb.bjjhwx.cn

[Q52] 删除指定行
来源：http://wh.jctech888.com.cn

DELETE FROM users WHERE id = 10;
来源：http://jv.hnjuh.cn

[Q53] 按条件删除
来源：http://yi.colortex.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://fy.521024.cn

[Q54] 清空表
来源：http://ra.szsharing.cn

TRUNCATE TABLE logs;
来源：http://at.shxzskj.cn

[Q55] 排名（并列占位）
来源：http://lp.yuexingan06.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://dh.newstarts.cn

[Q56] 密集排名（并列不占位）
来源：http://eb.9csxet.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://yh.haigaiapp.cn

[Q57] 行号
来源：http://uu.wgjwhj.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://rr.hnjuh.cn

[Q58] 累计求和
来源：http://jk.yuntaijiaju.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ou.hahajie.cn

[Q59] 分组内累计
来源：http://uw.szsharing.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://bj.lnxyls.cn

[Q60] 取上一行 / 下一行
来源：http://qa.szxytkj.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://nn.wgjwhj.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://zw.chemitech.net.cn

[Q61] 移动平均
来源：http://ld.szsharing.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://sk.panjiajie.cn

[Q62] 分组占比
来源：http://li.bjjhwx.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ba.szsharing.cn

[Q63] 开启事务
来源：http://xg.hnjuh.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://kl.nszjky.cn

[Q64] 提交事务
来源：http://mj.huixiangedu.cn

COMMIT;
来源：http://wz.jianghongdianzi.cn

[Q65] 回滚事务
来源：http://ef.wgjwhj.cn

ROLLBACK;
来源：http://me.wgjwhj.cn

[Q66] 行锁查询
来源：http://gx.lnxyls.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ie.521024.cn

[Q67] 设置隔离级别
来源：http://di.haigaiapp.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://bi.panjiajie.cn

[Q68] 保存点
来源：http://qj.chemitech.net.cn

SAVEPOINT sp1;
来源：http://dg.haigaiapp.cn

ROLLBACK TO sp1;
来源：http://qh.yuntaijiaju.cn

[Q69] 查看执行计划
来源：http://pf.muxihuayi.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://bg.szxytkj.cn

[Q70] 更新统计信息
来源：http://iv.szxytkj.cn

ANALYZE TABLE users;
来源：http://ja.huixinmuqiang.cn

[Q71] 查看建表语句
来源：http://kc.colortex.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://dg.bjjhwx.cn

[Q72] 查看索引
来源：http://ko.yuexingan06.cn

SHOW INDEX FROM users;
来源：http://px.jctech888.com.cn

[Q73] 查看表状态
来源：http://nm.szxytkj.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://uw.bjjhwx.cn

[Q74] 强制使用索引
来源：http://it.shxzukj.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ht.521024.cn

[Q75] 日期格式化
来源：http://ov.wgjwhj.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://fo.wgjwhj.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://vr.panjiajie.cn

[Q76] 按天统计
来源：http://kd.szsharing.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ik.asd995.cn

[Q77] 时间加减
来源：http://sh.yuntaijiaju.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://lx.huanxung.cn

[Q78] 当前时间
来源：http://gy.521024.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://gu.nicolike.cn

[Q79] 字符串拼接
来源：http://ri.nszjky.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://qm.521024.cn

[Q80] 字符串截取
来源：http://zj.nicolike.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hv.muxihuayi.cn

[Q81] 字符串替换
来源：http://sr.hahajie.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://eu.asd995.cn

[Q82] 字符长度与字节长度
来源：http://us.bjjhwx.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://be.huanxung.cn

[Q83] 大小写转换
来源：http://yr.shtwfgs.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://zg.9csxet.cn

[Q84] 去除首尾空格
来源：http://dp.hahajie.cn

SELECT TRIM(name) FROM users;
来源：http://ba.wgjwhj.cn

[Q85] 数值取整
来源：http://dw.huixiangedu.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://jz.gzmigu.cn

[Q86] 读取 JSON 字段
来源：http://ts.colortex.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://pv.shxzskj.cn

[Q87] JSON 字段做条件
来源：http://vs.hnjuh.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://rd.bjjhwx.cn

[Q88] 行转列（条件聚合）
来源：http://sm.huixinmuqiang.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://qy.bookmarksfly.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wq.yuexingan06.cn

[Q89] 判断表是否存在
来源：http://rj.panjiajie.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://rh.chemitech.net.cn

[Q90] 生成序号列
来源：http://bq.nszjky.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mp.521024.cn

================================================================================
来源：http://ph.huixinmuqiang.cn

R. Bash 专题
来源：http://bf.hahajie.cn

================================================================================
来源：http://ef.huixiangedu.cn

[R01] shebang 与严格模式
来源：http://jc.bjjhwx.cn

#!/usr/bin/env bash
来源：http://ne.huixinmuqiang.cn

set -euo pipefail
来源：http://bd.yuntaijiaju.cn

[R02] 变量赋值与使用
来源：http://id.shxzskj.cn

name="Tom"; echo "$name"
来源：http://nk.asd995.cn

[R03] 只读变量
来源：http://ys.haigaiapp.cn

readonly PI=3.14
来源：http://fy.chemitech.net.cn

[R04] 位置参数
来源：http://as.shtwfgs.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://qx.wgjwhj.cn

[R05] 参数默认值
来源：http://qg.huixiangedu.cn

name="${1:-default}"
来源：http://mp.nicolike.cn

[R06] 判断命令是否存在
来源：http://zg.newstarts.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://sg.szxytkj.cn

[R07] if 判断文件
来源：http://qk.shxzukj.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://tk.gzmigu.cn

[R08] 数值比较
来源：http://ya.nicolike.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://nu.panjiajie.cn

[R09] 字符串比较
来源：http://rh.szxytkj.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ob.chemitech.net.cn

[R10] 正则匹配
来源：http://hc.521024.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://se.jctech888.com.cn

[R11] case 多分支
来源：http://bg.gzmigu.cn

case "$1" in
来源：http://rt.szsharing.cn

start) echo "启动" ;;
来源：http://qp.9csxet.cn

stop)  echo "停止" ;;
来源：http://an.nszjky.cn

*)     echo "未知命令" ;;
来源：http://dc.huixinmuqiang.cn

esac
来源：http://ke.haigaiapp.cn

[R12] for 遍历文件
来源：http://fc.hahajie.cn

for f in *.txt; do echo "$f"; done
来源：http://zp.shtwfgs.cn

[R13] for 计数循环
来源：http://fo.gzmigu.cn

for i in {1..10}; do echo "$i"; done
来源：http://la.newstarts.cn

[R14] C 风格 for
来源：http://cz.hnjuh.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://vy.szsharing.cn

[R15] while 逐行读文件
来源：http://gx.jianghongdianzi.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://pq.wgjwhj.cn

[R16] until 等待条件
来源：http://ch.huixinmuqiang.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://qj.lnxyls.cn

[R17] 数组定义与取值
来源：http://ra.szsharing.cn

arr=(a b c); echo "${arr[0]}"
来源：http://hw.newstarts.cn

[R18] 遍历数组
来源：http://gd.hahajie.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://gn.jctech888.com.cn

[R19] 数组长度
来源：http://cz.szsharing.cn

echo "${#arr[@]}"
来源：http://fb.hahajie.cn

[R20] 关联数组（字典）
来源：http://hq.huixiangedu.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://zy.nszjky.cn

[R21] 字符串长度
来源：http://mu.nicolike.cn

echo "${#s}"
来源：http://mo.nszjky.cn

[R22] 截取子串
来源：http://lp.nszjky.cn

echo "${s:0:5}"
来源：http://tu.yuexingan06.cn

[R23] 字符串替换
来源：http://zw.yuntaijiaju.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://nn.huixiangedu.cn

[R24] 大小写转换
来源：http://oy.hnjuh.cn

echo "${s^^}"; echo "${s,,}"
来源：http://ay.jianghongdianzi.cn

[R25] 去后缀 / 去前缀
来源：http://nx.shtwfgs.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://yk.muxihuayi.cn

[R26] 命令替换
来源：http://ss.nszjky.cn

now=$(date +%F); echo "$now"
来源：http://bl.colortex.cn

[R27] 算术展开
来源：http://py.521024.cn

echo $((1 + 2 * 3))
来源：http://ds.hnjuh.cn

[R28] 浮点运算
来源：http://ya.yuexingan06.cn

echo "scale=2; 10/3" | bc
来源：http://ye.nicolike.cn

[R29] 定义函数
来源：http://cy.9csxet.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://bl.huixinmuqiang.cn

[R30] 函数返回状态码
来源：http://yx.9csxet.cn

f() { return 0; }; f || echo "失败了"
来源：http://xp.hahajie.cn

[R31] 局部变量
来源：http://fw.huanxung.cn

f() { local x=1; echo "$x"; }
来源：http://he.jctech888.com.cn

[R32] 参数个数校验
来源：http://gh.bookmarksfly.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://zq.chemitech.net.cn

[R33] 捕获错误并提示行号
来源：http://yi.szsharing.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://cn.9csxet.cn

[R34] 退出时清理
来源：http://xe.nszjky.cn

trap 'rm -f "$tmp"' EXIT
来源：http://dk.shxzskj.cn

[R35] 后台执行并等待
来源：http://kf.chemitech.net.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://gh.yuexingan06.cn

[R36] 并发执行多个任务
来源：http://ny.bjjhwx.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ny.9csxet.cn

[R37] 把输出赋给变量
来源：http://ot.bookmarksfly.cn

files=$(ls -1)
来源：http://xk.muxihuayi.cn

[R38] 管道串联
来源：http://or.yuexingan06.cn

cat a.txt | grep -i error | wc -l
来源：http://by.szsharing.cn

[R39] 重定向标准输出与错误
来源：http://ii.yuntaijiaju.cn

cmd > out.log 2>&1
来源：http://mq.jianghongdianzi.cn

[R40] 追加写日志
来源：http://nh.bookmarksfly.cn

echo "log" >> out.log
来源：http://sx.nicolike.cn

[R41] 丢弃输出
来源：http://nw.newstarts.cn

cmd >/dev/null 2>&1
来源：http://sf.yuntaijiaju.cn

[R42] 输入重定向
来源：http://nd.hahajie.cn

wc -l < a.txt
来源：http://aa.yuexingan06.cn

[R43] 按名字查找文件
来源：http://hs.nicolike.cn

find . -name "*.log" -type f
来源：http://yp.huixiangedu.cn

[R44] 按修改时间查找
来源：http://df.nszjky.cn

find . -mtime -7 -type f
来源：http://yk.jianghongdianzi.cn

[R45] 批量删除
来源：http://om.chemitech.net.cn

find . -name "*.tmp" -delete
来源：http://ke.huanxung.cn

[R46] 递归替换文件内容
来源：http://vk.huanxung.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://jd.lnxyls.cn

[R47] sed 单行替换
来源：http://qv.bookmarksfly.cn

sed -i 's/foo/bar/g' a.txt
来源：http://lg.wgjwhj.cn

[R48] awk 取指定列
来源：http://nd.shtwfgs.cn

awk '{print $1, $3}' a.txt
来源：http://kv.521024.cn

[R49] awk 带条件
来源：http://dk.colortex.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://vv.shtwfgs.cn

[R50] awk 求和
来源：http://on.panjiajie.cn

awk '{s += $2} END {print s}' a.txt
来源：http://aa.asd995.cn

[R51] 排序去重取前几
来源：http://um.nszjky.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://sb.jianghongdianzi.cn

[R52] 统计行数
来源：http://km.bjjhwx.cn

wc -l a.txt
来源：http://et.huixiangedu.cn

[R53] 查看文件头与实时尾
来源：http://cy.chemitech.net.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://sc.jctech888.com.cn

[R54] 比较两个文件
来源：http://kg.yuexingan06.cn

diff a.txt b.txt
来源：http://av.shxzukj.cn

[R55] 压缩与解压
来源：http://dj.bookmarksfly.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://gr.asd995.cn

[R56] 远程拷贝
来源：http://ad.asd995.cn

scp file user@host:/path/
来源：http://kw.bookmarksfly.cn

[R57] 远程执行命令
来源：http://ii.chemitech.net.cn

ssh user@host 'uptime'
来源：http://by.shxzukj.cn

[R58] 下载文件
来源：http://va.nszjky.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://vw.hnjuh.cn

[R59] 发 POST JSON
来源：http://qq.bookmarksfly.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://uf.chemitech.net.cn

[R60] 只看 HTTP 状态码
来源：http://tb.bjjhwx.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ro.yuntaijiaju.cn

[R61] 磁盘占用
来源：http://fa.shxzukj.cn

df -h;  du -sh *
来源：http://bu.huixinmuqiang.cn

[R62] 找最占空间的文件
来源：http://bc.hahajie.cn

du -ah . | sort -rh | head -10
来源：http://lr.521024.cn

[R63] 内存与进程
来源：http://yi.hnjuh.cn

free -h;  ps aux | grep nginx
来源：http://gq.shxzukj.cn

[R64] 结束进程
来源：http://yc.521024.cn

kill -9 $(pgrep -f app.py)
来源：http://jh.huixiangedu.cn

[R65] 查看端口占用
来源：http://cf.bookmarksfly.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ls.szsharing.cn

[R66] 定时任务
来源：http://cy.colortex.cn

crontab -e;  crontab -l
来源：http://we.yuntaijiaju.cn

[R67] 生成随机十六进制串
来源：http://fu.yuexingan06.cn

openssl rand -hex 16
来源：http://yu.panjiajie.cn

[R68] 计算文件校验值
来源：http://ns.yuntaijiaju.cn

sha256sum a.txt;  md5sum a.txt
来源：http://lc.bookmarksfly.cn

[R69] 生成随机密码
来源：http://ap.lnxyls.cn


<!-- 参考信息 -->