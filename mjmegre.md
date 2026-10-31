代发 wailian999

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hd.panjiajie.cn

[Q18] 模糊匹配
来源：http://xw.nicolike.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://df.huanxung.cn

[Q19] 范围查询
来源：http://ih.shxzukj.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://yh.chemitech.net.cn

[Q20] IN 列表
来源：http://gj.hnjuh.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://zk.bookmarksfly.cn

[Q21] 空值判断
来源：http://bl.szxytkj.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://bc.wgjwhj.cn

[Q22] 排序
来源：http://sc.colortex.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://am.yuexingan06.cn

[Q23] 分页
来源：http://nq.muxihuayi.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://nv.colortex.cn

[Q24] 去重
来源：http://lg.newstarts.cn

SELECT DISTINCT city FROM users;
来源：http://hx.nicolike.cn

[Q25] 只取前 N 条
来源：http://il.haigaiapp.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ls.newstarts.cn

[Q26] 计数
来源：http://cc.panjiajie.cn

SELECT COUNT(*) FROM users;
来源：http://km.yuntaijiaju.cn

[Q27] 条件计数
来源：http://hy.hnjuh.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://sm.521024.cn

[Q28] 求和与平均
来源：http://dy.yuntaijiaju.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://rx.yuexingan06.cn

[Q29] 最大最小值
来源：http://jo.hnjuh.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://jq.bookmarksfly.cn

[Q30] 分组统计
来源：http://ls.huanxung.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ab.panjiajie.cn

[Q31] 分组后过滤
来源：http://kj.shxzukj.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://dx.asd995.cn

[Q32] 分组拼接字符串
来源：http://iq.yuexingan06.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://vb.shxzukj.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://df.wgjwhj.cn

[Q33] 多列分组
来源：http://ng.asd995.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://xw.chemitech.net.cn

[Q34] 每组取第一条
来源：http://wk.shxzukj.cn

SELECT * FROM (
来源：http://ym.muxihuayi.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://tp.szxytkj.cn

) t WHERE rn = 1;
来源：http://tl.szsharing.cn

[Q35] 内连接
来源：http://qw.colortex.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://gj.huixiangedu.cn

[Q36] 左连接
来源：http://dl.hnjuh.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://qq.panjiajie.cn

[Q37] 右连接
来源：http://gk.9csxet.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://of.9csxet.cn

[Q38] 全外连接（PostgreSQL）
来源：http://ny.yuexingan06.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://qg.newstarts.cn

[Q39] 自连接（查上下级）
来源：http://ek.shxzukj.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://al.shxzskj.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://lz.wgjwhj.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://bg.haigaiapp.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://or.szxytkj.cn

[Q41] 多表连接
来源：http://kf.9csxet.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://ls.hnjuh.cn

JOIN users u ON u.id = o.user_id
来源：http://cy.haigaiapp.cn

JOIN products p ON p.id = o.product_id;
来源：http://dp.szsharing.cn

[Q42] 连接条件附加过滤
来源：http://dl.szxytkj.cn

SELECT u.name, o.amount FROM users u
来源：http://cz.hahajie.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mm.yuexingan06.cn

[Q43] 标量子查询
来源：http://nq.gzmigu.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://py.jianghongdianzi.cn

[Q44] IN 子查询
来源：http://ys.hnjuh.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://dw.szsharing.cn

[Q45] EXISTS 判断存在
来源：http://zk.shxzskj.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wn.bjjhwx.cn

[Q46] NOT EXISTS 判断不存在
来源：http://gy.haigaiapp.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wa.shxzukj.cn

[Q47] 与平均值比较
来源：http://fn.chemitech.net.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://as.shxzskj.cn

[Q48] CTE 公用表表达式
来源：http://ja.hahajie.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mr.chemitech.net.cn

SELECT * FROM t WHERE c > 5;
来源：http://lm.colortex.cn

[Q49] 更新单行
来源：http://pw.wgjwhj.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://gt.muxihuayi.cn

[Q50] 批量更新
来源：http://xy.asd995.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://bq.haigaiapp.cn

[Q51] 用子查询更新
来源：http://ce.521024.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://bo.huixinmuqiang.cn

[Q52] 删除指定行
来源：http://hg.bookmarksfly.cn

DELETE FROM users WHERE id = 10;
来源：http://nt.bookmarksfly.cn

[Q53] 按条件删除
来源：http://fo.newstarts.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://dj.huixiangedu.cn

[Q54] 清空表
来源：http://vz.bookmarksfly.cn

