代发 wailian999

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://dl.hnjuh.cn

[Q20] IN 列表
来源：http://ig.huixinmuqiang.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://iz.shxzskj.cn

[Q21] 空值判断
来源：http://ja.bookmarksfly.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://fa.szxytkj.cn

[Q22] 排序
来源：http://au.shxzskj.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://xx.shxzukj.cn

[Q23] 分页
来源：http://ix.lnxyls.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://pt.muxihuayi.cn

[Q24] 去重
来源：http://ab.lnxyls.cn

SELECT DISTINCT city FROM users;
来源：http://mm.huanxung.cn

[Q25] 只取前 N 条
来源：http://wm.nicolike.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ya.szxytkj.cn

[Q26] 计数
来源：http://sy.gzmigu.cn

SELECT COUNT(*) FROM users;
来源：http://rk.huixinmuqiang.cn

[Q27] 条件计数
来源：http://yy.521024.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://eu.haigaiapp.cn

[Q28] 求和与平均
来源：http://cb.szsharing.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://ke.521024.cn

[Q29] 最大最小值
来源：http://jq.yuntaijiaju.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://tr.lnxyls.cn

[Q30] 分组统计
来源：http://dt.yuntaijiaju.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hv.yuexingan06.cn

[Q31] 分组后过滤
来源：http://oz.lnxyls.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://uu.szsharing.cn

[Q32] 分组拼接字符串
来源：http://dk.chemitech.net.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://zo.yuexingan06.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ww.jianghongdianzi.cn

[Q33] 多列分组
来源：http://xa.hnjuh.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://de.nszjky.cn

[Q34] 每组取第一条
来源：http://px.bjjhwx.cn

SELECT * FROM (
来源：http://vc.gzmigu.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://bw.shxzskj.cn

) t WHERE rn = 1;
来源：http://xh.hnjuh.cn

[Q35] 内连接
来源：http://um.yuexingan06.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://kc.szxytkj.cn

[Q36] 左连接
来源：http://wr.nicolike.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://nw.gzmigu.cn

[Q37] 右连接
来源：http://ix.9csxet.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://xc.colortex.cn

[Q38] 全外连接（PostgreSQL）
来源：http://er.szxytkj.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ct.gzmigu.cn

[Q39] 自连接（查上下级）
来源：http://xx.521024.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://cm.gzmigu.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://kt.bookmarksfly.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://fh.newstarts.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ov.yuexingan06.cn

[Q41] 多表连接
来源：http://hf.wgjwhj.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://ff.chemitech.net.cn

JOIN users u ON u.id = o.user_id
来源：http://rp.yuntaijiaju.cn

JOIN products p ON p.id = o.product_id;
来源：http://nv.9csxet.cn

[Q42] 连接条件附加过滤
来源：http://vl.muxihuayi.cn

SELECT u.name, o.amount FROM users u
来源：http://kn.newstarts.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://tq.yuexingan06.cn

[Q43] 标量子查询
来源：http://oy.jctech888.com.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://fz.bookmarksfly.cn

[Q44] IN 子查询
来源：http://iu.jianghongdianzi.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://rf.jianghongdianzi.cn

[Q45] EXISTS 判断存在
来源：http://yt.hnjuh.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://cj.9csxet.cn

[Q46] NOT EXISTS 判断不存在
来源：http://yw.bjjhwx.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://vr.521024.cn

[Q47] 与平均值比较
来源：http://sq.521024.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://cf.yuntaijiaju.cn

[Q48] CTE 公用表表达式
来源：http://cu.jctech888.com.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://xf.yuntaijiaju.cn

SELECT * FROM t WHERE c > 5;
来源：http://lv.nicolike.cn

[Q49] 更新单行
来源：http://ur.shtwfgs.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://dd.yuntaijiaju.cn

[Q50] 批量更新
来源：http://ik.wgjwhj.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://lm.lnxyls.cn

[Q51] 用子查询更新
来源：http://iz.panjiajie.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://op.colortex.cn

[Q52] 删除指定行
来源：http://xj.jianghongdianzi.cn

DELETE FROM users WHERE id = 10;
来源：http://gs.newstarts.cn

[Q53] 按条件删除
来源：http://ks.lnxyls.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://zo.jctech888.com.cn

[Q54] 清空表
来源：http://zz.yuexingan06.cn

TRUNCATE TABLE logs;
来源：http://gs.colortex.cn

[Q55] 排名（并列占位）
来源：http://pk.huixinmuqiang.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://kf.yuntaijiaju.cn

