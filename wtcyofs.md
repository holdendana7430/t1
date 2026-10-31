代发 wailian999

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ut.lnxyls.cn

[Q11] 一次插入多行
来源：http://kz.chemitech.net.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://qc.9csxet.cn

[Q12] 插入后取自增 ID
来源：http://fg.521024.cn

INSERT INTO users (name) VALUES ('C');
来源：http://qp.yuexingan06.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ry.hahajie.cn

[Q13] 忽略重复插入
来源：http://dx.yuexingan06.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://nw.huanxung.cn

[Q14] 存在则更新（upsert）
来源：http://tw.nicolike.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://kl.haigaiapp.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://pd.hahajie.cn

[Q15] 查询全部
来源：http://fi.huanxung.cn

SELECT * FROM users;
来源：http://aj.newstarts.cn

[Q16] 查询指定列
来源：http://xy.lnxyls.cn

SELECT id, name FROM users;
来源：http://wo.asd995.cn

[Q17] 条件查询
来源：http://gw.bjjhwx.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://oo.muxihuayi.cn

[Q18] 模糊匹配
来源：http://ro.huanxung.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ai.bjjhwx.cn

[Q19] 范围查询
来源：http://nd.nszjky.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://pz.lnxyls.cn

[Q20] IN 列表
来源：http://mm.jctech888.com.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://zx.shxzukj.cn

[Q21] 空值判断
来源：http://im.haigaiapp.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://gd.521024.cn

[Q22] 排序
来源：http://rs.szsharing.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ba.shtwfgs.cn

[Q23] 分页
来源：http://kf.wgjwhj.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://qq.hnjuh.cn

[Q24] 去重
来源：http://dc.asd995.cn

SELECT DISTINCT city FROM users;
来源：http://ce.hahajie.cn

[Q25] 只取前 N 条
来源：http://sj.huixinmuqiang.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://rh.hnjuh.cn

[Q26] 计数
来源：http://eo.jctech888.com.cn

SELECT COUNT(*) FROM users;
来源：http://zd.9csxet.cn

[Q27] 条件计数
来源：http://cg.hahajie.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://go.521024.cn

[Q28] 求和与平均
来源：http://sw.hnjuh.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://cg.nicolike.cn

[Q29] 最大最小值
来源：http://jw.panjiajie.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://er.yuexingan06.cn

[Q30] 分组统计
来源：http://pa.jianghongdianzi.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ly.gzmigu.cn

[Q31] 分组后过滤
来源：http://fa.huanxung.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://sf.lnxyls.cn

[Q32] 分组拼接字符串
来源：http://re.newstarts.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://lq.panjiajie.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://cy.shxzukj.cn

[Q33] 多列分组
来源：http://iz.chemitech.net.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://rp.gzmigu.cn

[Q34] 每组取第一条
来源：http://mn.huixinmuqiang.cn

SELECT * FROM (
来源：http://en.huixinmuqiang.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://vo.jianghongdianzi.cn

) t WHERE rn = 1;
来源：http://mo.huixiangedu.cn

[Q35] 内连接
来源：http://aa.hahajie.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://cm.nszjky.cn

[Q36] 左连接
来源：http://lj.shxzskj.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ud.521024.cn

[Q37] 右连接
来源：http://rs.huixinmuqiang.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://oo.szxytkj.cn

[Q38] 全外连接（PostgreSQL）
来源：http://nr.huanxung.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://kt.szsharing.cn

[Q39] 自连接（查上下级）
来源：http://zx.nszjky.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://ya.hahajie.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ji.shxzukj.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://gq.nszjky.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://rp.huixinmuqiang.cn

[Q41] 多表连接
来源：http://fw.shxzskj.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://ko.huanxung.cn

JOIN users u ON u.id = o.user_id
来源：http://ju.yuntaijiaju.cn

JOIN products p ON p.id = o.product_id;
来源：http://wa.colortex.cn

[Q42] 连接条件附加过滤
来源：http://vb.huanxung.cn

SELECT u.name, o.amount FROM users u
来源：http://cd.gzmigu.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://cx.newstarts.cn

[Q43] 标量子查询
来源：http://gc.9csxet.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://yh.yuntaijiaju.cn

[Q44] IN 子查询
来源：http://by.jctech888.com.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://yz.shxzukj.cn

[Q45] EXISTS 判断存在
来源：http://ed.huanxung.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://fw.shxzskj.cn

[Q46] NOT EXISTS 判断不存在
来源：http://mf.gzmigu.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://eg.521024.cn

