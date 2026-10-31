代发 wailian999

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://sz.huanxung.cn

[Q18] 模糊匹配
来源：http://kk.gzmigu.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://no.huanxung.cn

[Q19] 范围查询
来源：http://aa.bookmarksfly.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://st.nicolike.cn

[Q20] IN 列表
来源：http://lq.szxytkj.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://xv.hnjuh.cn

[Q21] 空值判断
来源：http://fy.chemitech.net.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://xe.huanxung.cn

[Q22] 排序
来源：http://fg.shtwfgs.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://pv.hahajie.cn

[Q23] 分页
来源：http://vq.hahajie.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://io.huixinmuqiang.cn

[Q24] 去重
来源：http://ng.lnxyls.cn

SELECT DISTINCT city FROM users;
来源：http://js.yuntaijiaju.cn

[Q25] 只取前 N 条
来源：http://dg.lnxyls.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://uh.yuexingan06.cn

[Q26] 计数
来源：http://su.bjjhwx.cn

SELECT COUNT(*) FROM users;
来源：http://hx.bookmarksfly.cn

[Q27] 条件计数
来源：http://ld.yuexingan06.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://uu.wgjwhj.cn

[Q28] 求和与平均
来源：http://oj.haigaiapp.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://ay.colortex.cn

[Q29] 最大最小值
来源：http://ua.nszjky.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://fg.colortex.cn

[Q30] 分组统计
来源：http://hk.yuexingan06.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wt.gzmigu.cn

[Q31] 分组后过滤
来源：http://eu.huanxung.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ds.hahajie.cn

[Q32] 分组拼接字符串
来源：http://pd.bookmarksfly.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://eb.9csxet.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://se.szsharing.cn

[Q33] 多列分组
来源：http://wi.muxihuayi.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://tq.gzmigu.cn

[Q34] 每组取第一条
来源：http://zn.yuexingan06.cn

SELECT * FROM (
来源：http://vf.521024.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://pd.yuntaijiaju.cn

) t WHERE rn = 1;
来源：http://gi.shtwfgs.cn

[Q35] 内连接
来源：http://wy.nszjky.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://lt.jctech888.com.cn

[Q36] 左连接
来源：http://ga.yuntaijiaju.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://kq.colortex.cn

[Q37] 右连接
来源：http://eq.jianghongdianzi.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://dg.colortex.cn

[Q38] 全外连接（PostgreSQL）
来源：http://jq.asd995.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://tp.shxzskj.cn

[Q39] 自连接（查上下级）
来源：http://xo.lnxyls.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://ev.nszjky.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://yf.bjjhwx.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://yb.gzmigu.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ww.shtwfgs.cn

[Q41] 多表连接
来源：http://gu.szsharing.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://di.hahajie.cn

JOIN users u ON u.id = o.user_id
来源：http://of.muxihuayi.cn

JOIN products p ON p.id = o.product_id;
来源：http://ld.szxytkj.cn

[Q42] 连接条件附加过滤
来源：http://jc.wgjwhj.cn

SELECT u.name, o.amount FROM users u
来源：http://gy.panjiajie.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ub.bjjhwx.cn

[Q43] 标量子查询
来源：http://ol.9csxet.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://bc.szxytkj.cn

[Q44] IN 子查询
来源：http://lx.shxzukj.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://sl.huanxung.cn

[Q45] EXISTS 判断存在
来源：http://vj.shxzskj.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://bl.newstarts.cn

[Q46] NOT EXISTS 判断不存在
来源：http://pr.yuexingan06.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ni.hahajie.cn

[Q47] 与平均值比较
来源：http://tl.9csxet.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://oq.szsharing.cn

[Q48] CTE 公用表表达式
来源：http://iy.asd995.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://sj.szsharing.cn

SELECT * FROM t WHERE c > 5;
来源：http://ok.muxihuayi.cn

[Q49] 更新单行
来源：http://kq.colortex.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://dr.huixiangedu.cn

[Q50] 批量更新
来源：http://rd.lnxyls.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://qg.huanxung.cn

[Q51] 用子查询更新
来源：http://ux.muxihuayi.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://oy.wgjwhj.cn

[Q52] 删除指定行
来源：http://gc.lnxyls.cn

DELETE FROM users WHERE id = 10;
来源：http://sj.9csxet.cn

[Q53] 按条件删除
来源：http://az.szsharing.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ef.lnxyls.cn

[Q54] 清空表
来源：http://jn.521024.cn