[Q56] 密集排名（并列不占位）
来源：http://rx.huanxung.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://rq.haigaiapp.cn

[Q57] 行号
来源：http://vc.yuexingan06.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://uy.521024.cn

[Q58] 累计求和
来源：http://lb.chemitech.net.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wt.panjiajie.cn

[Q59] 分组内累计
来源：http://jg.asd995.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://az.nicolike.cn

[Q60] 取上一行 / 下一行
来源：http://nu.bjjhwx.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://xt.hnjuh.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://li.shxzskj.cn

[Q61] 移动平均
来源：http://jy.wgjwhj.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://nx.jianghongdianzi.cn

[Q62] 分组占比
来源：http://yh.newstarts.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ew.chemitech.net.cn

[Q63] 开启事务
来源：http://yf.panjiajie.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://mh.huanxung.cn

[Q64] 提交事务
来源：http://fr.huanxung.cn

COMMIT;
来源：http://ru.shxzskj.cn

[Q65] 回滚事务
来源：http://em.huixinmuqiang.cn

ROLLBACK;
来源：http://kr.gzmigu.cn

[Q66] 行锁查询
来源：http://vp.chemitech.net.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ao.colortex.cn

[Q67] 设置隔离级别
来源：http://vl.huanxung.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ex.huanxung.cn

[Q68] 保存点
来源：http://jb.muxihuayi.cn

SAVEPOINT sp1;
来源：http://jr.nszjky.cn

ROLLBACK TO sp1;
来源：http://zx.muxihuayi.cn

[Q69] 查看执行计划
来源：http://pt.muxihuayi.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://cl.newstarts.cn

[Q70] 更新统计信息
来源：http://ua.wgjwhj.cn

ANALYZE TABLE users;
来源：http://jk.521024.cn

[Q71] 查看建表语句
来源：http://yy.9csxet.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://tn.chemitech.net.cn

[Q72] 查看索引
来源：http://lu.yuexingan06.cn

SHOW INDEX FROM users;
来源：http://vn.nszjky.cn

[Q73] 查看表状态
来源：http://ac.bookmarksfly.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://fq.muxihuayi.cn

[Q74] 强制使用索引
来源：http://za.9csxet.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://nk.hahajie.cn

[Q75] 日期格式化
来源：http://ap.colortex.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://uz.nicolike.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wz.asd995.cn

[Q76] 按天统计
来源：http://dt.nszjky.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://vl.jctech888.com.cn

[Q77] 时间加减
来源：http://td.nszjky.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mk.nszjky.cn

[Q78] 当前时间
来源：http://tm.huanxung.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://kq.wgjwhj.cn

[Q79] 字符串拼接
来源：http://cj.9csxet.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wx.szxytkj.cn

[Q80] 字符串截取
来源：http://bh.nicolike.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wp.newstarts.cn

[Q81] 字符串替换
来源：http://kn.bookmarksfly.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ex.asd995.cn

[Q82] 字符长度与字节长度
来源：http://op.szxytkj.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mf.szsharing.cn

[Q83] 大小写转换
来源：http://ne.haigaiapp.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://pk.lnxyls.cn

[Q84] 去除首尾空格
来源：http://il.szxytkj.cn

SELECT TRIM(name) FROM users;
来源：http://uk.haigaiapp.cn

[Q85] 数值取整
来源：http://kf.huixinmuqiang.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ul.9csxet.cn

[Q86] 读取 JSON 字段
来源：http://ut.521024.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://dq.hnjuh.cn

[Q87] JSON 字段做条件
来源：http://pq.hnjuh.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ei.yuntaijiaju.cn

[Q88] 行转列（条件聚合）
来源：http://qg.yuexingan06.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ao.muxihuayi.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wt.nszjky.cn

[Q89] 判断表是否存在
来源：http://cc.hnjuh.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://az.szsharing.cn

[Q90] 生成序号列
来源：http://dw.shtwfgs.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ou.nszjky.cn

================================================================================
来源：http://ei.jianghongdianzi.cn

R. Bash 专题
来源：http://mb.bjjhwx.cn

================================================================================
来源：http://zv.panjiajie.cn

[R01] shebang 与严格模式
来源：http://li.shxzskj.cn

#!/usr/bin/env bash
来源：http://cx.shxzskj.cn

set -euo pipefail
来源：http://tt.newstarts.cn

[R02] 变量赋值与使用
来源：http://iy.szsharing.cn

name="Tom"; echo "$name"
来源：http://mn.jctech888.com.cn

[R03] 只读变量
来源：http://nv.szsharing.cn