[Q47] 与平均值比较
来源：http://fz.huixiangedu.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://dx.haigaiapp.cn

[Q48] CTE 公用表表达式
来源：http://ct.panjiajie.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mn.haigaiapp.cn

SELECT * FROM t WHERE c > 5;
来源：http://uf.nszjky.cn

[Q49] 更新单行
来源：http://so.colortex.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hd.jctech888.com.cn

[Q50] 批量更新
来源：http://sc.521024.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://sq.haigaiapp.cn

[Q51] 用子查询更新
来源：http://ow.gzmigu.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://cd.jianghongdianzi.cn

[Q52] 删除指定行
来源：http://fb.nicolike.cn

DELETE FROM users WHERE id = 10;
来源：http://tv.hahajie.cn

[Q53] 按条件删除
来源：http://ko.9csxet.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ba.bjjhwx.cn

[Q54] 清空表
来源：http://fk.gzmigu.cn

TRUNCATE TABLE logs;
来源：http://an.szxytkj.cn

[Q55] 排名（并列占位）
来源：http://pv.yuexingan06.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://si.yuexingan06.cn

[Q56] 密集排名（并列不占位）
来源：http://kv.yuexingan06.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://no.colortex.cn

[Q57] 行号
来源：http://hi.bookmarksfly.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://jf.haigaiapp.cn

[Q58] 累计求和
来源：http://pi.panjiajie.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://bl.shtwfgs.cn

[Q59] 分组内累计
来源：http://cf.nszjky.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://li.hnjuh.cn

[Q60] 取上一行 / 下一行
来源：http://yo.huixiangedu.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://or.gzmigu.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://nf.jianghongdianzi.cn

[Q61] 移动平均
来源：http://ve.hahajie.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://cb.lnxyls.cn

[Q62] 分组占比
来源：http://iv.yuntaijiaju.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://bn.yuexingan06.cn

[Q63] 开启事务
来源：http://ji.wgjwhj.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://ou.huixinmuqiang.cn

[Q64] 提交事务
来源：http://wy.huanxung.cn

COMMIT;
来源：http://pv.colortex.cn

[Q65] 回滚事务
来源：http://nt.newstarts.cn

ROLLBACK;
来源：http://tz.nszjky.cn

[Q66] 行锁查询
来源：http://we.huixiangedu.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://yv.yuntaijiaju.cn

[Q67] 设置隔离级别
来源：http://ub.9csxet.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wp.wgjwhj.cn

[Q68] 保存点
来源：http://hz.muxihuayi.cn

SAVEPOINT sp1;
来源：http://cb.gzmigu.cn

ROLLBACK TO sp1;
来源：http://pf.shxzukj.cn

[Q69] 查看执行计划
来源：http://jc.jianghongdianzi.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ey.gzmigu.cn

[Q70] 更新统计信息
来源：http://wx.gzmigu.cn

ANALYZE TABLE users;
来源：http://ln.hnjuh.cn

[Q71] 查看建表语句
来源：http://mx.bookmarksfly.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://va.wgjwhj.cn

[Q72] 查看索引
来源：http://pz.hahajie.cn

SHOW INDEX FROM users;
来源：http://qk.nszjky.cn

[Q73] 查看表状态
来源：http://nt.gzmigu.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://md.gzmigu.cn

[Q74] 强制使用索引
来源：http://mo.huanxung.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hk.jctech888.com.cn

[Q75] 日期格式化
来源：http://ua.yuexingan06.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://vh.9csxet.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wm.chemitech.net.cn

[Q76] 按天统计
来源：http://ux.jctech888.com.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://xx.hnjuh.cn

[Q77] 时间加减
来源：http://sh.shxzukj.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://yx.wgjwhj.cn

[Q78] 当前时间
来源：http://ut.newstarts.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://tx.bookmarksfly.cn

[Q79] 字符串拼接
来源：http://cc.gzmigu.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://cy.shxzskj.cn

[Q80] 字符串截取
来源：http://gl.gzmigu.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://yt.shtwfgs.cn

[Q81] 字符串替换
来源：http://ne.lnxyls.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ya.yuntaijiaju.cn

[Q82] 字符长度与字节长度
来源：http://bj.haigaiapp.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://kr.9csxet.cn

[Q83] 大小写转换
来源：http://cd.shxzskj.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://xn.huixiangedu.cn

[Q84] 去除首尾空格
来源：http://xb.szsharing.cn

