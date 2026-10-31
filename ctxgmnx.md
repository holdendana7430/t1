代发 wailian999

SELECT * FROM users;
来源：http://uc.521024.cn

[Q16] 查询指定列
来源：http://qf.yuntaijiaju.cn

SELECT id, name FROM users;
来源：http://di.shxzukj.cn

[Q17] 条件查询
来源：http://mq.gzmigu.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://cb.shxzukj.cn

[Q18] 模糊匹配
来源：http://rq.jianghongdianzi.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.shtwfgs.cn

[Q19] 范围查询
来源：http://aq.jctech888.com.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://zp.szsharing.cn

[Q20] IN 列表
来源：http://br.nicolike.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://uu.hnjuh.cn

[Q21] 空值判断
来源：http://od.yuexingan06.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://na.bjjhwx.cn

[Q22] 排序
来源：http://br.shtwfgs.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ij.szsharing.cn

[Q23] 分页
来源：http://pw.hnjuh.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://xt.bjjhwx.cn

[Q24] 去重
来源：http://df.hahajie.cn

SELECT DISTINCT city FROM users;
来源：http://ou.huixiangedu.cn

[Q25] 只取前 N 条
来源：http://vb.szxytkj.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://dt.huanxung.cn

[Q26] 计数
来源：http://yx.newstarts.cn

SELECT COUNT(*) FROM users;
来源：http://fd.bookmarksfly.cn

[Q27] 条件计数
来源：http://ch.huixiangedu.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://jd.yuexingan06.cn

[Q28] 求和与平均
来源：http://fo.colortex.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://sx.muxihuayi.cn

[Q29] 最大最小值
来源：http://av.hnjuh.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://wm.jctech888.com.cn

[Q30] 分组统计
来源：http://wn.shxzukj.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://rq.huixinmuqiang.cn

[Q31] 分组后过滤
来源：http://kp.panjiajie.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://cc.9csxet.cn

[Q32] 分组拼接字符串
来源：http://uo.9csxet.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://qh.chemitech.net.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://oo.panjiajie.cn

[Q33] 多列分组
来源：http://na.colortex.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://yn.bjjhwx.cn

[Q34] 每组取第一条
来源：http://zp.yuntaijiaju.cn

SELECT * FROM (
来源：http://yv.bookmarksfly.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://oc.9csxet.cn

) t WHERE rn = 1;
来源：http://zm.szxytkj.cn

[Q35] 内连接
来源：http://kf.gzmigu.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://tq.bjjhwx.cn

[Q36] 左连接
来源：http://fv.521024.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://jf.bjjhwx.cn

[Q37] 右连接
来源：http://gy.chemitech.net.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://gq.asd995.cn

[Q38] 全外连接（PostgreSQL）
来源：http://ea.newstarts.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://vp.yuntaijiaju.cn

[Q39] 自连接（查上下级）
来源：http://ev.panjiajie.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://qz.lnxyls.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://qr.shxzskj.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://kv.yuntaijiaju.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://xr.szxytkj.cn

[Q41] 多表连接
来源：http://gz.lnxyls.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://op.muxihuayi.cn

JOIN users u ON u.id = o.user_id
来源：http://my.yuntaijiaju.cn

JOIN products p ON p.id = o.product_id;
来源：http://in.hahajie.cn

[Q42] 连接条件附加过滤
来源：http://uc.szxytkj.cn

SELECT u.name, o.amount FROM users u
来源：http://pl.bookmarksfly.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ec.jctech888.com.cn

[Q43] 标量子查询
来源：http://gg.hnjuh.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://bw.hahajie.cn

[Q44] IN 子查询
来源：http://ab.yuntaijiaju.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://yb.muxihuayi.cn

[Q45] EXISTS 判断存在
来源：http://dq.szsharing.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://qd.lnxyls.cn

[Q46] NOT EXISTS 判断不存在
来源：http://fv.muxihuayi.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://tv.bookmarksfly.cn

[Q47] 与平均值比较
来源：http://jn.bjjhwx.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ph.lnxyls.cn

[Q48] CTE 公用表表达式
来源：http://lp.huixinmuqiang.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://jz.bjjhwx.cn

SELECT * FROM t WHERE c > 5;
来源：http://on.haigaiapp.cn

[Q49] 更新单行
来源：http://io.huixinmuqiang.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ph.panjiajie.cn

[Q50] 批量更新
来源：http://ba.9csxet.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://gz.colortex.cn

[Q51] 用子查询更新
来源：http://nr.yuexingan06.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://aj.lnxyls.cn

