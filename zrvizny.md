代发 wailian999

[Q14] 存在则更新（upsert）
来源：http://wx.9csxet.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://uc.jianghongdianzi.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://yf.jctech888.com.cn

[Q15] 查询全部
来源：http://vv.wgjwhj.cn

SELECT * FROM users;
来源：http://me.hnjuh.cn

[Q16] 查询指定列
来源：http://sr.shxzukj.cn

SELECT id, name FROM users;
来源：http://xh.szxytkj.cn

[Q17] 条件查询
来源：http://on.9csxet.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://yu.521024.cn

[Q18] 模糊匹配
来源：http://hu.szsharing.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://lr.newstarts.cn

[Q19] 范围查询
来源：http://il.lnxyls.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wb.hahajie.cn

[Q20] IN 列表
来源：http://zq.colortex.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://yy.yuexingan06.cn

[Q21] 空值判断
来源：http://kt.gzmigu.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://wt.hnjuh.cn

[Q22] 排序
来源：http://cd.521024.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ge.haigaiapp.cn

[Q23] 分页
来源：http://da.panjiajie.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mc.hahajie.cn

[Q24] 去重
来源：http://sv.huixiangedu.cn

SELECT DISTINCT city FROM users;
来源：http://bp.9csxet.cn

[Q25] 只取前 N 条
来源：http://wd.yuntaijiaju.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://sz.shxzukj.cn

[Q26] 计数
来源：http://pv.panjiajie.cn

SELECT COUNT(*) FROM users;
来源：http://vq.yuntaijiaju.cn

[Q27] 条件计数
来源：http://rd.muxihuayi.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://il.szsharing.cn

[Q28] 求和与平均
来源：http://gd.shxzskj.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://uw.hnjuh.cn

[Q29] 最大最小值
来源：http://ht.yuntaijiaju.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://aq.jianghongdianzi.cn

[Q30] 分组统计
来源：http://kq.shxzskj.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://we.shxzukj.cn

[Q31] 分组后过滤
来源：http://as.muxihuayi.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://tp.hahajie.cn

[Q32] 分组拼接字符串
来源：http://au.newstarts.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ja.521024.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://zs.asd995.cn

[Q33] 多列分组
来源：http://iu.nicolike.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ro.bjjhwx.cn

[Q34] 每组取第一条
来源：http://ir.huixiangedu.cn

SELECT * FROM (
来源：http://sp.newstarts.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://yr.jctech888.com.cn

) t WHERE rn = 1;
来源：http://sn.muxihuayi.cn

[Q35] 内连接
来源：http://jw.muxihuayi.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://fj.jianghongdianzi.cn

[Q36] 左连接
来源：http://td.muxihuayi.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://aq.yuexingan06.cn

[Q37] 右连接
来源：http://zr.chemitech.net.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://lg.yuntaijiaju.cn

[Q38] 全外连接（PostgreSQL）
来源：http://st.bjjhwx.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://yk.shxzukj.cn

[Q39] 自连接（查上下级）
来源：http://og.panjiajie.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://ih.wgjwhj.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ky.szxytkj.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://sn.haigaiapp.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://qu.szxytkj.cn

[Q41] 多表连接
来源：http://ld.colortex.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://ut.lnxyls.cn

JOIN users u ON u.id = o.user_id
来源：http://so.szxytkj.cn

JOIN products p ON p.id = o.product_id;
来源：http://pg.nszjky.cn

[Q42] 连接条件附加过滤
来源：http://pj.shtwfgs.cn

SELECT u.name, o.amount FROM users u
来源：http://my.jctech888.com.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://xu.szxytkj.cn

[Q43] 标量子查询
来源：http://oo.asd995.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://lj.haigaiapp.cn

[Q44] IN 子查询
来源：http://uw.shxzukj.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://uh.panjiajie.cn

[Q45] EXISTS 判断存在
来源：http://yb.lnxyls.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://qk.9csxet.cn

[Q46] NOT EXISTS 判断不存在
来源：http://cz.huixinmuqiang.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ta.huanxung.cn

[Q47] 与平均值比较
来源：http://gc.bookmarksfly.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hx.nicolike.cn

[Q48] CTE 公用表表达式
来源：http://ke.hahajie.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://bi.huanxung.cn

SELECT * FROM t WHERE c > 5;
来源：http://pv.521024.cn

[Q49] 更新单行
来源：http://oa.newstarts.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://rj.bjjhwx.cn

