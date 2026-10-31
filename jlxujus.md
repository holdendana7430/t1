代发 wailian999

SELECT * FROM users;
来源：http://fe.shxzukj.cn

[Q16] 查询指定列
来源：http://vp.haigaiapp.cn

SELECT id, name FROM users;
来源：http://eu.9csxet.cn

[Q17] 条件查询
来源：http://ih.chemitech.net.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://zd.wgjwhj.cn

[Q18] 模糊匹配
来源：http://sv.szxytkj.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ix.bookmarksfly.cn

[Q19] 范围查询
来源：http://or.szxytkj.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ls.lnxyls.cn

[Q20] IN 列表
来源：http://po.nszjky.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://zv.gzmigu.cn

[Q21] 空值判断
来源：http://fj.nicolike.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://ua.9csxet.cn

[Q22] 排序
来源：http://lg.hahajie.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://uz.colortex.cn

[Q23] 分页
来源：http://hl.jctech888.com.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://dv.newstarts.cn

[Q24] 去重
来源：http://xs.wgjwhj.cn

SELECT DISTINCT city FROM users;
来源：http://gk.huixinmuqiang.cn

[Q25] 只取前 N 条
来源：http://ah.yuntaijiaju.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://vk.jianghongdianzi.cn

[Q26] 计数
来源：http://wm.asd995.cn

SELECT COUNT(*) FROM users;
来源：http://pk.hnjuh.cn

[Q27] 条件计数
来源：http://ga.lnxyls.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://yr.huanxung.cn

[Q28] 求和与平均
来源：http://ms.9csxet.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://xh.shxzskj.cn

[Q29] 最大最小值
来源：http://qw.9csxet.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://ug.asd995.cn

[Q30] 分组统计
来源：http://ua.nicolike.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://rc.szxytkj.cn

[Q31] 分组后过滤
来源：http://wd.szsharing.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://bi.gzmigu.cn

[Q32] 分组拼接字符串
来源：http://es.gzmigu.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://zy.huixinmuqiang.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://cf.521024.cn

[Q33] 多列分组
来源：http://ew.huixinmuqiang.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://pf.shxzukj.cn

[Q34] 每组取第一条
来源：http://sa.521024.cn

SELECT * FROM (
来源：http://it.shxzskj.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://no.muxihuayi.cn

) t WHERE rn = 1;
来源：http://bf.yuntaijiaju.cn

[Q35] 内连接
来源：http://jx.muxihuayi.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ld.chemitech.net.cn

[Q36] 左连接
来源：http://ha.wgjwhj.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://vq.yuntaijiaju.cn

[Q37] 右连接
来源：http://mb.muxihuayi.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://vm.szxytkj.cn

[Q38] 全外连接（PostgreSQL）
来源：http://vu.huanxung.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://kj.shxzukj.cn

[Q39] 自连接（查上下级）
来源：http://lm.chemitech.net.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://fr.jctech888.com.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://kv.szsharing.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://sk.nszjky.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://sv.szsharing.cn

[Q41] 多表连接
来源：http://jc.9csxet.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://zo.szxytkj.cn

JOIN users u ON u.id = o.user_id
来源：http://mx.asd995.cn

JOIN products p ON p.id = o.product_id;
来源：http://ee.yuexingan06.cn

[Q42] 连接条件附加过滤
来源：http://lp.szsharing.cn

SELECT u.name, o.amount FROM users u
来源：http://ed.newstarts.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://tz.szxytkj.cn

[Q43] 标量子查询
来源：http://qb.shxzskj.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://cj.asd995.cn

[Q44] IN 子查询
来源：http://az.shxzskj.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://nt.chemitech.net.cn

[Q45] EXISTS 判断存在
来源：http://br.szxytkj.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://pn.9csxet.cn

[Q46] NOT EXISTS 判断不存在
来源：http://lq.wgjwhj.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://zk.panjiajie.cn

[Q47] 与平均值比较
来源：http://id.nszjky.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://xw.szsharing.cn

[Q48] CTE 公用表表达式
来源：http://pf.9csxet.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ep.szxytkj.cn

SELECT * FROM t WHERE c > 5;
来源：http://uz.shxzukj.cn

[Q49] 更新单行
来源：http://hq.9csxet.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://bg.panjiajie.cn

[Q50] 批量更新
来源：http://cg.nszjky.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wu.bookmarksfly.cn

[Q51] 用子查询更新
来源：http://zj.wgjwhj.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://xp.jctech888.com.cn

[Q52] 删除指定行
来源：http://ey.gzmigu.cn

