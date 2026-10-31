代发 wailian999

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ot.huixinmuqiang.cn

[Q20] IN 列表
来源：http://ie.bjjhwx.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://vw.panjiajie.cn

[Q21] 空值判断
来源：http://ym.szxytkj.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://bj.hahajie.cn

[Q22] 排序
来源：http://tp.jctech888.com.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ri.haigaiapp.cn

[Q23] 分页
来源：http://ta.wgjwhj.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://jl.shxzskj.cn

[Q24] 去重
来源：http://xs.jianghongdianzi.cn

SELECT DISTINCT city FROM users;
来源：http://jt.nicolike.cn

[Q25] 只取前 N 条
来源：http://fw.gzmigu.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://qq.chemitech.net.cn

[Q26] 计数
来源：http://xx.asd995.cn

SELECT COUNT(*) FROM users;
来源：http://ee.szxytkj.cn

[Q27] 条件计数
来源：http://sg.gzmigu.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ap.colortex.cn

[Q28] 求和与平均
来源：http://nl.gzmigu.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://rx.gzmigu.cn

[Q29] 最大最小值
来源：http://sz.newstarts.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://mt.hahajie.cn

[Q30] 分组统计
来源：http://qk.muxihuayi.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://pj.chemitech.net.cn

[Q31] 分组后过滤
来源：http://al.521024.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wc.huanxung.cn

[Q32] 分组拼接字符串
来源：http://ie.bookmarksfly.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://zl.haigaiapp.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://fd.yuexingan06.cn

[Q33] 多列分组
来源：http://hm.bookmarksfly.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://bu.panjiajie.cn

[Q34] 每组取第一条
来源：http://wm.hnjuh.cn

SELECT * FROM (
来源：http://gy.szxytkj.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://qk.hahajie.cn

) t WHERE rn = 1;
来源：http://dw.521024.cn

[Q35] 内连接
来源：http://mw.szxytkj.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://cd.muxihuayi.cn

[Q36] 左连接
来源：http://bg.haigaiapp.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hm.shxzskj.cn

[Q37] 右连接
来源：http://fp.huixiangedu.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ze.chemitech.net.cn

[Q38] 全外连接（PostgreSQL）
来源：http://pq.newstarts.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://su.newstarts.cn

[Q39] 自连接（查上下级）
来源：http://lt.bjjhwx.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://uv.lnxyls.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ij.huixiangedu.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://sr.huixinmuqiang.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://yt.chemitech.net.cn

[Q41] 多表连接
来源：http://ek.chemitech.net.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://uz.chemitech.net.cn

JOIN users u ON u.id = o.user_id
来源：http://rn.gzmigu.cn

JOIN products p ON p.id = o.product_id;
来源：http://ts.gzmigu.cn

[Q42] 连接条件附加过滤
来源：http://ov.colortex.cn

SELECT u.name, o.amount FROM users u
来源：http://br.panjiajie.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://bg.yuntaijiaju.cn

[Q43] 标量子查询
来源：http://ze.9csxet.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://bb.bookmarksfly.cn

[Q44] IN 子查询
来源：http://ow.asd995.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://zv.yuexingan06.cn

[Q45] EXISTS 判断存在
来源：http://hd.colortex.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://gs.nicolike.cn

[Q46] NOT EXISTS 判断不存在
来源：http://pz.hahajie.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://yl.yuntaijiaju.cn

[Q47] 与平均值比较
来源：http://ex.huanxung.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://iv.huixinmuqiang.cn

[Q48] CTE 公用表表达式
来源：http://vc.wgjwhj.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://bd.nicolike.cn

SELECT * FROM t WHERE c > 5;
来源：http://xx.9csxet.cn

[Q49] 更新单行
来源：http://hx.szsharing.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://nk.bjjhwx.cn

[Q50] 批量更新
来源：http://od.huanxung.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://ii.lnxyls.cn

[Q51] 用子查询更新
来源：http://py.shxzskj.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://je.nicolike.cn

[Q52] 删除指定行
来源：http://jb.yuntaijiaju.cn

DELETE FROM users WHERE id = 10;
来源：http://rk.chemitech.net.cn

[Q53] 按条件删除
来源：http://gw.gzmigu.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wv.colortex.cn

[Q54] 清空表
来源：http://ez.nicolike.cn

TRUNCATE TABLE logs;
来源：http://pn.hnjuh.cn

[Q55] 排名（并列占位）
来源：http://yd.haigaiapp.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://me.hahajie.cn