readonly PI=3.14
来源：http://kd.panjiajie.cn

[R04] 位置参数
来源：http://rk.bjjhwx.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ji.9csxet.cn

[R05] 参数默认值
来源：http://mk.shxzukj.cn

name="${1:-default}"
来源：http://up.wgjwhj.cn

[R06] 判断命令是否存在
来源：http://oo.shxzskj.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://lr.haigaiapp.cn

[R07] if 判断文件
来源：http://tn.bookmarksfly.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://sg.huanxung.cn

[R08] 数值比较
来源：http://zm.huixiangedu.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.bjjhwx.cn

[R09] 字符串比较
来源：http://ti.wgjwhj.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hr.newstarts.cn

[R10] 正则匹配
来源：http://ii.yuntaijiaju.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://sv.yuexingan06.cn

[R11] case 多分支
来源：http://cd.shtwfgs.cn

case "$1" in
来源：http://dv.huixinmuqiang.cn

start) echo "启动" ;;
来源：http://cx.shtwfgs.cn

stop)  echo "停止" ;;
来源：http://ci.jianghongdianzi.cn

*)     echo "未知命令" ;;
来源：http://gj.9csxet.cn

esac
来源：http://vd.nszjky.cn

[R12] for 遍历文件
来源：http://bt.yuntaijiaju.cn

for f in *.txt; do echo "$f"; done
来源：http://yw.szxytkj.cn

[R13] for 计数循环
来源：http://dt.haigaiapp.cn

for i in {1..10}; do echo "$i"; done
来源：http://zv.hnjuh.cn

[R14] C 风格 for
来源：http://qa.huanxung.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://uv.huixinmuqiang.cn

[R15] while 逐行读文件
来源：http://hb.huixinmuqiang.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://id.nszjky.cn

[R16] until 等待条件
来源：http://bj.szsharing.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ez.521024.cn

[R17] 数组定义与取值
来源：http://gi.szsharing.cn

arr=(a b c); echo "${arr[0]}"
来源：http://bk.nicolike.cn

[R18] 遍历数组
来源：http://zp.jctech888.com.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ow.hnjuh.cn

[R19] 数组长度
来源：http://lv.newstarts.cn

echo "${#arr[@]}"
来源：http://oz.muxihuayi.cn

[R20] 关联数组（字典）
来源：http://gp.shxzukj.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wn.jianghongdianzi.cn

[R21] 字符串长度
来源：http://ns.shtwfgs.cn

echo "${#s}"
来源：http://sz.muxihuayi.cn

[R22] 截取子串
来源：http://wv.521024.cn

echo "${s:0:5}"
来源：http://mu.shtwfgs.cn

[R23] 字符串替换
来源：http://sh.jctech888.com.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://lk.jctech888.com.cn

[R24] 大小写转换
来源：http://xa.jianghongdianzi.cn

echo "${s^^}"; echo "${s,,}"
来源：http://nc.yuexingan06.cn

[R25] 去后缀 / 去前缀
来源：http://ec.haigaiapp.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://dd.colortex.cn

[R26] 命令替换
来源：http://ks.newstarts.cn

now=$(date +%F); echo "$now"
来源：http://nf.yuexingan06.cn

[R27] 算术展开
来源：http://io.jianghongdianzi.cn

echo $((1 + 2 * 3))
来源：http://yb.muxihuayi.cn

[R28] 浮点运算
来源：http://od.bjjhwx.cn

echo "scale=2; 10/3" | bc
来源：http://yf.wgjwhj.cn

[R29] 定义函数
来源：http://yv.colortex.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://jv.shxzskj.cn

[R30] 函数返回状态码
来源：http://go.bjjhwx.cn

f() { return 0; }; f || echo "失败了"
来源：http://mq.9csxet.cn

[R31] 局部变量
来源：http://vr.9csxet.cn

f() { local x=1; echo "$x"; }
来源：http://dq.chemitech.net.cn

[R32] 参数个数校验
来源：http://zc.9csxet.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wr.huixinmuqiang.cn

[R33] 捕获错误并提示行号
来源：http://ah.lnxyls.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://go.szsharing.cn

[R34] 退出时清理
来源：http://gv.521024.cn

trap 'rm -f "$tmp"' EXIT
来源：http://tu.huixinmuqiang.cn

[R35] 后台执行并等待
来源：http://rc.muxihuayi.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://yo.lnxyls.cn

[R36] 并发执行多个任务
来源：http://yg.9csxet.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ap.newstarts.cn