TRUNCATE TABLE logs;
来源：http://mr.jctech888.com.cn

[Q55] 排名（并列占位）
来源：http://jc.huixinmuqiang.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://aw.bjjhwx.cn

[Q56] 密集排名（并列不占位）
来源：http://hb.hnjuh.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://cj.gzmigu.cn

[Q57] 行号
来源：http://hm.szxytkj.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://bh.shxzskj.cn

[Q58] 累计求和
来源：http://vj.newstarts.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://gb.colortex.cn

[Q59] 分组内累计
来源：http://sr.colortex.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://qh.haigaiapp.cn

[Q60] 取上一行 / 下一行
来源：http://nq.newstarts.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ue.hnjuh.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://la.lnxyls.cn

[Q61] 移动平均
来源：http://aa.gzmigu.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://vj.9csxet.cn

[Q62] 分组占比
来源：http://dm.newstarts.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ee.colortex.cn

[Q63] 开启事务
来源：http://qj.huanxung.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://hl.yuntaijiaju.cn

[Q64] 提交事务
来源：http://ok.chemitech.net.cn

COMMIT;
来源：http://gm.shtwfgs.cn

[Q65] 回滚事务
来源：http://bn.wgjwhj.cn

ROLLBACK;
来源：http://vz.jianghongdianzi.cn

[Q66] 行锁查询
来源：http://pd.bookmarksfly.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://tv.shxzskj.cn

[Q67] 设置隔离级别
来源：http://jj.muxihuayi.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://jy.haigaiapp.cn

[Q68] 保存点
来源：http://mu.yuexingan06.cn

SAVEPOINT sp1;
来源：http://ld.shxzskj.cn

ROLLBACK TO sp1;
来源：http://xc.huixiangedu.cn

[Q69] 查看执行计划
来源：http://zi.szxytkj.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://cr.lnxyls.cn

[Q70] 更新统计信息
来源：http://to.yuexingan06.cn

ANALYZE TABLE users;
来源：http://we.newstarts.cn

[Q71] 查看建表语句
来源：http://ae.wgjwhj.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://zp.wgjwhj.cn

[Q72] 查看索引
来源：http://rh.yuexingan06.cn

SHOW INDEX FROM users;
来源：http://hn.nszjky.cn

[Q73] 查看表状态
来源：http://ep.bjjhwx.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://ko.lnxyls.cn

[Q74] 强制使用索引
来源：http://zn.bjjhwx.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://tk.colortex.cn

[Q75] 日期格式化
来源：http://ay.nicolike.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://gs.yuexingan06.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://kb.bjjhwx.cn

[Q76] 按天统计
来源：http://wp.shtwfgs.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://sr.haigaiapp.cn

[Q77] 时间加减
来源：http://fa.9csxet.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://kv.nicolike.cn

[Q78] 当前时间
来源：http://pc.yuexingan06.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://if.colortex.cn

[Q79] 字符串拼接
来源：http://sh.huixiangedu.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://jq.muxihuayi.cn

[Q80] 字符串截取
来源：http://dq.colortex.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ct.9csxet.cn

[Q81] 字符串替换
来源：http://yk.wgjwhj.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://jn.hahajie.cn

[Q82] 字符长度与字节长度
来源：http://rf.9csxet.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://pl.huixinmuqiang.cn

[Q83] 大小写转换
来源：http://bh.haigaiapp.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://gr.muxihuayi.cn

[Q84] 去除首尾空格
来源：http://jn.gzmigu.cn

SELECT TRIM(name) FROM users;
来源：http://sp.asd995.cn

[Q85] 数值取整
来源：http://sg.panjiajie.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://zk.wgjwhj.cn

[Q86] 读取 JSON 字段
来源：http://yo.huixiangedu.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://dk.huixinmuqiang.cn

[Q87] JSON 字段做条件
来源：http://cg.shxzskj.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://jl.wgjwhj.cn

[Q88] 行转列（条件聚合）
来源：http://fi.panjiajie.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://yb.gzmigu.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://bw.bookmarksfly.cn

[Q89] 判断表是否存在
来源：http://kg.bjjhwx.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mx.muxihuayi.cn

[Q90] 生成序号列
来源：http://bk.newstarts.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://xh.newstarts.cn

================================================================================
来源：http://em.shxzskj.cn

R. Bash 专题
来源：http://ch.szsharing.cn

================================================================================
来源：http://ve.hahajie.cn

[R01] shebang 与严格模式
来源：http://ou.9csxet.cn

#!/usr/bin/env bash
来源：http://nd.shtwfgs.cn