[Q50] 批量更新
来源：http://ym.hnjuh.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://vg.huixiangedu.cn

[Q51] 用子查询更新
来源：http://az.nszjky.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://tc.nszjky.cn

[Q52] 删除指定行
来源：http://wy.colortex.cn

DELETE FROM users WHERE id = 10;
来源：http://nj.shxzukj.cn

[Q53] 按条件删除
来源：http://xq.521024.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wp.shxzskj.cn

[Q54] 清空表
来源：http://cl.colortex.cn

TRUNCATE TABLE logs;
来源：http://es.bjjhwx.cn

[Q55] 排名（并列占位）
来源：http://nb.asd995.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ry.nicolike.cn

[Q56] 密集排名（并列不占位）
来源：http://wj.hahajie.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://lt.szsharing.cn

[Q57] 行号
来源：http://op.bjjhwx.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ru.521024.cn

[Q58] 累计求和
来源：http://pf.hahajie.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://rc.hnjuh.cn

[Q59] 分组内累计
来源：http://xl.haigaiapp.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://nm.hnjuh.cn

[Q60] 取上一行 / 下一行
来源：http://aw.yuexingan06.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://sf.muxihuayi.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://xz.shxzskj.cn

[Q61] 移动平均
来源：http://bm.shxzskj.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://bn.haigaiapp.cn

[Q62] 分组占比
来源：http://tj.shxzskj.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://av.yuexingan06.cn

[Q63] 开启事务
来源：http://qp.521024.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://tm.chemitech.net.cn

[Q64] 提交事务
来源：http://qx.szxytkj.cn

COMMIT;
来源：http://qe.521024.cn

[Q65] 回滚事务
来源：http://mp.shtwfgs.cn

ROLLBACK;
来源：http://ex.huixinmuqiang.cn

[Q66] 行锁查询
来源：http://pv.szsharing.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://oa.szxytkj.cn

[Q67] 设置隔离级别
来源：http://uc.jianghongdianzi.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://bz.asd995.cn

[Q68] 保存点
来源：http://ua.asd995.cn

SAVEPOINT sp1;
来源：http://nq.nszjky.cn

ROLLBACK TO sp1;
来源：http://lg.hahajie.cn

[Q69] 查看执行计划
来源：http://fl.shtwfgs.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://zx.colortex.cn

[Q70] 更新统计信息
来源：http://na.szsharing.cn

ANALYZE TABLE users;
来源：http://du.szsharing.cn

[Q71] 查看建表语句
来源：http://ls.yuntaijiaju.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ky.bjjhwx.cn

[Q72] 查看索引
来源：http://kj.huixiangedu.cn

SHOW INDEX FROM users;
来源：http://tn.shxzukj.cn

[Q73] 查看表状态
来源：http://us.szxytkj.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://pc.newstarts.cn

[Q74] 强制使用索引
来源：http://cp.jianghongdianzi.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://pq.bjjhwx.cn

[Q75] 日期格式化
来源：http://aa.huixiangedu.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://pz.chemitech.net.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mn.colortex.cn

[Q76] 按天统计
来源：http://ze.9csxet.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://bt.lnxyls.cn

[Q77] 时间加减
来源：http://tt.shtwfgs.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://pp.panjiajie.cn

[Q78] 当前时间
来源：http://kc.szsharing.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://zy.gzmigu.cn

[Q79] 字符串拼接
来源：http://xz.wgjwhj.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://gt.bjjhwx.cn

[Q80] 字符串截取
来源：http://fr.huixinmuqiang.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://jg.jianghongdianzi.cn

[Q81] 字符串替换
来源：http://sy.newstarts.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://qr.nicolike.cn

[Q82] 字符长度与字节长度
来源：http://hk.nicolike.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://pv.hahajie.cn

[Q83] 大小写转换
来源：http://hh.asd995.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://dn.huixiangedu.cn

[Q84] 去除首尾空格
来源：http://og.szxytkj.cn

SELECT TRIM(name) FROM users;
来源：http://bd.huanxung.cn

[Q85] 数值取整
来源：http://td.muxihuayi.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://cy.huixinmuqiang.cn

[Q86] 读取 JSON 字段
来源：http://hi.huixiangedu.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://rk.bookmarksfly.cn

[Q87] JSON 字段做条件
来源：http://wi.wgjwhj.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ef.yuexingan06.cn

[Q88] 行转列（条件聚合）
来源：http://tz.nszjky.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://rl.jianghongdianzi.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://to.huixiangedu.cn

