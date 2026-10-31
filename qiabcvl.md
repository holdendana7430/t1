代发 wailian999

SELECT * FROM users;
来源：http://rd.asd995.cn

[Q16] 查询指定列
来源：http://th.jctech888.com.cn

SELECT id, name FROM users;
来源：http://hs.9csxet.cn

[Q17] 条件查询
来源：http://ic.shxzukj.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://zv.huanxung.cn

[Q18] 模糊匹配
来源：http://wu.haigaiapp.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://oe.shxzskj.cn

[Q19] 范围查询
来源：http://nt.yuntaijiaju.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://xb.szsharing.cn

[Q20] IN 列表
来源：http://py.huixinmuqiang.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://nh.szsharing.cn

[Q21] 空值判断
来源：http://yt.szsharing.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://dj.hnjuh.cn

[Q22] 排序
来源：http://ak.huixinmuqiang.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://dc.muxihuayi.cn

[Q23] 分页
来源：http://da.haigaiapp.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://nl.szxytkj.cn

[Q24] 去重
来源：http://ec.huanxung.cn

SELECT DISTINCT city FROM users;
来源：http://dy.asd995.cn

[Q25] 只取前 N 条
来源：http://vr.szsharing.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://yo.huixiangedu.cn

[Q26] 计数
来源：http://xp.bjjhwx.cn

SELECT COUNT(*) FROM users;
来源：http://tm.panjiajie.cn

[Q27] 条件计数
来源：http://lj.szsharing.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://uy.hahajie.cn

[Q28] 求和与平均
来源：http://co.wgjwhj.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://ka.wgjwhj.cn

[Q29] 最大最小值
来源：http://nm.newstarts.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://lq.jctech888.com.cn

[Q30] 分组统计
来源：http://ya.bjjhwx.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://tb.szsharing.cn

[Q31] 分组后过滤
来源：http://dd.panjiajie.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://rz.haigaiapp.cn

[Q32] 分组拼接字符串
来源：http://qn.shxzskj.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://rt.nicolike.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ru.nicolike.cn

[Q33] 多列分组
来源：http://gu.bookmarksfly.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ru.shtwfgs.cn

[Q34] 每组取第一条
来源：http://iu.szxytkj.cn

SELECT * FROM (
来源：http://lq.chemitech.net.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://va.9csxet.cn

) t WHERE rn = 1;
来源：http://gt.shtwfgs.cn

[Q35] 内连接
来源：http://ey.yuexingan06.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://jk.shxzukj.cn

[Q36] 左连接
来源：http://my.huixiangedu.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://st.huanxung.cn

[Q37] 右连接
来源：http://oh.colortex.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://vh.hahajie.cn

[Q38] 全外连接（PostgreSQL）
来源：http://zn.muxihuayi.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://uc.huanxung.cn

[Q39] 自连接（查上下级）
来源：http://ql.gzmigu.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://it.nicolike.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wp.bjjhwx.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://fm.gzmigu.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://xr.jctech888.com.cn

[Q41] 多表连接
来源：http://we.shtwfgs.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://du.yuexingan06.cn

JOIN users u ON u.id = o.user_id
来源：http://yq.nszjky.cn

JOIN products p ON p.id = o.product_id;
来源：http://ir.colortex.cn

[Q42] 连接条件附加过滤
来源：http://wm.colortex.cn

SELECT u.name, o.amount FROM users u
来源：http://kf.bookmarksfly.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://vv.wgjwhj.cn

[Q43] 标量子查询
来源：http://qa.jctech888.com.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://yr.szsharing.cn

[Q44] IN 子查询
来源：http://xu.nszjky.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://xj.521024.cn

[Q45] EXISTS 判断存在
来源：http://xv.huixiangedu.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mq.shxzukj.cn

[Q46] NOT EXISTS 判断不存在
来源：http://cr.haigaiapp.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ps.nszjky.cn

[Q47] 与平均值比较
来源：http://ka.colortex.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://dw.jctech888.com.cn

[Q48] CTE 公用表表达式
来源：http://gi.yuntaijiaju.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://cz.shtwfgs.cn

SELECT * FROM t WHERE c > 5;
来源：http://yl.nicolike.cn

[Q49] 更新单行
来源：http://wj.huixiangedu.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://tk.newstarts.cn

[Q50] 批量更新
来源：http://eg.asd995.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mc.szxytkj.cn

[Q51] 用子查询更新
来源：http://dl.haigaiapp.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://ks.jianghongdianzi.cn

[Q52] 删除指定行
来源：http://ip.hnjuh.cn