set -euo pipefail
来源：http://zb.asd995.cn

[R02] 变量赋值与使用
来源：http://wx.haigaiapp.cn

name="Tom"; echo "$name"
来源：http://gs.hnjuh.cn

[R03] 只读变量
来源：http://om.hahajie.cn

readonly PI=3.14
来源：http://db.wgjwhj.cn

[R04] 位置参数
来源：http://ya.muxihuayi.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ak.nicolike.cn

[R05] 参数默认值
来源：http://sx.hahajie.cn

name="${1:-default}"
来源：http://id.521024.cn

[R06] 判断命令是否存在
来源：http://it.szsharing.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ft.lnxyls.cn

[R07] if 判断文件
来源：http://kx.shtwfgs.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://fl.jianghongdianzi.cn

[R08] 数值比较
来源：http://op.hnjuh.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://ha.shxzskj.cn

[R09] 字符串比较
来源：http://ej.jctech888.com.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hf.lnxyls.cn

[R10] 正则匹配
来源：http://yg.hnjuh.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://xk.shxzskj.cn

[R11] case 多分支
来源：http://md.jctech888.com.cn

case "$1" in
来源：http://fe.shxzskj.cn

start) echo "启动" ;;
来源：http://sx.jianghongdianzi.cn

stop)  echo "停止" ;;
来源：http://rb.chemitech.net.cn

*)     echo "未知命令" ;;
来源：http://kw.wgjwhj.cn

esac
来源：http://yz.bjjhwx.cn

[R12] for 遍历文件
来源：http://du.hnjuh.cn

for f in *.txt; do echo "$f"; done
来源：http://ec.huixinmuqiang.cn

[R13] for 计数循环
来源：http://hw.newstarts.cn

for i in {1..10}; do echo "$i"; done
来源：http://tk.lnxyls.cn

[R14] C 风格 for
来源：http://wz.newstarts.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ei.jctech888.com.cn

[R15] while 逐行读文件
来源：http://sw.hnjuh.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://tv.szxytkj.cn

[R16] until 等待条件
来源：http://kk.wgjwhj.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ic.hnjuh.cn

[R17] 数组定义与取值
来源：http://of.szxytkj.cn

arr=(a b c); echo "${arr[0]}"
来源：http://bd.wgjwhj.cn

[R18] 遍历数组
来源：http://qb.yuntaijiaju.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://lf.bjjhwx.cn

[R19] 数组长度
来源：http://vx.gzmigu.cn

echo "${#arr[@]}"
来源：http://pv.hnjuh.cn

[R20] 关联数组（字典）
来源：http://em.wgjwhj.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://lo.nszjky.cn

[R21] 字符串长度
来源：http://oi.lnxyls.cn

echo "${#s}"
来源：http://fz.huixiangedu.cn

[R22] 截取子串
来源：http://jx.yuexingan06.cn

echo "${s:0:5}"
来源：http://li.lnxyls.cn

[R23] 字符串替换
来源：http://eo.yuntaijiaju.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ec.szsharing.cn

[R24] 大小写转换
来源：http://zi.jctech888.com.cn

echo "${s^^}"; echo "${s,,}"
来源：http://ey.gzmigu.cn

[R25] 去后缀 / 去前缀
来源：http://hh.shxzskj.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://pw.shxzskj.cn

[R26] 命令替换
来源：http://nj.nicolike.cn

now=$(date +%F); echo "$now"
来源：http://al.huixiangedu.cn

[R27] 算术展开
来源：http://qj.huanxung.cn

echo $((1 + 2 * 3))
来源：http://zj.muxihuayi.cn

[R28] 浮点运算
来源：http://uc.huanxung.cn

echo "scale=2; 10/3" | bc
来源：http://df.newstarts.cn

[R29] 定义函数
来源：http://ow.bookmarksfly.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hh.shtwfgs.cn

[R30] 函数返回状态码
来源：http://ty.chemitech.net.cn

f() { return 0; }; f || echo "失败了"
来源：http://jh.szxytkj.cn

[R31] 局部变量
来源：http://si.asd995.cn

f() { local x=1; echo "$x"; }
来源：http://rh.lnxyls.cn

[R32] 参数个数校验
来源：http://ol.shxzskj.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://jv.shxzskj.cn

[R33] 捕获错误并提示行号
来源：http://sz.jianghongdianzi.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://yq.lnxyls.cn

[R34] 退出时清理
来源：http://ch.521024.cn

