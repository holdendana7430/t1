代发 wailian999

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://vw.gzmigu.cn

[Q18] 模糊匹配
来源：http://st.colortex.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://lt.colortex.cn

[Q19] 范围查询
来源：http://ku.haigaiapp.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://kd.panjiajie.cn

[Q20] IN 列表
来源：http://du.haigaiapp.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://af.asd995.cn

[Q21] 空值判断
来源：http://cq.gzmigu.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://wi.szxytkj.cn

[Q22] 排序
来源：http://xk.shxzukj.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ys.haigaiapp.cn

[Q23] 分页
来源：http://fu.lnxyls.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://xy.shxzukj.cn

[Q24] 去重
来源：http://ob.panjiajie.cn

SELECT DISTINCT city FROM users;
来源：http://yj.asd995.cn

[Q25] 只取前 N 条
来源：http://vg.gzmigu.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ap.yuntaijiaju.cn

[Q26] 计数
来源：http://qe.shxzskj.cn

SELECT COUNT(*) FROM users;
来源：http://oy.haigaiapp.cn

[Q27] 条件计数
来源：http://ih.shxzskj.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://rv.haigaiapp.cn

[Q28] 求和与平均
来源：http://zu.asd995.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hn.shxzskj.cn

[Q29] 最大最小值
来源：http://rh.nszjky.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://fp.muxihuayi.cn

[Q30] 分组统计
来源：http://qe.wgjwhj.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ak.bookmarksfly.cn

[Q31] 分组后过滤
来源：http://pn.521024.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://bu.shtwfgs.cn

[Q32] 分组拼接字符串
来源：http://bo.gzmigu.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://aa.newstarts.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://qb.huanxung.cn

[Q33] 多列分组
来源：http://mg.nicolike.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ja.chemitech.net.cn

[Q34] 每组取第一条
来源：http://aa.newstarts.cn

SELECT * FROM (
来源：http://cw.shtwfgs.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://sc.huanxung.cn

) t WHERE rn = 1;
来源：http://gx.gzmigu.cn

[Q35] 内连接
来源：http://ad.bookmarksfly.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ls.jianghongdianzi.cn

[Q36] 左连接
来源：http://ep.hnjuh.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://qp.jianghongdianzi.cn

[Q37] 右连接
来源：http://it.nszjky.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://pe.szsharing.cn

[Q38] 全外连接（PostgreSQL）
来源：http://tp.newstarts.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://od.hnjuh.cn

[Q39] 自连接（查上下级）
来源：http://tj.shxzukj.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://dn.lnxyls.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://bf.hahajie.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://xz.521024.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wf.yuexingan06.cn

[Q41] 多表连接
来源：http://sk.shxzskj.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://tx.szxytkj.cn

JOIN users u ON u.id = o.user_id
来源：http://yr.jianghongdianzi.cn

JOIN products p ON p.id = o.product_id;
来源：http://ek.newstarts.cn

[Q42] 连接条件附加过滤
来源：http://cl.bookmarksfly.cn

SELECT u.name, o.amount FROM users u
来源：http://mr.lnxyls.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://lv.bjjhwx.cn

[Q43] 标量子查询
来源：http://td.bjjhwx.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://vt.huixinmuqiang.cn

[Q44] IN 子查询
来源：http://tl.yuexingan06.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://rf.9csxet.cn

[Q45] EXISTS 判断存在
来源：http://hd.hnjuh.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://sq.9csxet.cn

[Q46] NOT EXISTS 判断不存在
来源：http://ip.gzmigu.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://aw.shtwfgs.cn

[Q47] 与平均值比较
来源：http://om.hahajie.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://kx.yuntaijiaju.cn

[Q48] CTE 公用表表达式
来源：http://ao.colortex.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://fk.huixinmuqiang.cn

SELECT * FROM t WHERE c > 5;
来源：http://qy.bookmarksfly.cn

[Q49] 更新单行
来源：http://it.lnxyls.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://pr.muxihuayi.cn

[Q50] 批量更新
来源：http://dn.huixiangedu.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://vm.bjjhwx.cn

[Q51] 用子查询更新
来源：http://oy.newstarts.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mb.szxytkj.cn

[Q52] 删除指定行
来源：http://su.huixiangedu.cn

DELETE FROM users WHERE id = 10;
来源：http://rw.szsharing.cn

[Q53] 按条件删除
来源：http://bi.9csxet.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://rc.bjjhwx.cn

[Q54] 清空表
来源：http://uj.colortex.cn