DELETE FROM users WHERE id = 10;
来源：http://ya.huanxung.cn

[Q53] 按条件删除
来源：http://yk.huixiangedu.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://jt.nszjky.cn

[Q54] 清空表
来源：http://vv.huixiangedu.cn

TRUNCATE TABLE logs;
来源：http://az.lnxyls.cn

[Q55] 排名（并列占位）
来源：http://me.jctech888.com.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://in.yuntaijiaju.cn

[Q56] 密集排名（并列不占位）
来源：http://sc.hahajie.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ua.huixiangedu.cn

[Q57] 行号
来源：http://zg.lnxyls.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://qa.gzmigu.cn

[Q58] 累计求和
来源：http://zy.shxzskj.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wz.gzmigu.cn

[Q59] 分组内累计
来源：http://dr.muxihuayi.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://td.jctech888.com.cn

[Q60] 取上一行 / 下一行
来源：http://va.muxihuayi.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://gu.wgjwhj.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://oy.shtwfgs.cn

[Q61] 移动平均
来源：http://oj.bjjhwx.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://lp.jctech888.com.cn

[Q62] 分组占比
来源：http://vx.lnxyls.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ro.haigaiapp.cn

[Q63] 开启事务
来源：http://cx.shxzukj.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://ql.yuntaijiaju.cn

[Q64] 提交事务
来源：http://fp.9csxet.cn

COMMIT;
来源：http://sm.newstarts.cn

[Q65] 回滚事务
来源：http://et.huixiangedu.cn

ROLLBACK;
来源：http://em.hahajie.cn

[Q66] 行锁查询
来源：http://vr.shxzskj.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://kl.yuexingan06.cn

[Q67] 设置隔离级别
来源：http://kf.bjjhwx.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://yv.panjiajie.cn

[Q68] 保存点
来源：http://hd.shxzukj.cn

SAVEPOINT sp1;
来源：http://te.lnxyls.cn

ROLLBACK TO sp1;
来源：http://dc.huixiangedu.cn

[Q69] 查看执行计划
来源：http://rj.huixiangedu.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://us.521024.cn

[Q70] 更新统计信息
来源：http://ic.521024.cn

ANALYZE TABLE users;
来源：http://oy.huanxung.cn

[Q71] 查看建表语句
来源：http://st.hnjuh.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://vq.nszjky.cn

[Q72] 查看索引
来源：http://qf.panjiajie.cn

SHOW INDEX FROM users;
来源：http://pc.szxytkj.cn

[Q73] 查看表状态
来源：http://rm.jianghongdianzi.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://iu.nszjky.cn

[Q74] 强制使用索引
来源：http://rx.wgjwhj.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://my.szsharing.cn

[Q75] 日期格式化
来源：http://uw.chemitech.net.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://gu.shxzskj.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://yj.yuexingan06.cn

[Q76] 按天统计
来源：http://ml.bjjhwx.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://no.hnjuh.cn

[Q77] 时间加减
来源：http://dh.yuntaijiaju.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://az.shtwfgs.cn

[Q78] 当前时间
来源：http://tv.yuntaijiaju.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://kp.shxzukj.cn

[Q79] 字符串拼接
来源：http://re.huixiangedu.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://jn.yuexingan06.cn

[Q80] 字符串截取
来源：http://kb.jianghongdianzi.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://kl.wgjwhj.cn

[Q81] 字符串替换
来源：http://js.wgjwhj.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://em.gzmigu.cn

[Q82] 字符长度与字节长度
来源：http://cj.huixinmuqiang.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://np.shxzukj.cn

[Q83] 大小写转换
来源：http://bo.bjjhwx.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://qp.haigaiapp.cn

[Q84] 去除首尾空格
来源：http://if.nicolike.cn

SELECT TRIM(name) FROM users;
来源：http://si.szsharing.cn

[Q85] 数值取整
来源：http://fb.yuexingan06.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://gb.shxzukj.cn

[Q86] 读取 JSON 字段
来源：http://yo.hahajie.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://yt.nicolike.cn

[Q87] JSON 字段做条件
来源：http://ns.shtwfgs.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://im.gzmigu.cn

[Q88] 行转列（条件聚合）
来源：http://lp.hnjuh.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://cx.asd995.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://kj.szsharing.cn

[Q89] 判断表是否存在
来源：http://kj.shxzskj.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://lt.shxzukj.cn

[Q90] 生成序号列
来源：http://mv.newstarts.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://fs.huixiangedu.cn