[Q56] 密集排名（并列不占位）
来源：http://wi.gzmigu.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://nh.newstarts.cn

[Q57] 行号
来源：http://wp.shtwfgs.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://av.bjjhwx.cn

[Q58] 累计求和
来源：http://ty.colortex.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://yy.nicolike.cn

[Q59] 分组内累计
来源：http://pn.huixinmuqiang.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://nb.hnjuh.cn

[Q60] 取上一行 / 下一行
来源：http://jc.huixinmuqiang.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mk.nszjky.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wv.shxzukj.cn

[Q61] 移动平均
来源：http://hk.haigaiapp.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://xw.bookmarksfly.cn

[Q62] 分组占比
来源：http://mi.yuntaijiaju.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://gn.shxzskj.cn

[Q63] 开启事务
来源：http://ti.asd995.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://tu.szxytkj.cn

[Q64] 提交事务
来源：http://dt.nszjky.cn

COMMIT;
来源：http://jl.lnxyls.cn

[Q65] 回滚事务
来源：http://ev.9csxet.cn

ROLLBACK;
来源：http://kv.nszjky.cn

[Q66] 行锁查询
来源：http://ea.shxzukj.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://az.nicolike.cn

[Q67] 设置隔离级别
来源：http://ot.newstarts.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://dk.newstarts.cn

[Q68] 保存点
来源：http://iy.szsharing.cn

SAVEPOINT sp1;
来源：http://xh.colortex.cn

ROLLBACK TO sp1;
来源：http://ii.shtwfgs.cn

[Q69] 查看执行计划
来源：http://qv.hahajie.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://sl.yuntaijiaju.cn

[Q70] 更新统计信息
来源：http://yk.szxytkj.cn

ANALYZE TABLE users;
来源：http://zf.szsharing.cn

[Q71] 查看建表语句
来源：http://fe.yuntaijiaju.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://aw.shtwfgs.cn

[Q72] 查看索引
来源：http://dv.colortex.cn

SHOW INDEX FROM users;
来源：http://av.colortex.cn

[Q73] 查看表状态
来源：http://za.shxzukj.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://yj.szsharing.cn

[Q74] 强制使用索引
来源：http://je.huixinmuqiang.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://pa.haigaiapp.cn

[Q75] 日期格式化
来源：http://co.jianghongdianzi.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wx.hnjuh.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://gm.nicolike.cn

[Q76] 按天统计
来源：http://pf.yuexingan06.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://da.huixinmuqiang.cn

[Q77] 时间加减
来源：http://cu.jianghongdianzi.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://fc.huanxung.cn

[Q78] 当前时间
来源：http://eq.huixinmuqiang.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://zu.9csxet.cn

[Q79] 字符串拼接
来源：http://oi.newstarts.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://as.hnjuh.cn

[Q80] 字符串截取
来源：http://qf.szxytkj.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mc.huanxung.cn

[Q81] 字符串替换
来源：http://ro.nicolike.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ng.wgjwhj.cn

[Q82] 字符长度与字节长度
来源：http://cg.9csxet.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ty.huanxung.cn

[Q83] 大小写转换
来源：http://ur.muxihuayi.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://rr.huanxung.cn

[Q84] 去除首尾空格
来源：http://xo.panjiajie.cn

SELECT TRIM(name) FROM users;
来源：http://gt.hnjuh.cn

[Q85] 数值取整
来源：http://gf.huanxung.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://eg.haigaiapp.cn

[Q86] 读取 JSON 字段
来源：http://jd.jctech888.com.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ou.haigaiapp.cn

[Q87] JSON 字段做条件
来源：http://fm.shtwfgs.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://to.jctech888.com.cn

[Q88] 行转列（条件聚合）
来源：http://lh.muxihuayi.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mr.hahajie.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ik.panjiajie.cn

[Q89] 判断表是否存在
来源：http://lz.bjjhwx.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://we.nicolike.cn

[Q90] 生成序号列
来源：http://vx.asd995.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://rp.bjjhwx.cn

================================================================================
来源：http://rb.9csxet.cn

R. Bash 专题
来源：http://cf.bookmarksfly.cn

================================================================================
来源：http://jx.muxihuayi.cn

[R01] shebang 与严格模式
来源：http://ad.bookmarksfly.cn

#!/usr/bin/env bash
来源：http://ae.huanxung.cn

set -euo pipefail
来源：http://uh.shxzukj.cn

[R02] 变量赋值与使用
来源：http://sm.colortex.cn

name="Tom"; echo "$name"
来源：http://sp.chemitech.net.cn

