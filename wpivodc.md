代发 wailian999

[Q33] 多列分组
来源：http://qp.huixiangedu.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ig.521024.cn

[Q34] 每组取第一条
来源：http://rn.hahajie.cn

SELECT * FROM (
来源：http://np.szsharing.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://an.shxzskj.cn

) t WHERE rn = 1;
来源：http://ag.colortex.cn

[Q35] 内连接
来源：http://fy.lnxyls.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://rz.lnxyls.cn

[Q36] 左连接
来源：http://px.szxytkj.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://zm.huixinmuqiang.cn

[Q37] 右连接
来源：http://en.muxihuayi.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://lj.shxzukj.cn

[Q38] 全外连接（PostgreSQL）
来源：http://gz.521024.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://jq.panjiajie.cn

[Q39] 自连接（查上下级）
来源：http://ij.shxzukj.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://kd.shxzskj.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://il.newstarts.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://wh.newstarts.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://vz.yuntaijiaju.cn

[Q41] 多表连接
来源：http://gj.szxytkj.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://su.shxzskj.cn

JOIN users u ON u.id = o.user_id
来源：http://oi.shxzskj.cn

JOIN products p ON p.id = o.product_id;
来源：http://dc.9csxet.cn

[Q42] 连接条件附加过滤
来源：http://ba.haigaiapp.cn

SELECT u.name, o.amount FROM users u
来源：http://wa.jctech888.com.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hu.hnjuh.cn

[Q43] 标量子查询
来源：http://zs.asd995.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mv.jctech888.com.cn

[Q44] IN 子查询
来源：http://zw.yuexingan06.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://be.hnjuh.cn

[Q45] EXISTS 判断存在
来源：http://ly.hahajie.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ys.wgjwhj.cn

[Q46] NOT EXISTS 判断不存在
来源：http://et.bookmarksfly.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://fd.gzmigu.cn

[Q47] 与平均值比较
来源：http://dk.panjiajie.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://uz.bookmarksfly.cn

[Q48] CTE 公用表表达式
来源：http://ne.wgjwhj.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://kw.9csxet.cn

SELECT * FROM t WHERE c > 5;
来源：http://kl.nicolike.cn

[Q49] 更新单行
来源：http://mb.muxihuayi.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ty.9csxet.cn

[Q50] 批量更新
来源：http://eu.lnxyls.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://eh.nszjky.cn

[Q51] 用子查询更新
来源：http://kx.haigaiapp.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://ng.bookmarksfly.cn

[Q52] 删除指定行
来源：http://xf.newstarts.cn

DELETE FROM users WHERE id = 10;
来源：http://le.yuexingan06.cn

[Q53] 按条件删除
来源：http://uh.bookmarksfly.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://op.hahajie.cn

[Q54] 清空表
来源：http://lz.nszjky.cn

TRUNCATE TABLE logs;
来源：http://ej.wgjwhj.cn

[Q55] 排名（并列占位）
来源：http://fq.521024.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://pr.huixiangedu.cn

[Q56] 密集排名（并列不占位）
来源：http://ic.huixinmuqiang.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://cv.wgjwhj.cn

[Q57] 行号
来源：http://bm.shxzukj.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://so.huanxung.cn

[Q58] 累计求和
来源：http://lq.jctech888.com.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://eq.shxzukj.cn

[Q59] 分组内累计
来源：http://ev.shtwfgs.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://vl.lnxyls.cn

[Q60] 取上一行 / 下一行
来源：http://eo.haigaiapp.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ng.9csxet.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://yo.jianghongdianzi.cn

[Q61] 移动平均
来源：http://np.chemitech.net.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://xy.shtwfgs.cn

[Q62] 分组占比
来源：http://da.muxihuayi.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://jv.bookmarksfly.cn

[Q63] 开启事务
来源：http://zl.huixinmuqiang.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://vk.yuexingan06.cn

[Q64] 提交事务
来源：http://wi.jianghongdianzi.cn

COMMIT;
来源：http://pp.panjiajie.cn

[Q65] 回滚事务
来源：http://mt.jianghongdianzi.cn

ROLLBACK;
来源：http://dv.hnjuh.cn

[Q66] 行锁查询
来源：http://cb.asd995.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://bl.huanxung.cn

[Q67] 设置隔离级别
来源：http://en.huixiangedu.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://qc.colortex.cn

[Q68] 保存点
来源：http://yr.shxzukj.cn

SAVEPOINT sp1;
来源：http://vy.jctech888.com.cn

ROLLBACK TO sp1;
来源：http://gu.521024.cn

[Q69] 查看执行计划
来源：http://vv.huixiangedu.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ab.gzmigu.cn