TRUNCATE TABLE logs;
来源：http://uy.bookmarksfly.cn

[Q55] 排名（并列占位）
来源：http://cf.yuntaijiaju.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://nv.muxihuayi.cn

[Q56] 密集排名（并列不占位）
来源：http://yf.shxzskj.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ml.muxihuayi.cn

[Q57] 行号
来源：http://ez.colortex.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://qb.newstarts.cn

[Q58] 累计求和
来源：http://jw.hahajie.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ag.chemitech.net.cn

[Q59] 分组内累计
来源：http://cp.jctech888.com.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://es.yuntaijiaju.cn

[Q60] 取上一行 / 下一行
来源：http://mj.chemitech.net.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ke.newstarts.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://yn.yuntaijiaju.cn

[Q61] 移动平均
来源：http://fe.9csxet.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://pq.panjiajie.cn

[Q62] 分组占比
来源：http://px.newstarts.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://zg.chemitech.net.cn

[Q63] 开启事务
来源：http://qp.yuntaijiaju.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://ys.shxzskj.cn

[Q64] 提交事务
来源：http://jf.yuntaijiaju.cn

COMMIT;
来源：http://ld.panjiajie.cn

[Q65] 回滚事务
来源：http://xk.shtwfgs.cn

ROLLBACK;
来源：http://yc.jctech888.com.cn

[Q66] 行锁查询
来源：http://zt.shtwfgs.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://na.colortex.cn

[Q67] 设置隔离级别
来源：http://qf.521024.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://dv.colortex.cn

[Q68] 保存点
来源：http://az.521024.cn

SAVEPOINT sp1;
来源：http://hv.9csxet.cn

ROLLBACK TO sp1;
来源：http://be.gzmigu.cn

[Q69] 查看执行计划
来源：http://zt.nszjky.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://nt.bookmarksfly.cn

[Q70] 更新统计信息
来源：http://fn.lnxyls.cn

ANALYZE TABLE users;
来源：http://xu.chemitech.net.cn

[Q71] 查看建表语句
来源：http://nb.asd995.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ja.shxzukj.cn

[Q72] 查看索引
来源：http://uj.newstarts.cn

SHOW INDEX FROM users;
来源：http://my.szsharing.cn

[Q73] 查看表状态
来源：http://as.jianghongdianzi.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://ml.shxzskj.cn

[Q74] 强制使用索引
来源：http://dg.gzmigu.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://fz.nszjky.cn

[Q75] 日期格式化
来源：http://gm.chemitech.net.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://rg.huixinmuqiang.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://yr.shxzukj.cn

[Q76] 按天统计
来源：http://th.jctech888.com.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wz.panjiajie.cn

[Q77] 时间加减
来源：http://qw.9csxet.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://lx.szsharing.cn

[Q78] 当前时间
来源：http://bb.huanxung.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://vq.hnjuh.cn

[Q79] 字符串拼接
来源：http://kt.newstarts.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://rc.huixiangedu.cn

[Q80] 字符串截取
来源：http://fc.muxihuayi.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://cd.wgjwhj.cn

[Q81] 字符串替换
来源：http://zf.panjiajie.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ow.szxytkj.cn

[Q82] 字符长度与字节长度
来源：http://ou.haigaiapp.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://fg.9csxet.cn

[Q83] 大小写转换
来源：http://nt.nszjky.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://we.hnjuh.cn

[Q84] 去除首尾空格
来源：http://eq.szxytkj.cn

SELECT TRIM(name) FROM users;
来源：http://fa.szsharing.cn

[Q85] 数值取整
来源：http://sv.muxihuayi.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://rj.szsharing.cn

[Q86] 读取 JSON 字段
来源：http://un.szxytkj.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://pd.yuexingan06.cn

[Q87] JSON 字段做条件
来源：http://jb.panjiajie.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://yl.521024.cn

[Q88] 行转列（条件聚合）
来源：http://dt.hnjuh.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://qr.muxihuayi.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://kz.huanxung.cn

[Q89] 判断表是否存在
来源：http://ss.nszjky.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://cs.yuntaijiaju.cn

[Q90] 生成序号列
来源：http://ft.shtwfgs.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://iu.521024.cn

================================================================================
来源：http://ip.lnxyls.cn

R. Bash 专题
来源：http://qx.chemitech.net.cn

================================================================================
来源：http://si.bjjhwx.cn

[R01] shebang 与严格模式
来源：http://dx.szxytkj.cn