================================================================================
来源：http://lq.szsharing.cn

R. Bash 专题
来源：http://wd.nszjky.cn

================================================================================
来源：http://vm.hahajie.cn

[R01] shebang 与严格模式
来源：http://bs.shxzukj.cn

#!/usr/bin/env bash
来源：http://cb.shtwfgs.cn

set -euo pipefail
来源：http://wc.yuexingan06.cn

[R02] 变量赋值与使用
来源：http://tz.chemitech.net.cn

name="Tom"; echo "$name"
来源：http://ge.jctech888.com.cn

[R03] 只读变量
来源：http://xi.nicolike.cn

readonly PI=3.14
来源：http://ez.shxzskj.cn

[R04] 位置参数
来源：http://yb.hahajie.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ds.bjjhwx.cn

[R05] 参数默认值
来源：http://bi.shtwfgs.cn

name="${1:-default}"
来源：http://bv.521024.cn

[R06] 判断命令是否存在
来源：http://mt.huixinmuqiang.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://na.hnjuh.cn

[R07] if 判断文件
来源：http://ce.szsharing.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://vu.muxihuayi.cn

[R08] 数值比较
来源：http://vm.huanxung.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://uk.jianghongdianzi.cn

[R09] 字符串比较
来源：http://hc.huixiangedu.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://rk.yuntaijiaju.cn

[R10] 正则匹配
来源：http://gq.huixiangedu.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://gn.hahajie.cn

[R11] case 多分支
来源：http://nr.wgjwhj.cn

case "$1" in
来源：http://it.9csxet.cn

start) echo "启动" ;;
来源：http://ip.yuntaijiaju.cn

stop)  echo "停止" ;;
来源：http://mq.lnxyls.cn

*)     echo "未知命令" ;;
来源：http://wp.huanxung.cn

esac
来源：http://kb.yuntaijiaju.cn

[R12] for 遍历文件
来源：http://ap.panjiajie.cn

for f in *.txt; do echo "$f"; done
来源：http://iz.nicolike.cn

[R13] for 计数循环
来源：http://oq.lnxyls.cn

for i in {1..10}; do echo "$i"; done
来源：http://tl.yuexingan06.cn

[R14] C 风格 for
来源：http://ao.yuexingan06.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ls.lnxyls.cn

[R15] while 逐行读文件
来源：http://gc.wgjwhj.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://qm.panjiajie.cn

[R16] until 等待条件
来源：http://ja.muxihuayi.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hv.shxzukj.cn

[R17] 数组定义与取值
来源：http://qe.chemitech.net.cn

arr=(a b c); echo "${arr[0]}"
来源：http://ym.9csxet.cn

[R18] 遍历数组
来源：http://hj.hnjuh.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://lv.yuntaijiaju.cn

[R19] 数组长度
来源：http://vw.hahajie.cn

echo "${#arr[@]}"
来源：http://bu.yuntaijiaju.cn

[R20] 关联数组（字典）
来源：http://ei.huanxung.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://yz.bjjhwx.cn

[R21] 字符串长度
来源：http://hb.szsharing.cn

echo "${#s}"
来源：http://vw.colortex.cn

[R22] 截取子串
来源：http://qr.asd995.cn

echo "${s:0:5}"
来源：http://yq.colortex.cn

[R23] 字符串替换
来源：http://lm.colortex.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://in.shxzskj.cn

[R24] 大小写转换
来源：http://lu.yuexingan06.cn

echo "${s^^}"; echo "${s,,}"
来源：http://nl.nicolike.cn

[R25] 去后缀 / 去前缀
来源：http://ge.hahajie.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://rw.nszjky.cn

[R26] 命令替换
来源：http://fj.bookmarksfly.cn

now=$(date +%F); echo "$now"
来源：http://ru.shxzukj.cn

[R27] 算术展开
来源：http://gj.yuexingan06.cn

echo $((1 + 2 * 3))
来源：http://oa.panjiajie.cn

[R28] 浮点运算
来源：http://yc.nicolike.cn

echo "scale=2; 10/3" | bc
来源：http://wd.nicolike.cn

[R29] 定义函数
来源：http://zt.shxzskj.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://dt.szsharing.cn

[R30] 函数返回状态码
来源：http://sf.huixinmuqiang.cn

f() { return 0; }; f || echo "失败了"
来源：http://py.bjjhwx.cn

[R31] 局部变量
来源：http://iu.huixinmuqiang.cn

f() { local x=1; echo "$x"; }
来源：http://wm.wgjwhj.cn