[Q70] 更新统计信息
来源：http://dk.huixinmuqiang.cn

ANALYZE TABLE users;
来源：http://gr.shtwfgs.cn

[Q71] 查看建表语句
来源：http://pv.huixiangedu.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://bc.haigaiapp.cn

[Q72] 查看索引
来源：http://nf.yuntaijiaju.cn

SHOW INDEX FROM users;
来源：http://bv.bjjhwx.cn

[Q73] 查看表状态
来源：http://li.yuexingan06.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://eo.gzmigu.cn

[Q74] 强制使用索引
来源：http://cv.yuexingan06.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://xz.jianghongdianzi.cn

[Q75] 日期格式化
来源：http://ln.lnxyls.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://nu.nicolike.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://lz.nicolike.cn

[Q76] 按天统计
来源：http://kc.muxihuayi.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://fg.shtwfgs.cn

[Q77] 时间加减
来源：http://fc.panjiajie.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ky.bjjhwx.cn

[Q78] 当前时间
来源：http://oj.521024.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://nf.shxzukj.cn

[Q79] 字符串拼接
来源：http://qi.colortex.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://oi.bookmarksfly.cn

[Q80] 字符串截取
来源：http://ax.shtwfgs.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wv.shxzukj.cn

[Q81] 字符串替换
来源：http://kr.panjiajie.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://cp.huixiangedu.cn

[Q82] 字符长度与字节长度
来源：http://sc.9csxet.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://qx.shtwfgs.cn

[Q83] 大小写转换
来源：http://wa.hnjuh.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://on.colortex.cn

[Q84] 去除首尾空格
来源：http://ri.huanxung.cn

SELECT TRIM(name) FROM users;
来源：http://nj.wgjwhj.cn

[Q85] 数值取整
来源：http://pb.bookmarksfly.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://on.yuntaijiaju.cn

[Q86] 读取 JSON 字段
来源：http://vb.shtwfgs.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://il.huixinmuqiang.cn

[Q87] JSON 字段做条件
来源：http://lp.9csxet.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://vz.colortex.cn

[Q88] 行转列（条件聚合）
来源：http://th.yuntaijiaju.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://gu.szxytkj.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://cq.newstarts.cn

[Q89] 判断表是否存在
来源：http://ki.muxihuayi.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://qk.yuntaijiaju.cn

[Q90] 生成序号列
来源：http://fl.szsharing.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://fb.asd995.cn

================================================================================
来源：http://hf.haigaiapp.cn

R. Bash 专题
来源：http://ie.hahajie.cn

================================================================================
来源：http://dc.szxytkj.cn

[R01] shebang 与严格模式
来源：http://qu.yuntaijiaju.cn

#!/usr/bin/env bash
来源：http://vc.gzmigu.cn

set -euo pipefail
来源：http://th.szsharing.cn

[R02] 变量赋值与使用
来源：http://yj.chemitech.net.cn

name="Tom"; echo "$name"
来源：http://yk.huixinmuqiang.cn

[R03] 只读变量
来源：http://dq.gzmigu.cn

readonly PI=3.14
来源：http://ub.colortex.cn

[R04] 位置参数
来源：http://xh.colortex.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://kw.asd995.cn

[R05] 参数默认值
来源：http://ja.asd995.cn

name="${1:-default}"
来源：http://kw.szxytkj.cn

[R06] 判断命令是否存在
来源：http://iy.panjiajie.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ok.yuexingan06.cn

[R07] if 判断文件
来源：http://fk.gzmigu.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://yo.huixiangedu.cn

[R08] 数值比较
来源：http://ri.shxzukj.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://gh.hahajie.cn

[R09] 字符串比较
来源：http://gq.shxzukj.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ls.huixinmuqiang.cn

[R10] 正则匹配
来源：http://yc.jianghongdianzi.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://rs.521024.cn

[R11] case 多分支
来源：http://rg.muxihuayi.cn

case "$1" in
来源：http://ht.muxihuayi.cn

start) echo "启动" ;;
来源：http://vr.asd995.cn

stop)  echo "停止" ;;
来源：http://cx.szsharing.cn

*)     echo "未知命令" ;;
来源：http://st.huixinmuqiang.cn

esac
来源：http://sn.huanxung.cn

[R12] for 遍历文件
来源：http://zl.shxzskj.cn

for f in *.txt; do echo "$f"; done
来源：http://tx.shxzskj.cn

[R13] for 计数循环
来源：http://it.521024.cn

for i in {1..10}; do echo "$i"; done
来源：http://dy.hahajie.cn