SELECT TRIM(name) FROM users;
来源：http://vx.chemitech.net.cn

[Q85] 数值取整
来源：http://tm.nicolike.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://so.huanxung.cn

[Q86] 读取 JSON 字段
来源：http://bl.panjiajie.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://if.shtwfgs.cn

[Q87] JSON 字段做条件
来源：http://vk.shxzukj.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://rv.jctech888.com.cn

[Q88] 行转列（条件聚合）
来源：http://pf.haigaiapp.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wk.newstarts.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://jp.nicolike.cn

[Q89] 判断表是否存在
来源：http://ez.shxzskj.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://qi.shtwfgs.cn

[Q90] 生成序号列
来源：http://og.bookmarksfly.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://gp.521024.cn

================================================================================
来源：http://ol.yuntaijiaju.cn

R. Bash 专题
来源：http://ui.chemitech.net.cn

================================================================================
来源：http://vm.lnxyls.cn

[R01] shebang 与严格模式
来源：http://cd.asd995.cn

#!/usr/bin/env bash
来源：http://vh.nicolike.cn

set -euo pipefail
来源：http://ds.lnxyls.cn

[R02] 变量赋值与使用
来源：http://xr.shxzskj.cn

name="Tom"; echo "$name"
来源：http://md.wgjwhj.cn

[R03] 只读变量
来源：http://xc.jctech888.com.cn

readonly PI=3.14
来源：http://rb.hnjuh.cn

[R04] 位置参数
来源：http://jz.521024.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ho.521024.cn

[R05] 参数默认值
来源：http://cw.haigaiapp.cn

name="${1:-default}"
来源：http://mc.colortex.cn

[R06] 判断命令是否存在
来源：http://jh.hnjuh.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://do.shxzukj.cn

[R07] if 判断文件
来源：http://ok.jctech888.com.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://kj.huixinmuqiang.cn

[R08] 数值比较
来源：http://fa.szsharing.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://hb.szsharing.cn

[R09] 字符串比较
来源：http://gc.bjjhwx.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ns.shxzukj.cn

[R10] 正则匹配
来源：http://ey.szsharing.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://dz.shxzukj.cn

[R11] case 多分支
来源：http://jy.nszjky.cn

case "$1" in
来源：http://et.9csxet.cn

start) echo "启动" ;;
来源：http://ws.yuexingan06.cn

stop)  echo "停止" ;;
来源：http://ab.chemitech.net.cn

*)     echo "未知命令" ;;
来源：http://wn.lnxyls.cn

esac
来源：http://fs.bjjhwx.cn

[R12] for 遍历文件
来源：http://hj.yuntaijiaju.cn

for f in *.txt; do echo "$f"; done
来源：http://qo.newstarts.cn

[R13] for 计数循环
来源：http://fw.newstarts.cn

for i in {1..10}; do echo "$i"; done
来源：http://km.newstarts.cn

[R14] C 风格 for
来源：http://rk.szsharing.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://xv.colortex.cn

[R15] while 逐行读文件
来源：http://pj.9csxet.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://vs.lnxyls.cn

[R16] until 等待条件
来源：http://wu.lnxyls.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://tj.nicolike.cn

[R17] 数组定义与取值
来源：http://sl.wgjwhj.cn

arr=(a b c); echo "${arr[0]}"
来源：http://jl.asd995.cn

[R18] 遍历数组
来源：http://oz.shtwfgs.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://tb.panjiajie.cn

[R19] 数组长度
来源：http://nj.chemitech.net.cn

echo "${#arr[@]}"
来源：http://gy.szsharing.cn

[R20] 关联数组（字典）
来源：http://jf.newstarts.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://lt.9csxet.cn

[R21] 字符串长度
来源：http://bg.muxihuayi.cn

echo "${#s}"
来源：http://vg.9csxet.cn

[R22] 截取子串
来源：http://gc.nszjky.cn

echo "${s:0:5}"
来源：http://si.shxzukj.cn

[R23] 字符串替换
来源：http://dh.szsharing.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://sx.yuntaijiaju.cn

[R24] 大小写转换
来源：http://fs.bjjhwx.cn

echo "${s^^}"; echo "${s,,}"
来源：http://xg.szsharing.cn

[R25] 去后缀 / 去前缀
来源：http://rb.szxytkj.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://if.shxzskj.cn

[R26] 命令替换
来源：http://zb.9csxet.cn

now=$(date +%F); echo "$now"
来源：http://rt.yuntaijiaju.cn