[R03] 只读变量
来源：http://td.shxzskj.cn

readonly PI=3.14
来源：http://jp.yuntaijiaju.cn

[R04] 位置参数
来源：http://rd.huanxung.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://su.huixinmuqiang.cn

[R05] 参数默认值
来源：http://xa.shxzukj.cn

name="${1:-default}"
来源：http://ih.lnxyls.cn

[R06] 判断命令是否存在
来源：http://em.szsharing.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hb.hnjuh.cn

[R07] if 判断文件
来源：http://rh.hahajie.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://to.huixinmuqiang.cn

[R08] 数值比较
来源：http://fa.szsharing.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://wb.lnxyls.cn

[R09] 字符串比较
来源：http://cq.jctech888.com.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://nm.colortex.cn

[R10] 正则匹配
来源：http://px.huixinmuqiang.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://px.shxzskj.cn

[R11] case 多分支
来源：http://nn.newstarts.cn

case "$1" in
来源：http://pi.jianghongdianzi.cn

start) echo "启动" ;;
来源：http://bf.szxytkj.cn

stop)  echo "停止" ;;
来源：http://rd.lnxyls.cn

*)     echo "未知命令" ;;
来源：http://bx.panjiajie.cn

esac
来源：http://os.bookmarksfly.cn

[R12] for 遍历文件
来源：http://zn.chemitech.net.cn

for f in *.txt; do echo "$f"; done
来源：http://ot.panjiajie.cn

[R13] for 计数循环
来源：http://ps.wgjwhj.cn

for i in {1..10}; do echo "$i"; done
来源：http://vv.nicolike.cn

[R14] C 风格 for
来源：http://si.huixinmuqiang.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://fm.huixinmuqiang.cn

[R15] while 逐行读文件
来源：http://dp.shxzukj.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ml.colortex.cn

[R16] until 等待条件
来源：http://qr.lnxyls.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://tq.muxihuayi.cn

[R17] 数组定义与取值
来源：http://sn.shtwfgs.cn

arr=(a b c); echo "${arr[0]}"
来源：http://se.9csxet.cn

[R18] 遍历数组
来源：http://nn.bjjhwx.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ln.yuexingan06.cn

[R19] 数组长度
来源：http://vc.bookmarksfly.cn

echo "${#arr[@]}"
来源：http://nc.jctech888.com.cn

[R20] 关联数组（字典）
来源：http://qu.bookmarksfly.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://os.gzmigu.cn

[R21] 字符串长度
来源：http://st.9csxet.cn

echo "${#s}"
来源：http://dr.shxzukj.cn

[R22] 截取子串
来源：http://as.hnjuh.cn

echo "${s:0:5}"
来源：http://mh.yuntaijiaju.cn

[R23] 字符串替换
来源：http://as.haigaiapp.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://zh.wgjwhj.cn

[R24] 大小写转换
来源：http://ay.shxzukj.cn

echo "${s^^}"; echo "${s,,}"
来源：http://xj.hahajie.cn

[R25] 去后缀 / 去前缀
来源：http://vm.yuntaijiaju.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://wv.nszjky.cn

[R26] 命令替换
来源：http://sy.hnjuh.cn

now=$(date +%F); echo "$now"
来源：http://iv.muxihuayi.cn

[R27] 算术展开
来源：http://pz.shxzskj.cn

echo $((1 + 2 * 3))
来源：http://sn.chemitech.net.cn

[R28] 浮点运算
来源：http://oo.shxzskj.cn

echo "scale=2; 10/3" | bc
来源：http://kp.hahajie.cn

[R29] 定义函数
来源：http://js.chemitech.net.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://gq.hnjuh.cn

[R30] 函数返回状态码
来源：http://in.shxzukj.cn

f() { return 0; }; f || echo "失败了"
来源：http://hy.muxihuayi.cn

[R31] 局部变量
来源：http://tf.muxihuayi.cn

f() { local x=1; echo "$x"; }
来源：http://le.asd995.cn

[R32] 参数个数校验
来源：http://ee.jianghongdianzi.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://co.lnxyls.cn

[R33] 捕获错误并提示行号
来源：http://bo.wgjwhj.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://dl.huanxung.cn

[R34] 退出时清理
来源：http://vy.szxytkj.cn

trap 'rm -f "$tmp"' EXIT
来源：http://rv.9csxet.cn

[R35] 后台执行并等待
来源：http://fl.panjiajie.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://ii.shtwfgs.cn

[R36] 并发执行多个任务
来源：http://ny.panjiajie.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hw.wgjwhj.cn