TRUNCATE TABLE logs;
来源：http://kb.wgjwhj.cn

[Q55] 排名（并列占位）
来源：http://dm.chemitech.net.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ly.lnxyls.cn

[Q56] 密集排名（并列不占位）
来源：http://bs.newstarts.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://vd.hnjuh.cn

[Q57] 行号
来源：http://pg.521024.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://jq.jctech888.com.cn

[Q58] 累计求和
来源：http://kt.newstarts.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hg.bookmarksfly.cn

[Q59] 分组内累计
来源：http://tr.huixiangedu.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://za.nszjky.cn

[Q60] 取上一行 / 下一行
来源：http://eq.9csxet.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://nz.bookmarksfly.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://fa.newstarts.cn

[Q61] 移动平均
来源：http://ji.9csxet.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://cw.nicolike.cn

[Q62] 分组占比
来源：http://dq.9csxet.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ri.chemitech.net.cn

[Q63] 开启事务
来源：http://lv.bjjhwx.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://eq.nszjky.cn

[Q64] 提交事务
来源：http://oe.szxytkj.cn

COMMIT;
来源：http://wn.newstarts.cn

[Q65] 回滚事务
来源：http://ih.haigaiapp.cn

ROLLBACK;
来源：http://hf.huixiangedu.cn

[Q66] 行锁查询
来源：http://td.lnxyls.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://gw.gzmigu.cn

[Q67] 设置隔离级别
来源：http://zq.yuntaijiaju.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://tm.haigaiapp.cn

[Q68] 保存点
来源：http://dy.szsharing.cn

SAVEPOINT sp1;
来源：http://ub.bjjhwx.cn

ROLLBACK TO sp1;
来源：http://ag.gzmigu.cn

[Q69] 查看执行计划
来源：http://yi.hnjuh.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ap.huixiangedu.cn

[Q70] 更新统计信息
来源：http://jw.huixinmuqiang.cn

ANALYZE TABLE users;
来源：http://mt.jianghongdianzi.cn

[Q71] 查看建表语句
来源：http://nq.huixiangedu.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://rx.asd995.cn

[Q72] 查看索引
来源：http://gi.9csxet.cn

SHOW INDEX FROM users;
来源：http://ex.chemitech.net.cn

[Q73] 查看表状态
来源：http://qn.nszjky.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://nj.szsharing.cn

[Q74] 强制使用索引
来源：http://fd.bookmarksfly.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ff.yuexingan06.cn

[Q75] 日期格式化
来源：http://lq.shxzskj.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://co.nszjky.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://th.huanxung.cn

[Q76] 按天统计
来源：http://gp.521024.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://uh.shtwfgs.cn

[Q77] 时间加减
来源：http://ac.szxytkj.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://uc.bjjhwx.cn

[Q78] 当前时间
来源：http://ie.asd995.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://bg.bookmarksfly.cn

[Q79] 字符串拼接
来源：http://sv.shxzskj.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://nr.yuntaijiaju.cn

[Q80] 字符串截取
来源：http://cq.haigaiapp.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://xc.panjiajie.cn

[Q81] 字符串替换
来源：http://ng.lnxyls.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ra.nszjky.cn

[Q82] 字符长度与字节长度
来源：http://zd.yuntaijiaju.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://xr.chemitech.net.cn

[Q83] 大小写转换
来源：http://fg.shxzukj.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hd.szsharing.cn

[Q84] 去除首尾空格
来源：http://vi.yuntaijiaju.cn

SELECT TRIM(name) FROM users;
来源：http://lj.521024.cn

[Q85] 数值取整
来源：http://pi.colortex.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://se.shtwfgs.cn

[Q86] 读取 JSON 字段
来源：http://om.wgjwhj.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://kb.jctech888.com.cn

[Q87] JSON 字段做条件
来源：http://ns.huixinmuqiang.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://pp.shtwfgs.cn

[Q88] 行转列（条件聚合）
来源：http://ju.shxzskj.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ri.colortex.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://rt.chemitech.net.cn

[Q89] 判断表是否存在
来源：http://ik.szsharing.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://kk.bjjhwx.cn

[Q90] 生成序号列
来源：http://ad.521024.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ii.muxihuayi.cn

================================================================================
来源：http://ne.hnjuh.cn

R. Bash 专题
来源：http://ag.yuexingan06.cn

================================================================================
来源：http://pd.bookmarksfly.cn

[R01] shebang 与严格模式
来源：http://ke.wgjwhj.cn

