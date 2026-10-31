代发 wailian999

INSERT INTO users (name) VALUES ('C');
来源：http://fn.lnxyls.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://fy.lnxyls.cn

[Q13] 忽略重复插入
来源：http://nv.lnxyls.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://kg.jctech888.com.cn

[Q14] 存在则更新（upsert）
来源：http://et.hnjuh.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://tm.9csxet.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://qu.szsharing.cn

[Q15] 查询全部
来源：http://gg.bjjhwx.cn

SELECT * FROM users;
来源：http://nh.nicolike.cn

[Q16] 查询指定列
来源：http://mq.shtwfgs.cn

SELECT id, name FROM users;
来源：http://qr.yuntaijiaju.cn

[Q17] 条件查询
来源：http://uj.nicolike.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ue.shtwfgs.cn

[Q18] 模糊匹配
来源：http://gr.hahajie.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://xh.yuntaijiaju.cn

[Q19] 范围查询
来源：http://xz.newstarts.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://uy.shtwfgs.cn

[Q20] IN 列表
来源：http://zh.newstarts.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://zy.colortex.cn

[Q21] 空值判断
来源：http://zr.szsharing.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://uj.muxihuayi.cn

[Q22] 排序
来源：http://qy.gzmigu.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://td.521024.cn

[Q23] 分页
来源：http://zi.lnxyls.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hx.bookmarksfly.cn

[Q24] 去重
来源：http://we.521024.cn

SELECT DISTINCT city FROM users;
来源：http://ur.yuexingan06.cn

[Q25] 只取前 N 条
来源：http://ga.jctech888.com.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://qj.jctech888.com.cn

[Q26] 计数
来源：http://aw.lnxyls.cn

SELECT COUNT(*) FROM users;
来源：http://xu.gzmigu.cn

[Q27] 条件计数
来源：http://tc.shxzskj.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://uc.521024.cn

[Q28] 求和与平均
来源：http://iv.wgjwhj.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://ao.gzmigu.cn

[Q29] 最大最小值
来源：http://op.yuntaijiaju.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://pl.9csxet.cn

[Q30] 分组统计
来源：http://oc.szsharing.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://jj.bjjhwx.cn

[Q31] 分组后过滤
来源：http://xe.wgjwhj.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ss.hnjuh.cn

[Q32] 分组拼接字符串
来源：http://hq.wgjwhj.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://lo.jctech888.com.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://dj.colortex.cn

[Q33] 多列分组
来源：http://ew.huixinmuqiang.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://aa.jctech888.com.cn

[Q34] 每组取第一条
来源：http://ji.huixiangedu.cn

SELECT * FROM (
来源：http://my.chemitech.net.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://pp.jianghongdianzi.cn

) t WHERE rn = 1;
来源：http://sm.nszjky.cn

[Q35] 内连接
来源：http://yu.shtwfgs.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ya.shtwfgs.cn

[Q36] 左连接
来源：http://sd.bookmarksfly.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ca.huixinmuqiang.cn

[Q37] 右连接
来源：http://hd.hahajie.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ws.huanxung.cn

[Q38] 全外连接（PostgreSQL）
来源：http://me.chemitech.net.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ff.bookmarksfly.cn

[Q39] 自连接（查上下级）
来源：http://qc.wgjwhj.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://ps.gzmigu.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://gv.yuntaijiaju.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://qb.wgjwhj.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://tv.szxytkj.cn

[Q41] 多表连接
来源：http://sg.521024.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://oh.muxihuayi.cn

JOIN users u ON u.id = o.user_id
来源：http://my.521024.cn

JOIN products p ON p.id = o.product_id;
来源：http://iw.colortex.cn

[Q42] 连接条件附加过滤
来源：http://wh.huanxung.cn

SELECT u.name, o.amount FROM users u
来源：http://ds.huixiangedu.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://fs.bookmarksfly.cn

[Q43] 标量子查询
来源：http://nd.shxzukj.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://oi.bjjhwx.cn

[Q44] IN 子查询
来源：http://gm.panjiajie.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://bm.jianghongdianzi.cn

[Q45] EXISTS 判断存在
来源：http://wa.521024.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ys.jctech888.com.cn

[Q46] NOT EXISTS 判断不存在
来源：http://qm.szxytkj.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://jt.shxzukj.cn

[Q47] 与平均值比较
来源：http://ba.colortex.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://cb.wgjwhj.cn

[Q48] CTE 公用表表达式
来源：http://an.shtwfgs.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://cs.shtwfgs.cn