DELETE FROM users WHERE id = 10;
来源：http://th.jianghongdianzi.cn

[Q53] 按条件删除
来源：http://gm.jctech888.com.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://zi.haigaiapp.cn

[Q54] 清空表
来源：http://cj.huixinmuqiang.cn

TRUNCATE TABLE logs;
来源：http://sv.jianghongdianzi.cn

[Q55] 排名（并列占位）
来源：http://po.yuexingan06.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://aj.chemitech.net.cn

[Q56] 密集排名（并列不占位）
来源：http://oq.shxzskj.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ar.shxzskj.cn

[Q57] 行号
来源：http://mx.chemitech.net.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://dw.shxzskj.cn

[Q58] 累计求和
来源：http://vs.521024.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://lu.nszjky.cn

[Q59] 分组内累计
来源：http://sw.panjiajie.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://qo.nicolike.cn

[Q60] 取上一行 / 下一行
来源：http://ww.521024.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ny.yuntaijiaju.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wg.huixiangedu.cn

[Q61] 移动平均
来源：http://wx.9csxet.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://gm.asd995.cn

[Q62] 分组占比
来源：http://ms.wgjwhj.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://jr.nicolike.cn

[Q63] 开启事务
来源：http://tu.lnxyls.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://sz.521024.cn

[Q64] 提交事务
来源：http://yo.hahajie.cn

COMMIT;
来源：http://ss.huixiangedu.cn

[Q65] 回滚事务
来源：http://jt.nicolike.cn

ROLLBACK;
来源：http://mw.huixinmuqiang.cn

[Q66] 行锁查询
来源：http://od.yuntaijiaju.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://zc.gzmigu.cn

[Q67] 设置隔离级别
来源：http://pa.chemitech.net.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://uc.huixiangedu.cn

[Q68] 保存点
来源：http://rk.huixinmuqiang.cn

SAVEPOINT sp1;
来源：http://de.huixiangedu.cn

ROLLBACK TO sp1;
来源：http://op.gzmigu.cn

[Q69] 查看执行计划
来源：http://iu.haigaiapp.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ex.huixiangedu.cn

[Q70] 更新统计信息
来源：http://ib.wgjwhj.cn

ANALYZE TABLE users;
来源：http://wt.bjjhwx.cn

[Q71] 查看建表语句
来源：http://hw.lnxyls.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ot.yuexingan06.cn

[Q72] 查看索引
来源：http://ym.shxzskj.cn

SHOW INDEX FROM users;
来源：http://pv.shtwfgs.cn

[Q73] 查看表状态
来源：http://si.huixinmuqiang.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://qr.bjjhwx.cn

[Q74] 强制使用索引
来源：http://cx.wgjwhj.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://th.shtwfgs.cn

[Q75] 日期格式化
来源：http://jj.hahajie.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://bh.jctech888.com.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://qj.jianghongdianzi.cn

[Q76] 按天统计
来源：http://rm.bookmarksfly.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://bz.jianghongdianzi.cn

[Q77] 时间加减
来源：http://ej.yuexingan06.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://oz.jianghongdianzi.cn

[Q78] 当前时间
来源：http://qw.szsharing.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ca.muxihuayi.cn

[Q79] 字符串拼接
来源：http://wt.nszjky.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://up.huanxung.cn

[Q80] 字符串截取
来源：http://hv.wgjwhj.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://zf.jianghongdianzi.cn

[Q81] 字符串替换
来源：http://kv.huixinmuqiang.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://yx.chemitech.net.cn

[Q82] 字符长度与字节长度
来源：http://tr.szxytkj.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://xq.9csxet.cn

[Q83] 大小写转换
来源：http://jm.shxzskj.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://bo.yuntaijiaju.cn

[Q84] 去除首尾空格
来源：http://fl.shtwfgs.cn

SELECT TRIM(name) FROM users;
来源：http://du.haigaiapp.cn

[Q85] 数值取整
来源：http://jk.jctech888.com.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ch.newstarts.cn

[Q86] 读取 JSON 字段
来源：http://mb.shtwfgs.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://lt.szsharing.cn

[Q87] JSON 字段做条件
来源：http://ib.szsharing.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://yh.9csxet.cn

[Q88] 行转列（条件聚合）
来源：http://nh.lnxyls.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://jh.shtwfgs.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://id.shxzskj.cn

[Q89] 判断表是否存在
来源：http://hn.lnxyls.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://oy.asd995.cn

[Q90] 生成序号列
来源：http://im.wgjwhj.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ru.jctech888.com.cn