#!/usr/bin/env bash
来源：http://go.huixiangedu.cn

set -euo pipefail
来源：http://ef.asd995.cn

[R02] 变量赋值与使用
来源：http://qj.nszjky.cn

name="Tom"; echo "$name"
来源：http://fl.newstarts.cn

[R03] 只读变量
来源：http://zy.huanxung.cn

readonly PI=3.14
来源：http://cq.521024.cn

[R04] 位置参数
来源：http://be.panjiajie.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://tm.bjjhwx.cn

[R05] 参数默认值
来源：http://qi.asd995.cn

name="${1:-default}"
来源：http://ip.szxytkj.cn

[R06] 判断命令是否存在
来源：http://fw.szsharing.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://bk.chemitech.net.cn

[R07] if 判断文件
来源：http://fq.szxytkj.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://gw.9csxet.cn

[R08] 数值比较
来源：http://ws.huanxung.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://jh.huanxung.cn

[R09] 字符串比较
来源：http://ly.szsharing.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://pu.huanxung.cn

[R10] 正则匹配
来源：http://ez.huanxung.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ik.jctech888.com.cn

[R11] case 多分支
来源：http://fz.gzmigu.cn

case "$1" in
来源：http://pu.521024.cn

start) echo "启动" ;;
来源：http://sk.panjiajie.cn

stop)  echo "停止" ;;
来源：http://af.9csxet.cn

*)     echo "未知命令" ;;
来源：http://uw.haigaiapp.cn

esac
来源：http://pz.panjiajie.cn

[R12] for 遍历文件
来源：http://pa.lnxyls.cn

for f in *.txt; do echo "$f"; done
来源：http://wb.huanxung.cn

[R13] for 计数循环
来源：http://dd.huixiangedu.cn

for i in {1..10}; do echo "$i"; done
来源：http://pd.panjiajie.cn

[R14] C 风格 for
来源：http://ji.shxzukj.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://gs.lnxyls.cn

[R15] while 逐行读文件
来源：http://di.hahajie.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hc.haigaiapp.cn

[R16] until 等待条件
来源：http://gs.panjiajie.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ya.huixinmuqiang.cn

[R17] 数组定义与取值
来源：http://zd.shxzukj.cn

arr=(a b c); echo "${arr[0]}"
来源：http://mb.panjiajie.cn

[R18] 遍历数组
来源：http://vy.huanxung.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://pi.yuexingan06.cn

[R19] 数组长度
来源：http://su.yuntaijiaju.cn

echo "${#arr[@]}"
来源：http://tj.huixinmuqiang.cn

[R20] 关联数组（字典）
来源：http://oe.colortex.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://gn.nicolike.cn

[R21] 字符串长度
来源：http://mj.asd995.cn

echo "${#s}"
来源：http://cf.hahajie.cn

[R22] 截取子串
来源：http://kd.lnxyls.cn

echo "${s:0:5}"
来源：http://pw.panjiajie.cn

[R23] 字符串替换
来源：http://lh.nicolike.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://il.huanxung.cn

[R24] 大小写转换
来源：http://ak.szsharing.cn

echo "${s^^}"; echo "${s,,}"
来源：http://di.nicolike.cn

[R25] 去后缀 / 去前缀
来源：http://iz.asd995.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://go.hahajie.cn

[R26] 命令替换
来源：http://dd.lnxyls.cn

now=$(date +%F); echo "$now"
来源：http://sk.9csxet.cn

[R27] 算术展开
来源：http://zv.muxihuayi.cn

echo $((1 + 2 * 3))
来源：http://ny.nicolike.cn

[R28] 浮点运算
来源：http://fz.asd995.cn

echo "scale=2; 10/3" | bc
来源：http://ky.9csxet.cn

[R29] 定义函数
来源：http://tf.haigaiapp.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://dv.yuexingan06.cn

[R30] 函数返回状态码
来源：http://th.9csxet.cn

f() { return 0; }; f || echo "失败了"
来源：http://nl.nicolike.cn

[R31] 局部变量
来源：http://ik.yuexingan06.cn

f() { local x=1; echo "$x"; }
来源：http://oe.asd995.cn

[R32] 参数个数校验
来源：http://ay.bookmarksfly.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://va.bjjhwx.cn

[R33] 捕获错误并提示行号
来源：http://go.wgjwhj.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://vg.huixinmuqiang.cn

[R34] 退出时清理
来源：http://zd.newstarts.cn