[Q52] 删除指定行
来源：http://yo.521024.cn

DELETE FROM users WHERE id = 10;
来源：http://mf.szsharing.cn

[Q53] 按条件删除
来源：http://wq.panjiajie.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mo.szsharing.cn

[Q54] 清空表
来源：http://io.yuexingan06.cn

TRUNCATE TABLE logs;
来源：http://ru.bjjhwx.cn

[Q55] 排名（并列占位）
来源：http://ex.panjiajie.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://dm.bjjhwx.cn

[Q56] 密集排名（并列不占位）
来源：http://hx.huanxung.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://zn.jianghongdianzi.cn

[Q57] 行号
来源：http://im.jctech888.com.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://gv.yuntaijiaju.cn

[Q58] 累计求和
来源：http://rw.huixinmuqiang.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://id.shxzskj.cn

[Q59] 分组内累计
来源：http://lj.hnjuh.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ds.huanxung.cn

[Q60] 取上一行 / 下一行
来源：http://tf.chemitech.net.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ya.nszjky.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://am.521024.cn

[Q61] 移动平均
来源：http://jn.yuexingan06.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://go.jctech888.com.cn

[Q62] 分组占比
来源：http://pw.jctech888.com.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://pu.haigaiapp.cn

[Q63] 开启事务
来源：http://bz.newstarts.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://kc.yuntaijiaju.cn

[Q64] 提交事务
来源：http://vl.panjiajie.cn

COMMIT;
来源：http://vz.asd995.cn

[Q65] 回滚事务
来源：http://wh.bookmarksfly.cn

ROLLBACK;
来源：http://od.jctech888.com.cn

[Q66] 行锁查询
来源：http://az.panjiajie.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ow.nicolike.cn

[Q67] 设置隔离级别
来源：http://hk.chemitech.net.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://zf.yuntaijiaju.cn

[Q68] 保存点
来源：http://wu.gzmigu.cn

SAVEPOINT sp1;
来源：http://zs.szxytkj.cn

ROLLBACK TO sp1;
来源：http://ny.9csxet.cn

[Q69] 查看执行计划
来源：http://ho.huixiangedu.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ra.szsharing.cn

[Q70] 更新统计信息
来源：http://yz.bookmarksfly.cn

ANALYZE TABLE users;
来源：http://fk.bookmarksfly.cn

[Q71] 查看建表语句
来源：http://ix.lnxyls.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://bh.newstarts.cn

[Q72] 查看索引
来源：http://lg.hahajie.cn

SHOW INDEX FROM users;
来源：http://qi.yuntaijiaju.cn

[Q73] 查看表状态
来源：http://hx.gzmigu.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://cy.muxihuayi.cn

[Q74] 强制使用索引
来源：http://pt.yuntaijiaju.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://tr.hahajie.cn

[Q75] 日期格式化
来源：http://ef.lnxyls.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://lp.huixiangedu.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://qr.nszjky.cn

[Q76] 按天统计
来源：http://hx.hnjuh.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://zy.gzmigu.cn

[Q77] 时间加减
来源：http://qx.9csxet.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://qk.panjiajie.cn

[Q78] 当前时间
来源：http://ky.521024.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://fj.muxihuayi.cn

[Q79] 字符串拼接
来源：http://ix.szxytkj.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ln.szsharing.cn

[Q80] 字符串截取
来源：http://bp.shxzukj.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://vj.newstarts.cn

[Q81] 字符串替换
来源：http://wi.521024.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ht.huixiangedu.cn

[Q82] 字符长度与字节长度
来源：http://np.jianghongdianzi.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://zi.gzmigu.cn

[Q83] 大小写转换
来源：http://wf.wgjwhj.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wf.yuexingan06.cn

[Q84] 去除首尾空格
来源：http://qr.yuexingan06.cn

SELECT TRIM(name) FROM users;
来源：http://yz.hnjuh.cn

[Q85] 数值取整
来源：http://im.nicolike.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://xt.nszjky.cn

[Q86] 读取 JSON 字段
来源：http://sv.haigaiapp.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://yk.jianghongdianzi.cn

[Q87] JSON 字段做条件
来源：http://sw.szsharing.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://xs.colortex.cn

[Q88] 行转列（条件聚合）
来源：http://wn.asd995.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mp.szsharing.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mt.lnxyls.cn

[Q89] 判断表是否存在
来源：http://ol.nszjky.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mu.shxzskj.cn

[Q90] 生成序号列
来源：http://sq.szxytkj.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://tp.colortex.cn