================================================================================
来源：http://hp.chemitech.net.cn

R. Bash 专题
来源：http://ac.panjiajie.cn

================================================================================
来源：http://ng.shxzukj.cn

[R01] shebang 与严格模式
来源：http://ob.newstarts.cn

#!/usr/bin/env bash
来源：http://my.gzmigu.cn

set -euo pipefail
来源：http://ne.hahajie.cn

[R02] 变量赋值与使用
来源：http://yc.jianghongdianzi.cn

name="Tom"; echo "$name"
来源：http://xy.yuexingan06.cn

[R03] 只读变量
来源：http://ee.muxihuayi.cn

readonly PI=3.14
来源：http://fr.nicolike.cn

[R04] 位置参数
来源：http://le.szxytkj.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wf.newstarts.cn

[R05] 参数默认值
来源：http://hw.521024.cn

name="${1:-default}"
来源：http://ge.colortex.cn

[R06] 判断命令是否存在
来源：http://ls.bookmarksfly.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://kd.hahajie.cn

[R07] if 判断文件
来源：http://rs.gzmigu.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://th.521024.cn

[R08] 数值比较
来源：http://bm.nicolike.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://oh.muxihuayi.cn

[R09] 字符串比较
来源：http://ws.haigaiapp.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://yg.wgjwhj.cn

[R10] 正则匹配
来源：http://tz.bookmarksfly.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hs.huixiangedu.cn

[R11] case 多分支
来源：http://tk.hnjuh.cn

case "$1" in
来源：http://cx.yuntaijiaju.cn

start) echo "启动" ;;
来源：http://zy.huixiangedu.cn

stop)  echo "停止" ;;
来源：http://zj.huanxung.cn

*)     echo "未知命令" ;;
来源：http://jl.hahajie.cn

esac
来源：http://un.huixinmuqiang.cn

[R12] for 遍历文件
来源：http://vc.521024.cn

for f in *.txt; do echo "$f"; done
来源：http://sw.szxytkj.cn

[R13] for 计数循环
来源：http://zi.bookmarksfly.cn

for i in {1..10}; do echo "$i"; done
来源：http://az.lnxyls.cn

[R14] C 风格 for
来源：http://yp.nicolike.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://tt.nszjky.cn

[R15] while 逐行读文件
来源：http://ai.jianghongdianzi.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://fo.521024.cn

[R16] until 等待条件
来源：http://vv.nszjky.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://bu.shtwfgs.cn

[R17] 数组定义与取值
来源：http://ht.asd995.cn

arr=(a b c); echo "${arr[0]}"
来源：http://bm.lnxyls.cn

[R18] 遍历数组
来源：http://kt.huanxung.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hd.newstarts.cn

[R19] 数组长度
来源：http://eb.asd995.cn

echo "${#arr[@]}"
来源：http://cx.huanxung.cn

[R20] 关联数组（字典）
来源：http://rc.muxihuayi.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wn.yuexingan06.cn

[R21] 字符串长度
来源：http://ot.bjjhwx.cn

echo "${#s}"
来源：http://gs.yuexingan06.cn

[R22] 截取子串
来源：http://ez.chemitech.net.cn

echo "${s:0:5}"
来源：http://xk.yuexingan06.cn

[R23] 字符串替换
来源：http://ac.huixiangedu.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://tv.hahajie.cn

[R24] 大小写转换
来源：http://zx.huixinmuqiang.cn

echo "${s^^}"; echo "${s,,}"
来源：http://id.shxzskj.cn

[R25] 去后缀 / 去前缀
来源：http://st.hnjuh.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://ec.yuntaijiaju.cn

[R26] 命令替换
来源：http://ss.szxytkj.cn

now=$(date +%F); echo "$now"
来源：http://do.lnxyls.cn

[R27] 算术展开
来源：http://yv.shtwfgs.cn

echo $((1 + 2 * 3))
来源：http://jc.shxzukj.cn

[R28] 浮点运算
来源：http://kl.hnjuh.cn

echo "scale=2; 10/3" | bc
来源：http://fk.asd995.cn

[R29] 定义函数
来源：http://lr.panjiajie.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://zi.nicolike.cn

[R30] 函数返回状态码
来源：http://kt.9csxet.cn

f() { return 0; }; f || echo "失败了"
来源：http://nq.huixinmuqiang.cn

[R31] 局部变量
来源：http://ey.shxzskj.cn

f() { local x=1; echo "$x"; }
来源：http://pd.szsharing.cn