SELECT * FROM t WHERE c > 5;
来源：http://oh.hahajie.cn

[Q49] 更新单行
来源：http://fj.huixiangedu.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://zy.newstarts.cn

[Q50] 批量更新
来源：http://nk.9csxet.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://ay.shxzskj.cn

[Q51] 用子查询更新
来源：http://ys.9csxet.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wz.nszjky.cn

[Q52] 删除指定行
来源：http://zv.jctech888.com.cn

DELETE FROM users WHERE id = 10;
来源：http://oh.521024.cn

[Q53] 按条件删除
来源：http://rx.9csxet.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://zp.gzmigu.cn

[Q54] 清空表
来源：http://hc.bookmarksfly.cn

TRUNCATE TABLE logs;
来源：http://kc.huixinmuqiang.cn

[Q55] 排名（并列占位）
来源：http://dg.gzmigu.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://vz.yuexingan06.cn

[Q56] 密集排名（并列不占位）
来源：http://nr.nicolike.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://gc.asd995.cn

[Q57] 行号
来源：http://qt.bookmarksfly.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://fw.bjjhwx.cn

[Q58] 累计求和
来源：http://ko.szxytkj.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://eo.muxihuayi.cn

[Q59] 分组内累计
来源：http://ix.haigaiapp.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://fm.nszjky.cn

[Q60] 取上一行 / 下一行
来源：http://sb.szsharing.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mf.nicolike.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://xc.szsharing.cn

[Q61] 移动平均
来源：http://xs.nicolike.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://dv.nicolike.cn

[Q62] 分组占比
来源：http://vc.wgjwhj.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://rn.wgjwhj.cn

[Q63] 开启事务
来源：http://jp.jianghongdianzi.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://ys.shxzukj.cn

[Q64] 提交事务
来源：http://rz.gzmigu.cn

COMMIT;
来源：http://uz.shxzskj.cn

[Q65] 回滚事务
来源：http://wh.nszjky.cn

ROLLBACK;
来源：http://jz.bookmarksfly.cn

[Q66] 行锁查询
来源：http://uu.yuexingan06.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wu.szxytkj.cn

[Q67] 设置隔离级别
来源：http://dj.huixinmuqiang.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://tj.huixinmuqiang.cn

[Q68] 保存点
来源：http://af.panjiajie.cn

SAVEPOINT sp1;
来源：http://lu.haigaiapp.cn

ROLLBACK TO sp1;
来源：http://lz.521024.cn

[Q69] 查看执行计划
来源：http://jm.lnxyls.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://gl.colortex.cn

[Q70] 更新统计信息
来源：http://az.nszjky.cn

ANALYZE TABLE users;
来源：http://ab.asd995.cn

[Q71] 查看建表语句
来源：http://zv.9csxet.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://up.jctech888.com.cn

[Q72] 查看索引
来源：http://ar.shxzskj.cn

SHOW INDEX FROM users;
来源：http://ie.asd995.cn

[Q73] 查看表状态
来源：http://yv.haigaiapp.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://xj.muxihuayi.cn

[Q74] 强制使用索引
来源：http://da.panjiajie.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://jo.hnjuh.cn

[Q75] 日期格式化
来源：http://ub.bjjhwx.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://em.panjiajie.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hf.wgjwhj.cn

[Q76] 按天统计
来源：http://zg.szsharing.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://zw.gzmigu.cn

[Q77] 时间加减
来源：http://ik.newstarts.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://jf.bookmarksfly.cn

[Q78] 当前时间
来源：http://vc.bookmarksfly.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ge.wgjwhj.cn

[Q79] 字符串拼接
来源：http://pn.shxzukj.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://sz.bjjhwx.cn

[Q80] 字符串截取
来源：http://lt.jctech888.com.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mv.9csxet.cn

[Q81] 字符串替换
来源：http://dy.hnjuh.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://bz.hnjuh.cn

[Q82] 字符长度与字节长度
来源：http://uz.hahajie.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ix.szsharing.cn

[Q83] 大小写转换
来源：http://jz.asd995.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://fl.nicolike.cn

[Q84] 去除首尾空格
来源：http://fk.bookmarksfly.cn

SELECT TRIM(name) FROM users;
来源：http://qq.haigaiapp.cn

[Q85] 数值取整
来源：http://uw.haigaiapp.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://gy.jctech888.com.cn

[Q86] 读取 JSON 字段
来源：http://dr.haigaiapp.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://dy.shtwfgs.cn