================================================================================
来源：http://ei.nicolike.cn

R. Bash 专题
来源：http://rq.yuntaijiaju.cn

================================================================================
来源：http://vd.nicolike.cn

[R01] shebang 与严格模式
来源：http://yn.bookmarksfly.cn

#!/usr/bin/env bash
来源：http://kb.newstarts.cn

set -euo pipefail
来源：http://nc.asd995.cn

[R02] 变量赋值与使用
来源：http://ka.haigaiapp.cn

name="Tom"; echo "$name"
来源：http://kb.szxytkj.cn

[R03] 只读变量
来源：http://kf.yuexingan06.cn

readonly PI=3.14
来源：http://xj.shxzskj.cn

[R04] 位置参数
来源：http://ml.panjiajie.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://dq.nicolike.cn

[R05] 参数默认值
来源：http://jd.lnxyls.cn

name="${1:-default}"
来源：http://mt.hnjuh.cn

[R06] 判断命令是否存在
来源：http://jh.hahajie.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://nh.haigaiapp.cn

[R07] if 判断文件
来源：http://gv.yuntaijiaju.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://pn.panjiajie.cn

[R08] 数值比较
来源：http://xe.hnjuh.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://yt.szsharing.cn

[R09] 字符串比较
来源：http://dx.shxzukj.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hp.lnxyls.cn

[R10] 正则匹配
来源：http://yi.bookmarksfly.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ti.muxihuayi.cn

[R11] case 多分支
来源：http://kw.chemitech.net.cn

case "$1" in
来源：http://go.huanxung.cn

start) echo "启动" ;;
来源：http://az.jianghongdianzi.cn

stop)  echo "停止" ;;
来源：http://tc.colortex.cn

*)     echo "未知命令" ;;
来源：http://yf.wgjwhj.cn

esac
来源：http://ac.haigaiapp.cn

[R12] for 遍历文件
来源：http://jt.bookmarksfly.cn

for f in *.txt; do echo "$f"; done
来源：http://jq.9csxet.cn

[R13] for 计数循环
来源：http://fq.chemitech.net.cn

for i in {1..10}; do echo "$i"; done
来源：http://zh.bjjhwx.cn

[R14] C 风格 for
来源：http://go.jctech888.com.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://yk.panjiajie.cn

[R15] while 逐行读文件
来源：http://hc.hnjuh.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://xj.gzmigu.cn

[R16] until 等待条件
来源：http://tc.szsharing.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ei.shtwfgs.cn

[R17] 数组定义与取值
来源：http://ai.wgjwhj.cn

arr=(a b c); echo "${arr[0]}"
来源：http://vu.muxihuayi.cn

[R18] 遍历数组
来源：http://io.huixiangedu.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://dl.szxytkj.cn

[R19] 数组长度
来源：http://zd.newstarts.cn

echo "${#arr[@]}"
来源：http://mt.haigaiapp.cn

[R20] 关联数组（字典）
来源：http://gw.shxzskj.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://xe.bookmarksfly.cn

[R21] 字符串长度
来源：http://ni.hahajie.cn

echo "${#s}"
来源：http://dp.haigaiapp.cn

[R22] 截取子串
来源：http://dm.muxihuayi.cn

echo "${s:0:5}"
来源：http://it.nszjky.cn

[R23] 字符串替换
来源：http://vq.huixiangedu.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ah.shxzskj.cn

[R24] 大小写转换
来源：http://xe.szsharing.cn

echo "${s^^}"; echo "${s,,}"
来源：http://gt.shxzukj.cn

[R25] 去后缀 / 去前缀
来源：http://jw.panjiajie.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://ay.wgjwhj.cn

[R26] 命令替换
来源：http://ao.panjiajie.cn

now=$(date +%F); echo "$now"
来源：http://wk.nszjky.cn

[R27] 算术展开
来源：http://tj.9csxet.cn

echo $((1 + 2 * 3))
来源：http://ol.bjjhwx.cn

[R28] 浮点运算
来源：http://vf.shxzukj.cn

echo "scale=2; 10/3" | bc
来源：http://sn.haigaiapp.cn

[R29] 定义函数
来源：http://jj.huixiangedu.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://zd.colortex.cn

[R30] 函数返回状态码
来源：http://qp.szxytkj.cn

f() { return 0; }; f || echo "失败了"
来源：http://bn.szxytkj.cn

[R31] 局部变量
来源：http://hc.yuexingan06.cn

f() { local x=1; echo "$x"; }
来源：http://pb.haigaiapp.cn