#!/usr/bin/env bash
来源：http://hv.521024.cn

set -euo pipefail
来源：http://xu.szsharing.cn

[R02] 变量赋值与使用
来源：http://qu.chemitech.net.cn

name="Tom"; echo "$name"
来源：http://tz.szxytkj.cn

[R03] 只读变量
来源：http://un.jianghongdianzi.cn

readonly PI=3.14
来源：http://yt.shtwfgs.cn

[R04] 位置参数
来源：http://wj.huixinmuqiang.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://uc.haigaiapp.cn

[R05] 参数默认值
来源：http://ie.newstarts.cn

name="${1:-default}"
来源：http://sg.huixinmuqiang.cn

[R06] 判断命令是否存在
来源：http://ps.huanxung.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://cr.huanxung.cn

[R07] if 判断文件
来源：http://bm.newstarts.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://qo.gzmigu.cn

[R08] 数值比较
来源：http://wl.huixinmuqiang.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://fb.lnxyls.cn

[R09] 字符串比较
来源：http://sc.jianghongdianzi.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mj.9csxet.cn

[R10] 正则匹配
来源：http://ai.chemitech.net.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://iu.haigaiapp.cn

[R11] case 多分支
来源：http://wa.hahajie.cn

case "$1" in
来源：http://lf.jianghongdianzi.cn

start) echo "启动" ;;
来源：http://ga.hnjuh.cn

stop)  echo "停止" ;;
来源：http://rs.szxytkj.cn

*)     echo "未知命令" ;;
来源：http://wz.shxzukj.cn

esac
来源：http://vt.521024.cn

[R12] for 遍历文件
来源：http://cw.colortex.cn

for f in *.txt; do echo "$f"; done
来源：http://ep.hnjuh.cn

[R13] for 计数循环
来源：http://ys.huanxung.cn

for i in {1..10}; do echo "$i"; done
来源：http://vd.colortex.cn

[R14] C 风格 for
来源：http://bz.wgjwhj.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://aq.gzmigu.cn

[R15] while 逐行读文件
来源：http://bo.shxzskj.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://md.gzmigu.cn

[R16] until 等待条件
来源：http://dm.hahajie.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mz.huixiangedu.cn

[R17] 数组定义与取值
来源：http://sg.jctech888.com.cn

arr=(a b c); echo "${arr[0]}"
来源：http://hn.jctech888.com.cn

[R18] 遍历数组
来源：http://tl.asd995.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://yb.chemitech.net.cn

[R19] 数组长度
来源：http://lb.hnjuh.cn

echo "${#arr[@]}"
来源：http://eb.wgjwhj.cn

[R20] 关联数组（字典）
来源：http://ye.jianghongdianzi.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://dm.huixiangedu.cn

[R21] 字符串长度
来源：http://go.wgjwhj.cn

echo "${#s}"
来源：http://wu.lnxyls.cn

[R22] 截取子串
来源：http://vf.bookmarksfly.cn

echo "${s:0:5}"
来源：http://qj.chemitech.net.cn

[R23] 字符串替换
来源：http://vh.jctech888.com.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://zz.bookmarksfly.cn

[R24] 大小写转换
来源：http://nk.szsharing.cn

echo "${s^^}"; echo "${s,,}"
来源：http://mh.hahajie.cn

[R25] 去后缀 / 去前缀
来源：http://xc.9csxet.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://dd.hahajie.cn

[R26] 命令替换
来源：http://yu.9csxet.cn

now=$(date +%F); echo "$now"
来源：http://bu.lnxyls.cn

[R27] 算术展开
来源：http://qs.muxihuayi.cn

echo $((1 + 2 * 3))
来源：http://hx.huixiangedu.cn

[R28] 浮点运算
来源：http://hf.chemitech.net.cn

echo "scale=2; 10/3" | bc
来源：http://cq.9csxet.cn

[R29] 定义函数
来源：http://yf.9csxet.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://fs.gzmigu.cn

[R30] 函数返回状态码
来源：http://jc.szsharing.cn

f() { return 0; }; f || echo "失败了"
来源：http://bj.newstarts.cn

[R31] 局部变量
来源：http://df.huanxung.cn

f() { local x=1; echo "$x"; }
来源：http://xt.newstarts.cn

[R32] 参数个数校验
来源：http://qg.521024.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ym.gzmigu.cn

[R33] 捕获错误并提示行号
来源：http://ja.newstarts.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://oh.wgjwhj.cn

[R34] 退出时清理
来源：http://zl.huixiangedu.cn