[R32] 参数个数校验
来源：http://ah.bookmarksfly.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://in.huixiangedu.cn

[R33] 捕获错误并提示行号
来源：http://la.shxzukj.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://qj.huixiangedu.cn

[R34] 退出时清理
来源：http://mm.szsharing.cn

trap 'rm -f "$tmp"' EXIT
来源：http://go.bjjhwx.cn

[R35] 后台执行并等待
来源：http://iu.haigaiapp.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://nv.bjjhwx.cn

[R36] 并发执行多个任务
来源：http://ha.huanxung.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://pc.shxzskj.cn

[R37] 把输出赋给变量
来源：http://hs.521024.cn

files=$(ls -1)
来源：http://zn.521024.cn

[R38] 管道串联
来源：http://fh.jctech888.com.cn

cat a.txt | grep -i error | wc -l
来源：http://mi.szxytkj.cn

[R39] 重定向标准输出与错误
来源：http://fs.szxytkj.cn

cmd > out.log 2>&1
来源：http://dk.colortex.cn

[R40] 追加写日志
来源：http://et.jianghongdianzi.cn

echo "log" >> out.log
来源：http://ge.szsharing.cn

[R41] 丢弃输出
来源：http://dm.yuntaijiaju.cn

cmd >/dev/null 2>&1
来源：http://hj.wgjwhj.cn

[R42] 输入重定向
来源：http://jz.chemitech.net.cn

wc -l < a.txt
来源：http://ec.colortex.cn

[R43] 按名字查找文件
来源：http://ot.nszjky.cn

find . -name "*.log" -type f
来源：http://lz.yuntaijiaju.cn

[R44] 按修改时间查找
来源：http://ah.hahajie.cn

find . -mtime -7 -type f
来源：http://cl.wgjwhj.cn

[R45] 批量删除
来源：http://ma.jctech888.com.cn

find . -name "*.tmp" -delete
来源：http://ql.hnjuh.cn

[R46] 递归替换文件内容
来源：http://oh.jctech888.com.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://sd.bjjhwx.cn

[R47] sed 单行替换
来源：http://wb.hnjuh.cn

sed -i 's/foo/bar/g' a.txt
来源：http://hs.lnxyls.cn

[R48] awk 取指定列
来源：http://kg.nszjky.cn

awk '{print $1, $3}' a.txt
来源：http://te.521024.cn

[R49] awk 带条件
来源：http://fk.huixiangedu.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://nl.huixiangedu.cn

[R50] awk 求和
来源：http://eh.szxytkj.cn

awk '{s += $2} END {print s}' a.txt
来源：http://qp.jianghongdianzi.cn

[R51] 排序去重取前几
来源：http://gs.colortex.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://oe.asd995.cn

[R52] 统计行数
来源：http://pl.hnjuh.cn

wc -l a.txt
来源：http://wj.hnjuh.cn

[R53] 查看文件头与实时尾
来源：http://gu.panjiajie.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://al.szxytkj.cn

[R54] 比较两个文件
来源：http://op.9csxet.cn

diff a.txt b.txt
来源：http://ca.521024.cn

[R55] 压缩与解压
来源：http://pn.bjjhwx.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://vu.hnjuh.cn

[R56] 远程拷贝
来源：http://qz.9csxet.cn

scp file user@host:/path/
来源：http://ho.bjjhwx.cn

[R57] 远程执行命令
来源：http://pg.lnxyls.cn

ssh user@host 'uptime'
来源：http://cn.shxzukj.cn

[R58] 下载文件
来源：http://ug.huixiangedu.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://up.lnxyls.cn

[R59] 发 POST JSON
来源：http://db.lnxyls.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://vh.newstarts.cn

[R60] 只看 HTTP 状态码
来源：http://ke.huanxung.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://zu.hnjuh.cn

[R61] 磁盘占用
来源：http://vh.haigaiapp.cn

df -h;  du -sh *
来源：http://zj.gzmigu.cn

[R62] 找最占空间的文件
来源：http://yz.shxzukj.cn

du -ah . | sort -rh | head -10
来源：http://yr.yuexingan06.cn

[R63] 内存与进程
来源：http://if.huixiangedu.cn

free -h;  ps aux | grep nginx
来源：http://xc.jctech888.com.cn

[R64] 结束进程
来源：http://kx.shtwfgs.cn

kill -9 $(pgrep -f app.py)
来源：http://wk.szxytkj.cn

[R65] 查看端口占用
来源：http://ky.nszjky.cn


<!-- 参考信息 -->