trap 'rm -f "$tmp"' EXIT
来源：http://um.shtwfgs.cn

[R35] 后台执行并等待
来源：http://yc.szsharing.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://bj.muxihuayi.cn

[R36] 并发执行多个任务
来源：http://tq.lnxyls.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://am.yuexingan06.cn

[R37] 把输出赋给变量
来源：http://af.gzmigu.cn

files=$(ls -1)
来源：http://zy.huixinmuqiang.cn

[R38] 管道串联
来源：http://kh.huixinmuqiang.cn

cat a.txt | grep -i error | wc -l
来源：http://tr.bookmarksfly.cn

[R39] 重定向标准输出与错误
来源：http://om.szsharing.cn

cmd > out.log 2>&1
来源：http://su.muxihuayi.cn

[R40] 追加写日志
来源：http://od.szxytkj.cn

echo "log" >> out.log
来源：http://wm.bjjhwx.cn

[R41] 丢弃输出
来源：http://jc.bjjhwx.cn

cmd >/dev/null 2>&1
来源：http://iq.hnjuh.cn

[R42] 输入重定向
来源：http://zq.shxzukj.cn

wc -l < a.txt
来源：http://cj.muxihuayi.cn

[R43] 按名字查找文件
来源：http://if.shtwfgs.cn

find . -name "*.log" -type f
来源：http://sl.szxytkj.cn

[R44] 按修改时间查找
来源：http://uk.lnxyls.cn

find . -mtime -7 -type f
来源：http://yq.asd995.cn

[R45] 批量删除
来源：http://jn.jctech888.com.cn

find . -name "*.tmp" -delete
来源：http://jb.hnjuh.cn

[R46] 递归替换文件内容
来源：http://uf.muxihuayi.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://rw.hahajie.cn

[R47] sed 单行替换
来源：http://dd.bjjhwx.cn

sed -i 's/foo/bar/g' a.txt
来源：http://dm.huixiangedu.cn

[R48] awk 取指定列
来源：http://wf.shxzukj.cn

awk '{print $1, $3}' a.txt
来源：http://hh.wgjwhj.cn

[R49] awk 带条件
来源：http://po.9csxet.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://xz.szxytkj.cn

[R50] awk 求和
来源：http://jj.huixiangedu.cn

awk '{s += $2} END {print s}' a.txt
来源：http://or.shtwfgs.cn

[R51] 排序去重取前几
来源：http://fz.hahajie.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://lu.huanxung.cn

[R52] 统计行数
来源：http://jp.colortex.cn

wc -l a.txt
来源：http://hf.gzmigu.cn

[R53] 查看文件头与实时尾
来源：http://ct.shxzskj.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://tk.shxzskj.cn

[R54] 比较两个文件
来源：http://up.nszjky.cn

diff a.txt b.txt
来源：http://tu.huixiangedu.cn

[R55] 压缩与解压
来源：http://xx.szsharing.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://oh.yuntaijiaju.cn

[R56] 远程拷贝
来源：http://aq.muxihuayi.cn

scp file user@host:/path/
来源：http://cw.huixiangedu.cn

[R57] 远程执行命令
来源：http://hl.nicolike.cn

ssh user@host 'uptime'
来源：http://kd.jianghongdianzi.cn

[R58] 下载文件
来源：http://xv.muxihuayi.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wd.shtwfgs.cn

[R59] 发 POST JSON
来源：http://jw.huanxung.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ko.huixiangedu.cn

[R60] 只看 HTTP 状态码
来源：http://xq.9csxet.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://of.wgjwhj.cn

[R61] 磁盘占用
来源：http://kx.shtwfgs.cn

df -h;  du -sh *
来源：http://xj.shtwfgs.cn

[R62] 找最占空间的文件
来源：http://su.yuexingan06.cn

du -ah . | sort -rh | head -10
来源：http://pq.nszjky.cn

[R63] 内存与进程
来源：http://dw.9csxet.cn

free -h;  ps aux | grep nginx
来源：http://ea.shxzskj.cn

[R64] 结束进程
来源：http://qx.asd995.cn

kill -9 $(pgrep -f app.py)
来源：http://pe.chemitech.net.cn

[R65] 查看端口占用
来源：http://iw.shxzskj.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ee.9csxet.cn

[R66] 定时任务
来源：http://ys.nicolike.cn

crontab -e;  crontab -l
来源：http://ky.bjjhwx.cn

[R67] 生成随机十六进制串
来源：http://ma.shxzskj.cn


<!-- 参考信息 -->