trap 'rm -f "$tmp"' EXIT
来源：http://qy.yuntaijiaju.cn

[R35] 后台执行并等待
来源：http://ed.nicolike.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://xy.newstarts.cn

[R36] 并发执行多个任务
来源：http://gc.hnjuh.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://cy.lnxyls.cn

[R37] 把输出赋给变量
来源：http://bf.hnjuh.cn

files=$(ls -1)
来源：http://xg.szxytkj.cn

[R38] 管道串联
来源：http://du.asd995.cn

cat a.txt | grep -i error | wc -l
来源：http://kx.shxzskj.cn

[R39] 重定向标准输出与错误
来源：http://qv.shxzukj.cn

cmd > out.log 2>&1
来源：http://mc.shxzskj.cn

[R40] 追加写日志
来源：http://la.gzmigu.cn

echo "log" >> out.log
来源：http://sr.colortex.cn

[R41] 丢弃输出
来源：http://to.haigaiapp.cn

cmd >/dev/null 2>&1
来源：http://uf.szxytkj.cn

[R42] 输入重定向
来源：http://lc.newstarts.cn

wc -l < a.txt
来源：http://do.asd995.cn

[R43] 按名字查找文件
来源：http://rs.gzmigu.cn

find . -name "*.log" -type f
来源：http://yz.yuexingan06.cn

[R44] 按修改时间查找
来源：http://vk.bjjhwx.cn

find . -mtime -7 -type f
来源：http://ge.szsharing.cn

[R45] 批量删除
来源：http://zo.newstarts.cn

find . -name "*.tmp" -delete
来源：http://dy.nicolike.cn

[R46] 递归替换文件内容
来源：http://eu.haigaiapp.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://vz.jctech888.com.cn

[R47] sed 单行替换
来源：http://ki.haigaiapp.cn

sed -i 's/foo/bar/g' a.txt
来源：http://wk.panjiajie.cn

[R48] awk 取指定列
来源：http://rp.yuexingan06.cn

awk '{print $1, $3}' a.txt
来源：http://mc.szsharing.cn

[R49] awk 带条件
来源：http://tr.9csxet.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://xi.chemitech.net.cn

[R50] awk 求和
来源：http://iy.asd995.cn

awk '{s += $2} END {print s}' a.txt
来源：http://wg.bookmarksfly.cn

[R51] 排序去重取前几
来源：http://pi.colortex.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://cx.asd995.cn

[R52] 统计行数
来源：http://gr.wgjwhj.cn

wc -l a.txt
来源：http://db.szxytkj.cn

[R53] 查看文件头与实时尾
来源：http://jl.szsharing.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://aj.asd995.cn

[R54] 比较两个文件
来源：http://py.chemitech.net.cn

diff a.txt b.txt
来源：http://rt.panjiajie.cn

[R55] 压缩与解压
来源：http://lg.nszjky.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ku.asd995.cn

[R56] 远程拷贝
来源：http://ys.nszjky.cn

scp file user@host:/path/
来源：http://sb.9csxet.cn

[R57] 远程执行命令
来源：http://gg.shxzskj.cn

ssh user@host 'uptime'
来源：http://zl.huanxung.cn

[R58] 下载文件
来源：http://jo.huanxung.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wa.muxihuayi.cn

[R59] 发 POST JSON
来源：http://ua.jctech888.com.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wc.shtwfgs.cn

[R60] 只看 HTTP 状态码
来源：http://yb.bjjhwx.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://jw.shxzskj.cn

[R61] 磁盘占用
来源：http://kr.hnjuh.cn

df -h;  du -sh *
来源：http://pl.huanxung.cn

[R62] 找最占空间的文件
来源：http://vp.muxihuayi.cn

du -ah . | sort -rh | head -10
来源：http://oi.huanxung.cn

[R63] 内存与进程
来源：http://ss.nicolike.cn

free -h;  ps aux | grep nginx
来源：http://lk.bookmarksfly.cn

[R64] 结束进程
来源：http://tg.nicolike.cn

kill -9 $(pgrep -f app.py)
来源：http://ko.szxytkj.cn

[R65] 查看端口占用
来源：http://pg.szsharing.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://xw.szsharing.cn

[R66] 定时任务
来源：http://ps.shxzukj.cn

crontab -e;  crontab -l
来源：http://gc.muxihuayi.cn

[R67] 生成随机十六进制串
来源：http://cc.chemitech.net.cn


<!-- 参考信息 -->