[R37] 把输出赋给变量
来源：http://ox.hahajie.cn

files=$(ls -1)
来源：http://gr.asd995.cn

[R38] 管道串联
来源：http://lr.chemitech.net.cn

cat a.txt | grep -i error | wc -l
来源：http://ri.wgjwhj.cn

[R39] 重定向标准输出与错误
来源：http://sy.nszjky.cn

cmd > out.log 2>&1
来源：http://cu.haigaiapp.cn

[R40] 追加写日志
来源：http://ts.jctech888.com.cn

echo "log" >> out.log
来源：http://er.shxzskj.cn

[R41] 丢弃输出
来源：http://nx.haigaiapp.cn

cmd >/dev/null 2>&1
来源：http://bw.huixiangedu.cn

[R42] 输入重定向
来源：http://wd.hnjuh.cn

wc -l < a.txt
来源：http://ln.nszjky.cn

[R43] 按名字查找文件
来源：http://nt.jctech888.com.cn

find . -name "*.log" -type f
来源：http://tp.asd995.cn

[R44] 按修改时间查找
来源：http://cc.nszjky.cn

find . -mtime -7 -type f
来源：http://mh.colortex.cn

[R45] 批量删除
来源：http://qk.bookmarksfly.cn

find . -name "*.tmp" -delete
来源：http://ci.lnxyls.cn

[R46] 递归替换文件内容
来源：http://bp.shtwfgs.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://zp.jianghongdianzi.cn

[R47] sed 单行替换
来源：http://kz.muxihuayi.cn

sed -i 's/foo/bar/g' a.txt
来源：http://ja.shxzskj.cn

[R48] awk 取指定列
来源：http://yp.shxzukj.cn

awk '{print $1, $3}' a.txt
来源：http://pm.jianghongdianzi.cn

[R49] awk 带条件
来源：http://wt.huanxung.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://fh.yuntaijiaju.cn

[R50] awk 求和
来源：http://ww.shxzskj.cn

awk '{s += $2} END {print s}' a.txt
来源：http://ve.asd995.cn

[R51] 排序去重取前几
来源：http://nt.huanxung.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://ru.colortex.cn

[R52] 统计行数
来源：http://oq.newstarts.cn

wc -l a.txt
来源：http://pw.huixinmuqiang.cn

[R53] 查看文件头与实时尾
来源：http://xg.hahajie.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://yg.muxihuayi.cn

[R54] 比较两个文件
来源：http://wq.szsharing.cn

diff a.txt b.txt
来源：http://ej.muxihuayi.cn

[R55] 压缩与解压
来源：http://ch.wgjwhj.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://er.lnxyls.cn

[R56] 远程拷贝
来源：http://ax.521024.cn

scp file user@host:/path/
来源：http://qw.bjjhwx.cn

[R57] 远程执行命令
来源：http://ug.newstarts.cn

ssh user@host 'uptime'
来源：http://rf.jianghongdianzi.cn

[R58] 下载文件
来源：http://tj.huixiangedu.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://fm.nicolike.cn

[R59] 发 POST JSON
来源：http://mw.yuexingan06.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://rn.szxytkj.cn

[R60] 只看 HTTP 状态码
来源：http://zs.nszjky.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://is.lnxyls.cn

[R61] 磁盘占用
来源：http://tc.colortex.cn

df -h;  du -sh *
来源：http://be.newstarts.cn

[R62] 找最占空间的文件
来源：http://mg.asd995.cn

du -ah . | sort -rh | head -10
来源：http://yf.newstarts.cn

[R63] 内存与进程
来源：http://vt.yuntaijiaju.cn

free -h;  ps aux | grep nginx
来源：http://fh.shxzskj.cn

[R64] 结束进程
来源：http://zo.gzmigu.cn

kill -9 $(pgrep -f app.py)
来源：http://qz.panjiajie.cn

[R65] 查看端口占用
来源：http://oo.asd995.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://rm.yuntaijiaju.cn

[R66] 定时任务
来源：http://et.asd995.cn

crontab -e;  crontab -l
来源：http://lz.shxzskj.cn

[R67] 生成随机十六进制串
来源：http://ro.bjjhwx.cn

openssl rand -hex 16
来源：http://gk.newstarts.cn

[R68] 计算文件校验值
来源：http://gr.haigaiapp.cn

sha256sum a.txt;  md5sum a.txt
来源：http://kj.colortex.cn

[R69] 生成随机密码
来源：http://xf.shxzukj.cn


<!-- 参考信息 -->