trap 'rm -f "$tmp"' EXIT
来源：http://pl.521024.cn

[R35] 后台执行并等待
来源：http://nk.lnxyls.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://dl.newstarts.cn

[R36] 并发执行多个任务
来源：http://gg.9csxet.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ar.yuntaijiaju.cn

[R37] 把输出赋给变量
来源：http://oh.szsharing.cn

files=$(ls -1)
来源：http://eo.huixinmuqiang.cn

[R38] 管道串联
来源：http://fm.huanxung.cn

cat a.txt | grep -i error | wc -l
来源：http://ua.hnjuh.cn

[R39] 重定向标准输出与错误
来源：http://qt.bjjhwx.cn

cmd > out.log 2>&1
来源：http://zh.hnjuh.cn

[R40] 追加写日志
来源：http://lo.huanxung.cn

echo "log" >> out.log
来源：http://tc.yuexingan06.cn

[R41] 丢弃输出
来源：http://hf.shxzukj.cn

cmd >/dev/null 2>&1
来源：http://hl.szxytkj.cn

[R42] 输入重定向
来源：http://ge.muxihuayi.cn

wc -l < a.txt
来源：http://pa.nszjky.cn

[R43] 按名字查找文件
来源：http://ht.szxytkj.cn

find . -name "*.log" -type f
来源：http://zi.bookmarksfly.cn

[R44] 按修改时间查找
来源：http://hb.huixinmuqiang.cn

find . -mtime -7 -type f
来源：http://hm.muxihuayi.cn

[R45] 批量删除
来源：http://jn.colortex.cn

find . -name "*.tmp" -delete
来源：http://ed.colortex.cn

[R46] 递归替换文件内容
来源：http://bk.bookmarksfly.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://fq.szsharing.cn

[R47] sed 单行替换
来源：http://qz.huixinmuqiang.cn

sed -i 's/foo/bar/g' a.txt
来源：http://cb.jianghongdianzi.cn

[R48] awk 取指定列
来源：http://mm.szxytkj.cn

awk '{print $1, $3}' a.txt
来源：http://qo.hahajie.cn

[R49] awk 带条件
来源：http://vv.9csxet.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://st.szsharing.cn

[R50] awk 求和
来源：http://iw.nicolike.cn

awk '{s += $2} END {print s}' a.txt
来源：http://jo.colortex.cn

[R51] 排序去重取前几
来源：http://gv.haigaiapp.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://an.chemitech.net.cn

[R52] 统计行数
来源：http://em.bookmarksfly.cn

wc -l a.txt
来源：http://qr.panjiajie.cn

[R53] 查看文件头与实时尾
来源：http://zz.huanxung.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hx.newstarts.cn

[R54] 比较两个文件
来源：http://cq.yuntaijiaju.cn

diff a.txt b.txt
来源：http://gb.szxytkj.cn

[R55] 压缩与解压
来源：http://fd.yuexingan06.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://vt.hnjuh.cn

[R56] 远程拷贝
来源：http://lm.muxihuayi.cn

scp file user@host:/path/
来源：http://we.szxytkj.cn

[R57] 远程执行命令
来源：http://ga.gzmigu.cn

ssh user@host 'uptime'
来源：http://pt.muxihuayi.cn

[R58] 下载文件
来源：http://cy.huixinmuqiang.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://uh.521024.cn

[R59] 发 POST JSON
来源：http://ej.hnjuh.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://xa.haigaiapp.cn

[R60] 只看 HTTP 状态码
来源：http://ls.9csxet.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://rw.chemitech.net.cn

[R61] 磁盘占用
来源：http://au.hnjuh.cn

df -h;  du -sh *
来源：http://um.colortex.cn

[R62] 找最占空间的文件
来源：http://wh.huixiangedu.cn

du -ah . | sort -rh | head -10
来源：http://gh.shtwfgs.cn

[R63] 内存与进程
来源：http://be.hnjuh.cn

free -h;  ps aux | grep nginx
来源：http://ju.jianghongdianzi.cn

[R64] 结束进程
来源：http://ov.shxzukj.cn

kill -9 $(pgrep -f app.py)
来源：http://ue.shtwfgs.cn

[R65] 查看端口占用
来源：http://oz.haigaiapp.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://dz.yuntaijiaju.cn

[R66] 定时任务
来源：http://zu.gzmigu.cn

crontab -e;  crontab -l
来源：http://le.huixiangedu.cn

[R67] 生成随机十六进制串
来源：http://we.szsharing.cn


<!-- 参考信息 -->