[R27] 算术展开
来源：http://we.asd995.cn

echo $((1 + 2 * 3))
来源：http://mc.newstarts.cn

[R28] 浮点运算
来源：http://yj.muxihuayi.cn

echo "scale=2; 10/3" | bc
来源：http://on.panjiajie.cn

[R29] 定义函数
来源：http://ya.szsharing.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://et.bjjhwx.cn

[R30] 函数返回状态码
来源：http://sv.bookmarksfly.cn

f() { return 0; }; f || echo "失败了"
来源：http://bl.9csxet.cn

[R31] 局部变量
来源：http://uv.jianghongdianzi.cn

f() { local x=1; echo "$x"; }
来源：http://wv.huixinmuqiang.cn

[R32] 参数个数校验
来源：http://pj.nicolike.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://nl.yuntaijiaju.cn

[R33] 捕获错误并提示行号
来源：http://nj.panjiajie.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://xz.huixiangedu.cn

[R34] 退出时清理
来源：http://tp.jianghongdianzi.cn

trap 'rm -f "$tmp"' EXIT
来源：http://qv.bjjhwx.cn

[R35] 后台执行并等待
来源：http://li.nszjky.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://hu.bjjhwx.cn

[R36] 并发执行多个任务
来源：http://pu.szsharing.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://yv.lnxyls.cn

[R37] 把输出赋给变量
来源：http://ii.huixinmuqiang.cn

files=$(ls -1)
来源：http://jb.jianghongdianzi.cn

[R38] 管道串联
来源：http://ng.jctech888.com.cn

cat a.txt | grep -i error | wc -l
来源：http://mc.nicolike.cn

[R39] 重定向标准输出与错误
来源：http://qj.haigaiapp.cn

cmd > out.log 2>&1
来源：http://kt.521024.cn

[R40] 追加写日志
来源：http://km.chemitech.net.cn

echo "log" >> out.log
来源：http://lw.muxihuayi.cn

[R41] 丢弃输出
来源：http://gm.jianghongdianzi.cn

cmd >/dev/null 2>&1
来源：http://bp.bjjhwx.cn

[R42] 输入重定向
来源：http://vj.chemitech.net.cn

wc -l < a.txt
来源：http://lp.shxzukj.cn

[R43] 按名字查找文件
来源：http://ja.nicolike.cn

find . -name "*.log" -type f
来源：http://of.huanxung.cn

[R44] 按修改时间查找
来源：http://hd.jianghongdianzi.cn

find . -mtime -7 -type f
来源：http://wu.yuntaijiaju.cn

[R45] 批量删除
来源：http://eu.newstarts.cn

find . -name "*.tmp" -delete
来源：http://wl.wgjwhj.cn

[R46] 递归替换文件内容
来源：http://pr.shtwfgs.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://tp.asd995.cn

[R47] sed 单行替换
来源：http://mv.bookmarksfly.cn

sed -i 's/foo/bar/g' a.txt
来源：http://go.asd995.cn

[R48] awk 取指定列
来源：http://mq.bookmarksfly.cn

awk '{print $1, $3}' a.txt
来源：http://dg.bjjhwx.cn

[R49] awk 带条件
来源：http://vh.huixinmuqiang.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://kd.chemitech.net.cn

[R50] awk 求和
来源：http://vf.9csxet.cn

awk '{s += $2} END {print s}' a.txt
来源：http://th.panjiajie.cn

[R51] 排序去重取前几
来源：http://ap.szsharing.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://my.colortex.cn

[R52] 统计行数
来源：http://hr.hahajie.cn

wc -l a.txt
来源：http://eh.szxytkj.cn

[R53] 查看文件头与实时尾
来源：http://lg.szsharing.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://di.yuexingan06.cn

[R54] 比较两个文件
来源：http://or.shxzukj.cn

diff a.txt b.txt
来源：http://un.huixiangedu.cn

[R55] 压缩与解压
来源：http://bm.colortex.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://vz.shxzskj.cn

[R56] 远程拷贝
来源：http://sy.bookmarksfly.cn

scp file user@host:/path/
来源：http://aa.panjiajie.cn

[R57] 远程执行命令
来源：http://yh.shtwfgs.cn

ssh user@host 'uptime'
来源：http://mx.nszjky.cn

[R58] 下载文件
来源：http://bq.shxzskj.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ib.bjjhwx.cn

[R59] 发 POST JSON
来源：http://ck.nicolike.cn


<!-- 参考信息 -->