[R32] 参数个数校验
来源：http://km.chemitech.net.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://tw.haigaiapp.cn

[R33] 捕获错误并提示行号
来源：http://ct.panjiajie.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://bf.shxzukj.cn

[R34] 退出时清理
来源：http://or.yuntaijiaju.cn

trap 'rm -f "$tmp"' EXIT
来源：http://kl.hnjuh.cn

[R35] 后台执行并等待
来源：http://tq.shxzskj.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://bi.521024.cn

[R36] 并发执行多个任务
来源：http://ce.newstarts.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://qi.521024.cn

[R37] 把输出赋给变量
来源：http://fh.muxihuayi.cn

files=$(ls -1)
来源：http://on.szsharing.cn

[R38] 管道串联
来源：http://dq.jianghongdianzi.cn

cat a.txt | grep -i error | wc -l
来源：http://hu.muxihuayi.cn

[R39] 重定向标准输出与错误
来源：http://cq.huanxung.cn

cmd > out.log 2>&1
来源：http://gs.colortex.cn

[R40] 追加写日志
来源：http://ua.hahajie.cn

echo "log" >> out.log
来源：http://ap.huanxung.cn

[R41] 丢弃输出
来源：http://ad.bjjhwx.cn

cmd >/dev/null 2>&1
来源：http://iw.huixinmuqiang.cn

[R42] 输入重定向
来源：http://yu.nicolike.cn

wc -l < a.txt
来源：http://os.shtwfgs.cn

[R43] 按名字查找文件
来源：http://kv.shtwfgs.cn

find . -name "*.log" -type f
来源：http://un.gzmigu.cn

[R44] 按修改时间查找
来源：http://pd.shxzskj.cn

find . -mtime -7 -type f
来源：http://eg.jianghongdianzi.cn

[R45] 批量删除
来源：http://do.hahajie.cn

find . -name "*.tmp" -delete
来源：http://mt.chemitech.net.cn

[R46] 递归替换文件内容
来源：http://ow.shtwfgs.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://eq.huixinmuqiang.cn

[R47] sed 单行替换
来源：http://by.lnxyls.cn

sed -i 's/foo/bar/g' a.txt
来源：http://gr.newstarts.cn

[R48] awk 取指定列
来源：http://cz.chemitech.net.cn

awk '{print $1, $3}' a.txt
来源：http://rh.panjiajie.cn

[R49] awk 带条件
来源：http://xb.yuexingan06.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ku.yuntaijiaju.cn

[R50] awk 求和
来源：http://bh.hnjuh.cn

awk '{s += $2} END {print s}' a.txt
来源：http://wa.lnxyls.cn

[R51] 排序去重取前几
来源：http://lc.hahajie.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://dj.newstarts.cn

[R52] 统计行数
来源：http://dg.huixiangedu.cn

wc -l a.txt
来源：http://su.wgjwhj.cn

[R53] 查看文件头与实时尾
来源：http://zx.nszjky.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://yc.shtwfgs.cn

[R54] 比较两个文件
来源：http://ih.yuexingan06.cn

diff a.txt b.txt
来源：http://jm.nszjky.cn

[R55] 压缩与解压
来源：http://af.asd995.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://pw.yuexingan06.cn

[R56] 远程拷贝
来源：http://pw.9csxet.cn

scp file user@host:/path/
来源：http://xw.wgjwhj.cn

[R57] 远程执行命令
来源：http://xg.lnxyls.cn

ssh user@host 'uptime'
来源：http://df.huixinmuqiang.cn

[R58] 下载文件
来源：http://al.muxihuayi.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://rm.huixinmuqiang.cn

[R59] 发 POST JSON
来源：http://md.szxytkj.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mh.asd995.cn

[R60] 只看 HTTP 状态码
来源：http://yc.jctech888.com.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://yr.bjjhwx.cn

[R61] 磁盘占用
来源：http://px.nszjky.cn

df -h;  du -sh *
来源：http://we.shtwfgs.cn

[R62] 找最占空间的文件
来源：http://ss.9csxet.cn

du -ah . | sort -rh | head -10
来源：http://nz.bjjhwx.cn

[R63] 内存与进程
来源：http://vr.nszjky.cn

free -h;  ps aux | grep nginx
来源：http://jr.bjjhwx.cn

[R64] 结束进程
来源：http://rk.bjjhwx.cn

kill -9 $(pgrep -f app.py)
来源：http://ej.9csxet.cn

[R65] 查看端口占用
来源：http://ss.huixinmuqiang.cn


<!-- 参考信息 -->