[Q89] 判断表是否存在
来源：http://jn.haigaiapp.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://po.haigaiapp.cn

[Q90] 生成序号列
来源：http://pw.gzmigu.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://pm.huixiangedu.cn

================================================================================
来源：http://op.jianghongdianzi.cn

R. Bash 专题
来源：http://hq.shtwfgs.cn

================================================================================
来源：http://av.szxytkj.cn

[R01] shebang 与严格模式
来源：http://hn.yuntaijiaju.cn

#!/usr/bin/env bash
来源：http://kw.jctech888.com.cn

set -euo pipefail
来源：http://nj.newstarts.cn

[R02] 变量赋值与使用
来源：http://rv.asd995.cn

name="Tom"; echo "$name"
来源：http://br.nszjky.cn

[R03] 只读变量
来源：http://vi.panjiajie.cn

readonly PI=3.14
来源：http://lh.wgjwhj.cn

[R04] 位置参数
来源：http://dh.jianghongdianzi.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://bg.colortex.cn

[R05] 参数默认值
来源：http://hk.shxzukj.cn

name="${1:-default}"
来源：http://ni.shtwfgs.cn

[R06] 判断命令是否存在
来源：http://uf.szxytkj.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ut.shtwfgs.cn

[R07] if 判断文件
来源：http://om.nicolike.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://yg.bjjhwx.cn

[R08] 数值比较
来源：http://mt.huixiangedu.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://xn.szsharing.cn

[R09] 字符串比较
来源：http://jl.szsharing.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://yt.yuntaijiaju.cn

[R10] 正则匹配
来源：http://gn.yuexingan06.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mm.jctech888.com.cn

[R11] case 多分支
来源：http://fr.yuntaijiaju.cn

case "$1" in
来源：http://ia.muxihuayi.cn

start) echo "启动" ;;
来源：http://qz.colortex.cn

stop)  echo "停止" ;;
来源：http://zh.jctech888.com.cn

*)     echo "未知命令" ;;
来源：http://pl.yuntaijiaju.cn

esac
来源：http://gq.jianghongdianzi.cn

[R12] for 遍历文件
来源：http://fr.nszjky.cn

for f in *.txt; do echo "$f"; done
来源：http://fe.huixinmuqiang.cn

[R13] for 计数循环
来源：http://mb.colortex.cn

for i in {1..10}; do echo "$i"; done
来源：http://tx.bjjhwx.cn

[R14] C 风格 for
来源：http://yq.nicolike.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://rm.jianghongdianzi.cn

[R15] while 逐行读文件
来源：http://td.shxzskj.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://si.shxzukj.cn

[R16] until 等待条件
来源：http://bx.newstarts.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://nr.bjjhwx.cn

[R17] 数组定义与取值
来源：http://ou.panjiajie.cn

arr=(a b c); echo "${arr[0]}"
来源：http://rl.jctech888.com.cn

[R18] 遍历数组
来源：http://dt.nszjky.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://er.shxzukj.cn

[R19] 数组长度
来源：http://fr.nicolike.cn

echo "${#arr[@]}"
来源：http://qw.haigaiapp.cn

[R20] 关联数组（字典）
来源：http://kt.panjiajie.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://rs.huixinmuqiang.cn

[R21] 字符串长度
来源：http://po.jianghongdianzi.cn

echo "${#s}"
来源：http://to.chemitech.net.cn

[R22] 截取子串
来源：http://nn.shxzukj.cn

echo "${s:0:5}"
来源：http://jo.szsharing.cn

[R23] 字符串替换
来源：http://me.szxytkj.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://cj.hahajie.cn

[R24] 大小写转换
来源：http://cw.hnjuh.cn

echo "${s^^}"; echo "${s,,}"
来源：http://do.jianghongdianzi.cn

[R25] 去后缀 / 去前缀
来源：http://fo.bjjhwx.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://qt.yuexingan06.cn

[R26] 命令替换
来源：http://iy.shxzskj.cn

now=$(date +%F); echo "$now"
来源：http://rs.yuntaijiaju.cn

[R27] 算术展开
来源：http://js.nszjky.cn

echo $((1 + 2 * 3))
来源：http://kg.shxzskj.cn

[R28] 浮点运算
来源：http://vv.nszjky.cn

echo "scale=2; 10/3" | bc
来源：http://mf.haigaiapp.cn

[R29] 定义函数
来源：http://aa.muxihuayi.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ch.hnjuh.cn

[R30] 函数返回状态码
来源：http://ip.szsharing.cn