[R14] C 风格 for
来源：http://jr.haigaiapp.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ne.shtwfgs.cn

[R15] while 逐行读文件
来源：http://wh.bookmarksfly.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wf.nszjky.cn

[R16] until 等待条件
来源：http://kc.newstarts.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ql.nszjky.cn

[R17] 数组定义与取值
来源：http://ip.szxytkj.cn

arr=(a b c); echo "${arr[0]}"
来源：http://fk.yuexingan06.cn

[R18] 遍历数组
来源：http://oj.yuexingan06.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://fw.nicolike.cn

[R19] 数组长度
来源：http://cy.haigaiapp.cn

echo "${#arr[@]}"
来源：http://on.huixiangedu.cn

[R20] 关联数组（字典）
来源：http://lc.jctech888.com.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://oj.bjjhwx.cn

[R21] 字符串长度
来源：http://ih.huixinmuqiang.cn

echo "${#s}"
来源：http://is.jianghongdianzi.cn

[R22] 截取子串
来源：http://xz.521024.cn

echo "${s:0:5}"
来源：http://fe.nszjky.cn

[R23] 字符串替换
来源：http://cr.shxzukj.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ju.bookmarksfly.cn

[R24] 大小写转换
来源：http://mm.521024.cn

echo "${s^^}"; echo "${s,,}"
来源：http://gq.jctech888.com.cn

[R25] 去后缀 / 去前缀
来源：http://wz.haigaiapp.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://jb.haigaiapp.cn

[R26] 命令替换
来源：http://au.521024.cn

now=$(date +%F); echo "$now"
来源：http://sc.shxzskj.cn

[R27] 算术展开
来源：http://vb.yuexingan06.cn

echo $((1 + 2 * 3))
来源：http://yz.shtwfgs.cn

[R28] 浮点运算
来源：http://kt.hahajie.cn

echo "scale=2; 10/3" | bc
来源：http://ii.yuntaijiaju.cn

[R29] 定义函数
来源：http://zu.muxihuayi.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://rh.9csxet.cn

[R30] 函数返回状态码
来源：http://ti.huixinmuqiang.cn

f() { return 0; }; f || echo "失败了"
来源：http://vk.lnxyls.cn

[R31] 局部变量
来源：http://xs.jctech888.com.cn

f() { local x=1; echo "$x"; }
来源：http://ug.yuexingan06.cn

[R32] 参数个数校验
来源：http://xk.9csxet.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://pz.huixiangedu.cn

[R33] 捕获错误并提示行号
来源：http://ov.yuntaijiaju.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ct.yuntaijiaju.cn

[R34] 退出时清理
来源：http://yd.9csxet.cn

trap 'rm -f "$tmp"' EXIT
来源：http://np.gzmigu.cn

[R35] 后台执行并等待
来源：http://th.hnjuh.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://np.szxytkj.cn

[R36] 并发执行多个任务
来源：http://se.asd995.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ij.chemitech.net.cn

[R37] 把输出赋给变量
来源：http://zr.panjiajie.cn

files=$(ls -1)
来源：http://tq.szxytkj.cn

[R38] 管道串联
来源：http://il.colortex.cn

cat a.txt | grep -i error | wc -l
来源：http://el.huixiangedu.cn

[R39] 重定向标准输出与错误
来源：http://sg.shxzskj.cn

cmd > out.log 2>&1
来源：http://df.bjjhwx.cn

[R40] 追加写日志
来源：http://ul.yuntaijiaju.cn

echo "log" >> out.log
来源：http://fo.gzmigu.cn

[R41] 丢弃输出
来源：http://sr.nszjky.cn

cmd >/dev/null 2>&1
来源：http://xk.yuexingan06.cn

[R42] 输入重定向
来源：http://sc.gzmigu.cn

wc -l < a.txt
来源：http://fn.panjiajie.cn

[R43] 按名字查找文件
来源：http://yy.jianghongdianzi.cn

find . -name "*.log" -type f
来源：http://ya.bookmarksfly.cn

[R44] 按修改时间查找
来源：http://rm.muxihuayi.cn

find . -mtime -7 -type f
来源：http://mj.huixinmuqiang.cn

[R45] 批量删除
来源：http://wo.huanxung.cn

find . -name "*.tmp" -delete
来源：http://nt.asd995.cn

[R46] 递归替换文件内容
来源：http://og.asd995.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ff.lnxyls.cn

[R47] sed 单行替换
来源：http://vu.hahajie.cn

sed -i 's/foo/bar/g' a.txt
来源：http://ry.colortex.cn

[R48] awk 取指定列
来源：http://yv.szsharing.cn