[R37] 把输出赋给变量
来源：http://dn.chemitech.net.cn

files=$(ls -1)
来源：http://rf.muxihuayi.cn

[R38] 管道串联
来源：http://km.yuntaijiaju.cn

cat a.txt | grep -i error | wc -l
来源：http://ff.huixinmuqiang.cn

[R39] 重定向标准输出与错误
来源：http://nh.bjjhwx.cn

cmd > out.log 2>&1
来源：http://fl.huixinmuqiang.cn

[R40] 追加写日志
来源：http://mm.colortex.cn

echo "log" >> out.log
来源：http://nk.jianghongdianzi.cn

[R41] 丢弃输出
来源：http://sb.yuexingan06.cn

cmd >/dev/null 2>&1
来源：http://aj.huixiangedu.cn

[R42] 输入重定向
来源：http://jo.jianghongdianzi.cn

wc -l < a.txt
来源：http://sv.szsharing.cn

[R43] 按名字查找文件
来源：http://jd.jctech888.com.cn

find . -name "*.log" -type f
来源：http://rg.bjjhwx.cn

[R44] 按修改时间查找
来源：http://kc.newstarts.cn

find . -mtime -7 -type f
来源：http://qj.hahajie.cn

[R45] 批量删除
来源：http://us.hahajie.cn

find . -name "*.tmp" -delete
来源：http://bu.huixiangedu.cn

[R46] 递归替换文件内容
来源：http://so.szsharing.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ne.colortex.cn

[R47] sed 单行替换
来源：http://yy.521024.cn

sed -i 's/foo/bar/g' a.txt
来源：http://xi.shxzukj.cn

[R48] awk 取指定列
来源：http://cl.hahajie.cn

awk '{print $1, $3}' a.txt
来源：http://ku.huixiangedu.cn

[R49] awk 带条件
来源：http://cu.shxzukj.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ln.asd995.cn

[R50] awk 求和
来源：http://ze.hahajie.cn

awk '{s += $2} END {print s}' a.txt
来源：http://yz.bjjhwx.cn

[R51] 排序去重取前几
来源：http://rn.bjjhwx.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://cs.shxzskj.cn

[R52] 统计行数
来源：http://mv.yuexingan06.cn

wc -l a.txt
来源：http://qw.chemitech.net.cn

[R53] 查看文件头与实时尾
来源：http://bb.lnxyls.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://py.huixiangedu.cn

[R54] 比较两个文件
来源：http://rv.szxytkj.cn

diff a.txt b.txt
来源：http://nv.lnxyls.cn

[R55] 压缩与解压
来源：http://ah.huixiangedu.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://tm.colortex.cn

[R56] 远程拷贝
来源：http://cu.521024.cn

scp file user@host:/path/
来源：http://tu.lnxyls.cn

[R57] 远程执行命令
来源：http://zv.lnxyls.cn

ssh user@host 'uptime'
来源：http://kg.yuexingan06.cn

[R58] 下载文件
来源：http://da.bjjhwx.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://xq.hnjuh.cn

[R59] 发 POST JSON
来源：http://kb.bjjhwx.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://fi.colortex.cn

[R60] 只看 HTTP 状态码
来源：http://oa.szxytkj.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://tk.huixiangedu.cn

[R61] 磁盘占用
来源：http://km.nicolike.cn

df -h;  du -sh *
来源：http://hx.jianghongdianzi.cn

[R62] 找最占空间的文件
来源：http://xv.521024.cn

du -ah . | sort -rh | head -10
来源：http://ru.shxzukj.cn

[R63] 内存与进程
来源：http://eh.9csxet.cn

free -h;  ps aux | grep nginx
来源：http://gh.huixiangedu.cn

[R64] 结束进程
来源：http://rq.jianghongdianzi.cn

kill -9 $(pgrep -f app.py)
来源：http://xv.yuntaijiaju.cn

[R65] 查看端口占用
来源：http://iz.wgjwhj.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://kc.szsharing.cn

[R66] 定时任务
来源：http://ac.asd995.cn

crontab -e;  crontab -l
来源：http://kz.gzmigu.cn

[R67] 生成随机十六进制串
来源：http://tj.gzmigu.cn

openssl rand -hex 16
来源：http://pj.huixiangedu.cn

[R68] 计算文件校验值
来源：http://wv.huixinmuqiang.cn

sha256sum a.txt;  md5sum a.txt
来源：http://jx.jctech888.com.cn

[R69] 生成随机密码
来源：http://yo.shxzskj.cn


<!-- 参考信息 -->