[Q87] JSON 字段做条件
来源：http://kq.muxihuayi.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://co.asd995.cn

[Q88] 行转列（条件聚合）
来源：http://el.yuntaijiaju.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ft.huanxung.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://tb.shxzukj.cn

[Q89] 判断表是否存在
来源：http://xs.huixiangedu.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://kv.huixinmuqiang.cn

[Q90] 生成序号列
来源：http://gf.yuntaijiaju.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://te.bookmarksfly.cn

================================================================================
来源：http://sz.bookmarksfly.cn

R. Bash 专题
来源：http://wn.wgjwhj.cn

================================================================================
来源：http://dt.muxihuayi.cn

[R01] shebang 与严格模式
来源：http://db.nszjky.cn

#!/usr/bin/env bash
来源：http://dy.lnxyls.cn

set -euo pipefail
来源：http://xp.nicolike.cn

[R02] 变量赋值与使用
来源：http://sy.muxihuayi.cn

name="Tom"; echo "$name"
来源：http://iz.gzmigu.cn

[R03] 只读变量
来源：http://vk.huanxung.cn

readonly PI=3.14
来源：http://sf.huanxung.cn

[R04] 位置参数
来源：http://tt.gzmigu.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://jj.nicolike.cn

[R05] 参数默认值
来源：http://ym.nszjky.cn

name="${1:-default}"
来源：http://bz.shxzskj.cn

[R06] 判断命令是否存在
来源：http://cw.huixiangedu.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://bh.huixinmuqiang.cn

[R07] if 判断文件
来源：http://hk.lnxyls.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wf.yuntaijiaju.cn

[R08] 数值比较
来源：http://wy.jctech888.com.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://io.huixiangedu.cn

[R09] 字符串比较
来源：http://fk.gzmigu.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://jj.521024.cn

[R10] 正则匹配
来源：http://gi.hahajie.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://nu.shtwfgs.cn

[R11] case 多分支
来源：http://br.muxihuayi.cn

case "$1" in
来源：http://sv.huixiangedu.cn

start) echo "启动" ;;
来源：http://be.bjjhwx.cn

stop)  echo "停止" ;;
来源：http://pu.szsharing.cn

*)     echo "未知命令" ;;
来源：http://vu.nicolike.cn

esac
来源：http://gs.lnxyls.cn

[R12] for 遍历文件
来源：http://ji.yuexingan06.cn

for f in *.txt; do echo "$f"; done
来源：http://nc.shtwfgs.cn

[R13] for 计数循环
来源：http://wh.hahajie.cn

for i in {1..10}; do echo "$i"; done
来源：http://fa.lnxyls.cn

[R14] C 风格 for
来源：http://yi.jianghongdianzi.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://km.nszjky.cn

[R15] while 逐行读文件
来源：http://au.colortex.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://rl.huixinmuqiang.cn

[R16] until 等待条件
来源：http://iq.szxytkj.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://gg.chemitech.net.cn

[R17] 数组定义与取值
来源：http://jx.hnjuh.cn

arr=(a b c); echo "${arr[0]}"
来源：http://nl.yuntaijiaju.cn

[R18] 遍历数组
来源：http://ot.colortex.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ww.panjiajie.cn

[R19] 数组长度
来源：http://qu.colortex.cn

echo "${#arr[@]}"
来源：http://fk.shxzukj.cn

[R20] 关联数组（字典）
来源：http://ds.hnjuh.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://eb.nicolike.cn

[R21] 字符串长度
来源：http://jk.521024.cn

echo "${#s}"
来源：http://pa.jianghongdianzi.cn

[R22] 截取子串
来源：http://mc.bjjhwx.cn

echo "${s:0:5}"
来源：http://ib.nicolike.cn

[R23] 字符串替换
来源：http://dp.szsharing.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://yq.szsharing.cn

[R24] 大小写转换
来源：http://ju.bjjhwx.cn

echo "${s^^}"; echo "${s,,}"
来源：http://sz.chemitech.net.cn

[R25] 去后缀 / 去前缀
来源：http://ja.bjjhwx.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://my.yuntaijiaju.cn

[R26] 命令替换
来源：http://sp.huixiangedu.cn

now=$(date +%F); echo "$now"
来源：http://zx.nszjky.cn

[R27] 算术展开
来源：http://ko.chemitech.net.cn

echo $((1 + 2 * 3))
来源：http://ux.nicolike.cn