awk '{print $1, $3}' a.txt
来源：http://zd.nszjky.cn

[R49] awk 带条件
来源：http://cx.9csxet.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wq.huanxung.cn

[R50] awk 求和
来源：http://ts.gzmigu.cn

awk '{s += $2} END {print s}' a.txt
来源：http://to.hahajie.cn

[R51] 排序去重取前几
来源：http://jl.huanxung.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://xi.chemitech.net.cn

[R52] 统计行数
来源：http://zq.haigaiapp.cn

wc -l a.txt
来源：http://jj.hnjuh.cn

[R53] 查看文件头与实时尾
来源：http://pj.panjiajie.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://rj.shxzukj.cn

[R54] 比较两个文件
来源：http://ih.chemitech.net.cn

diff a.txt b.txt
来源：http://ay.521024.cn

[R55] 压缩与解压
来源：http://qw.gzmigu.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://lc.jianghongdianzi.cn

[R56] 远程拷贝
来源：http://ix.521024.cn

scp file user@host:/path/
来源：http://bs.jctech888.com.cn

[R57] 远程执行命令
来源：http://mq.gzmigu.cn

ssh user@host 'uptime'
来源：http://fz.huixinmuqiang.cn

[R58] 下载文件
来源：http://iz.shtwfgs.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hl.jianghongdianzi.cn

[R59] 发 POST JSON
来源：http://ke.szxytkj.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://uh.wgjwhj.cn

[R60] 只看 HTTP 状态码
来源：http://xl.huixiangedu.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://oc.haigaiapp.cn

[R61] 磁盘占用
来源：http://ej.lnxyls.cn

df -h;  du -sh *
来源：http://ie.wgjwhj.cn

[R62] 找最占空间的文件
来源：http://fj.gzmigu.cn

du -ah . | sort -rh | head -10
来源：http://ew.521024.cn

[R63] 内存与进程
来源：http://kj.bookmarksfly.cn

free -h;  ps aux | grep nginx
来源：http://wb.jianghongdianzi.cn

[R64] 结束进程
来源：http://zj.shxzukj.cn

kill -9 $(pgrep -f app.py)
来源：http://xs.nicolike.cn

[R65] 查看端口占用
来源：http://gt.colortex.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://du.huixinmuqiang.cn

[R66] 定时任务
来源：http://sm.asd995.cn

crontab -e;  crontab -l
来源：http://dd.hnjuh.cn

[R67] 生成随机十六进制串
来源：http://kb.haigaiapp.cn

openssl rand -hex 16
来源：http://jb.yuntaijiaju.cn

[R68] 计算文件校验值
来源：http://lc.jctech888.com.cn

sha256sum a.txt;  md5sum a.txt
来源：http://sk.szsharing.cn

[R69] 生成随机密码
来源：http://pe.jctech888.com.cn

head -c 16 /dev/urandom | base64
来源：http://jt.yuntaijiaju.cn

[R70] 时间戳与互转
来源：http://pa.yuntaijiaju.cn

date +%s;  date -d @1700000000
来源：http://hl.chemitech.net.cn

[R71] 日期格式化
来源：http://va.shtwfgs.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://ar.panjiajie.cn

[R72] 等待端口就绪
来源：http://ft.yuntaijiaju.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://gt.hnjuh.cn

[R73] 分割大日志
来源：http://at.9csxet.cn

split -l 1000 big.log part_
来源：http://re.huixiangedu.cn

[R74] 批量重命名
来源：http://ar.521024.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ce.9csxet.cn

[R75] 导出环境变量
来源：http://sd.jctech888.com.cn

export PATH="$HOME/bin:$PATH"
来源：http://ew.szsharing.cn

[R76] 使用临时文件
来源：http://tz.jianghongdianzi.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hf.nszjky.cn

[R77] 读取用户输入
来源：http://rn.haigaiapp.cn

read -rp "请输入: " ans
来源：http://vc.yuexingan06.cn

[R78] 交互式菜单
来源：http://rm.colortex.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://xs.huixinmuqiang.cn

[R79] 解析命令行选项
来源：http://sb.panjiajie.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hr.huixinmuqiang.cn

[R80] 查看脚本执行耗时
来源：http://ge.muxihuayi.cn

time ./run.sh
来源：http://dj.yuexingan06.cn

================================================================================
来源：http://fg.newstarts.cn

S. C / C++ 专题
来源：http://nz.chemitech.net.cn

================================================================================
来源：http://qs.lnxyls.cn

[S01] C：Hello World
来源：http://je.shxzskj.cn

#include <stdio.h>
来源：http://uz.jianghongdianzi.cn


<!-- 参考信息 -->