[R32] 参数个数校验
来源：http://td.521024.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://fi.huixinmuqiang.cn

[R33] 捕获错误并提示行号
来源：http://jl.9csxet.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ew.colortex.cn

[R34] 退出时清理
来源：http://rs.szxytkj.cn

trap 'rm -f "$tmp"' EXIT
来源：http://tc.nicolike.cn

[R35] 后台执行并等待
来源：http://bs.szsharing.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://mw.szsharing.cn

[R36] 并发执行多个任务
来源：http://xr.9csxet.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://bs.yuntaijiaju.cn

[R37] 把输出赋给变量
来源：http://mm.yuexingan06.cn

files=$(ls -1)
来源：http://ji.shtwfgs.cn

[R38] 管道串联
来源：http://dt.bjjhwx.cn

cat a.txt | grep -i error | wc -l
来源：http://iw.jianghongdianzi.cn

[R39] 重定向标准输出与错误
来源：http://ba.panjiajie.cn

cmd > out.log 2>&1
来源：http://te.lnxyls.cn

[R40] 追加写日志
来源：http://cf.yuexingan06.cn

echo "log" >> out.log
来源：http://vu.huixinmuqiang.cn

[R41] 丢弃输出
来源：http://pk.bookmarksfly.cn

cmd >/dev/null 2>&1
来源：http://ty.panjiajie.cn

[R42] 输入重定向
来源：http://ln.huanxung.cn

wc -l < a.txt
来源：http://go.panjiajie.cn

[R43] 按名字查找文件
来源：http://pl.szxytkj.cn

find . -name "*.log" -type f
来源：http://dj.huixiangedu.cn

[R44] 按修改时间查找
来源：http://pc.nicolike.cn

find . -mtime -7 -type f
来源：http://vk.haigaiapp.cn

[R45] 批量删除
来源：http://fc.bjjhwx.cn

find . -name "*.tmp" -delete
来源：http://ab.muxihuayi.cn

[R46] 递归替换文件内容
来源：http://cx.gzmigu.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ab.jctech888.com.cn

[R47] sed 单行替换
来源：http://oj.hnjuh.cn

sed -i 's/foo/bar/g' a.txt
来源：http://tb.shtwfgs.cn

[R48] awk 取指定列
来源：http://gv.shxzskj.cn

awk '{print $1, $3}' a.txt
来源：http://wr.huixinmuqiang.cn

[R49] awk 带条件
来源：http://mm.lnxyls.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://vl.huixiangedu.cn

[R50] awk 求和
来源：http://kp.gzmigu.cn

awk '{s += $2} END {print s}' a.txt
来源：http://vp.shxzukj.cn

[R51] 排序去重取前几
来源：http://fd.bookmarksfly.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://qz.szsharing.cn

[R52] 统计行数
来源：http://yo.9csxet.cn

wc -l a.txt
来源：http://pm.shxzskj.cn

[R53] 查看文件头与实时尾
来源：http://hm.hahajie.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://qs.bookmarksfly.cn

[R54] 比较两个文件
来源：http://gm.jctech888.com.cn

diff a.txt b.txt
来源：http://sk.521024.cn

[R55] 压缩与解压
来源：http://os.9csxet.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://vy.gzmigu.cn

[R56] 远程拷贝
来源：http://tu.jctech888.com.cn

scp file user@host:/path/
来源：http://tp.asd995.cn

[R57] 远程执行命令
来源：http://bj.huixinmuqiang.cn

ssh user@host 'uptime'
来源：http://ec.huanxung.cn

[R58] 下载文件
来源：http://gk.huixinmuqiang.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mi.shxzskj.cn

[R59] 发 POST JSON
来源：http://qk.szsharing.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ee.jctech888.com.cn

[R60] 只看 HTTP 状态码
来源：http://og.szsharing.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://vh.szxytkj.cn

[R61] 磁盘占用
来源：http://rw.yuexingan06.cn

df -h;  du -sh *
来源：http://sq.huanxung.cn

[R62] 找最占空间的文件
来源：http://gt.yuexingan06.cn

du -ah . | sort -rh | head -10
来源：http://mh.huixiangedu.cn

[R63] 内存与进程
来源：http://ls.shxzukj.cn

free -h;  ps aux | grep nginx
来源：http://qd.bookmarksfly.cn

[R64] 结束进程
来源：http://zs.szsharing.cn

kill -9 $(pgrep -f app.py)
来源：http://fg.shxzukj.cn

[R65] 查看端口占用
来源：http://bj.szxytkj.cn


<!-- 参考信息 -->