[R28] 浮点运算
来源：http://bi.521024.cn

echo "scale=2; 10/3" | bc
来源：http://yl.hahajie.cn

[R29] 定义函数
来源：http://cn.shtwfgs.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://qf.hnjuh.cn

[R30] 函数返回状态码
来源：http://jx.yuexingan06.cn

f() { return 0; }; f || echo "失败了"
来源：http://kp.yuexingan06.cn

[R31] 局部变量
来源：http://sy.asd995.cn

f() { local x=1; echo "$x"; }
来源：http://en.haigaiapp.cn

[R32] 参数个数校验
来源：http://wk.colortex.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://vt.colortex.cn

[R33] 捕获错误并提示行号
来源：http://wk.huanxung.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ms.shxzskj.cn

[R34] 退出时清理
来源：http://mw.wgjwhj.cn

trap 'rm -f "$tmp"' EXIT
来源：http://ur.huixinmuqiang.cn

[R35] 后台执行并等待
来源：http://sk.chemitech.net.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://gd.521024.cn

[R36] 并发执行多个任务
来源：http://mh.newstarts.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://qq.huixinmuqiang.cn

[R37] 把输出赋给变量
来源：http://gf.yuexingan06.cn

files=$(ls -1)
来源：http://uj.shtwfgs.cn

[R38] 管道串联
来源：http://de.nszjky.cn

cat a.txt | grep -i error | wc -l
来源：http://co.muxihuayi.cn

[R39] 重定向标准输出与错误
来源：http://nv.haigaiapp.cn

cmd > out.log 2>&1
来源：http://oz.wgjwhj.cn

[R40] 追加写日志
来源：http://ud.szxytkj.cn

echo "log" >> out.log
来源：http://kr.jctech888.com.cn

[R41] 丢弃输出
来源：http://gl.wgjwhj.cn

cmd >/dev/null 2>&1
来源：http://kg.colortex.cn

[R42] 输入重定向
来源：http://vn.yuntaijiaju.cn

wc -l < a.txt
来源：http://wj.bookmarksfly.cn

[R43] 按名字查找文件
来源：http://it.szsharing.cn

find . -name "*.log" -type f
来源：http://id.nszjky.cn

[R44] 按修改时间查找
来源：http://it.colortex.cn

find . -mtime -7 -type f
来源：http://gf.lnxyls.cn

[R45] 批量删除
来源：http://mu.nicolike.cn

find . -name "*.tmp" -delete
来源：http://mm.shxzskj.cn

[R46] 递归替换文件内容
来源：http://hr.nicolike.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://as.huixiangedu.cn

[R47] sed 单行替换
来源：http://dk.wgjwhj.cn

sed -i 's/foo/bar/g' a.txt
来源：http://fx.lnxyls.cn

[R48] awk 取指定列
来源：http://uo.huixinmuqiang.cn

awk '{print $1, $3}' a.txt
来源：http://qq.szxytkj.cn

[R49] awk 带条件
来源：http://dv.bookmarksfly.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://zk.szsharing.cn

[R50] awk 求和
来源：http://do.shxzukj.cn

awk '{s += $2} END {print s}' a.txt
来源：http://bs.hahajie.cn

[R51] 排序去重取前几
来源：http://sk.panjiajie.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://qb.haigaiapp.cn

[R52] 统计行数
来源：http://kr.hnjuh.cn

wc -l a.txt
来源：http://ws.szsharing.cn

[R53] 查看文件头与实时尾
来源：http://ys.colortex.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ym.shxzskj.cn

[R54] 比较两个文件
来源：http://tt.newstarts.cn

diff a.txt b.txt
来源：http://ka.huixinmuqiang.cn

[R55] 压缩与解压
来源：http://fe.chemitech.net.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://qf.wgjwhj.cn

[R56] 远程拷贝
来源：http://xw.shxzskj.cn

scp file user@host:/path/
来源：http://pf.shxzukj.cn

[R57] 远程执行命令
来源：http://vm.nszjky.cn

ssh user@host 'uptime'
来源：http://wq.nicolike.cn

[R58] 下载文件
来源：http://qm.huixinmuqiang.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ke.colortex.cn

[R59] 发 POST JSON
来源：http://vp.wgjwhj.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://an.muxihuayi.cn

[R60] 只看 HTTP 状态码
来源：http://ix.bookmarksfly.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://vc.hahajie.cn

[R61] 磁盘占用
来源：http://fz.szxytkj.cn


<!-- 参考信息 -->