f() { return 0; }; f || echo "失败了"
来源：http://lz.asd995.cn

[R31] 局部变量
来源：http://dy.yuexingan06.cn

f() { local x=1; echo "$x"; }
来源：http://hx.szsharing.cn

[R32] 参数个数校验
来源：http://ej.panjiajie.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ax.huixinmuqiang.cn

[R33] 捕获错误并提示行号
来源：http://wp.jctech888.com.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ip.newstarts.cn

[R34] 退出时清理
来源：http://ky.hahajie.cn

trap 'rm -f "$tmp"' EXIT
来源：http://ik.huanxung.cn

[R35] 后台执行并等待
来源：http://fc.wgjwhj.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://pn.chemitech.net.cn

[R36] 并发执行多个任务
来源：http://nn.9csxet.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://lk.panjiajie.cn

[R37] 把输出赋给变量
来源：http://ny.nszjky.cn

files=$(ls -1)
来源：http://pl.lnxyls.cn

[R38] 管道串联
来源：http://du.muxihuayi.cn

cat a.txt | grep -i error | wc -l
来源：http://fh.szsharing.cn

[R39] 重定向标准输出与错误
来源：http://us.gzmigu.cn

cmd > out.log 2>&1
来源：http://yi.panjiajie.cn

[R40] 追加写日志
来源：http://wg.szxytkj.cn

echo "log" >> out.log
来源：http://lv.huixiangedu.cn

[R41] 丢弃输出
来源：http://cy.hahajie.cn

cmd >/dev/null 2>&1
来源：http://jq.jctech888.com.cn

[R42] 输入重定向
来源：http://ju.hahajie.cn

wc -l < a.txt
来源：http://cs.shxzukj.cn

[R43] 按名字查找文件
来源：http://ly.bjjhwx.cn

find . -name "*.log" -type f
来源：http://dr.panjiajie.cn

[R44] 按修改时间查找
来源：http://vs.chemitech.net.cn

find . -mtime -7 -type f
来源：http://am.jianghongdianzi.cn

[R45] 批量删除
来源：http://es.szsharing.cn

find . -name "*.tmp" -delete
来源：http://ve.newstarts.cn

[R46] 递归替换文件内容
来源：http://qa.wgjwhj.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://em.haigaiapp.cn

[R47] sed 单行替换
来源：http://wy.chemitech.net.cn

sed -i 's/foo/bar/g' a.txt
来源：http://gs.wgjwhj.cn

[R48] awk 取指定列
来源：http://nw.wgjwhj.cn

awk '{print $1, $3}' a.txt
来源：http://mk.hnjuh.cn

[R49] awk 带条件
来源：http://ld.panjiajie.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://cb.shxzukj.cn

[R50] awk 求和
来源：http://ga.huanxung.cn

awk '{s += $2} END {print s}' a.txt
来源：http://xa.huixinmuqiang.cn

[R51] 排序去重取前几
来源：http://id.shxzukj.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://qx.shxzskj.cn

[R52] 统计行数
来源：http://na.newstarts.cn

wc -l a.txt
来源：http://cj.huanxung.cn

[R53] 查看文件头与实时尾
来源：http://qv.hahajie.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://uz.huanxung.cn

[R54] 比较两个文件
来源：http://cq.shxzukj.cn

diff a.txt b.txt
来源：http://uq.jianghongdianzi.cn

[R55] 压缩与解压
来源：http://al.bjjhwx.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://rw.huixinmuqiang.cn

[R56] 远程拷贝
来源：http://ie.yuexingan06.cn

scp file user@host:/path/
来源：http://zw.yuntaijiaju.cn

[R57] 远程执行命令
来源：http://ib.jianghongdianzi.cn

ssh user@host 'uptime'
来源：http://dm.9csxet.cn

[R58] 下载文件
来源：http://pk.huixiangedu.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ji.shtwfgs.cn

[R59] 发 POST JSON
来源：http://wb.huanxung.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://id.9csxet.cn

[R60] 只看 HTTP 状态码
来源：http://go.szxytkj.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://lt.nicolike.cn

[R61] 磁盘占用
来源：http://yc.lnxyls.cn

df -h;  du -sh *
来源：http://sx.huanxung.cn

[R62] 找最占空间的文件
来源：http://xt.jctech888.com.cn

du -ah . | sort -rh | head -10
来源：http://hw.lnxyls.cn

[R63] 内存与进程
来源：http://dk.huixiangedu.cn


<!-- 参考信息 -->