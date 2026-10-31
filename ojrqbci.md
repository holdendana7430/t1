代发 wailian999

SELECT MAX(age), MIN(age) FROM users;
来源：http://uf.jctech888.com.cn

[Q30] 分组统计
来源：http://wn.colortex.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ky.jctech888.com.cn

[Q31] 分组后过滤
来源：http://ma.gzmigu.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://cp.wgjwhj.cn

[Q32] 分组拼接字符串
来源：http://mv.wgjwhj.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mv.gzmigu.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ba.gzmigu.cn

[Q33] 多列分组
来源：http://hh.shxzskj.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://qu.nicolike.cn

[Q34] 每组取第一条
来源：http://se.wgjwhj.cn

SELECT * FROM (
来源：http://tq.521024.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://av.hahajie.cn

) t WHERE rn = 1;
来源：http://ps.hnjuh.cn

[Q35] 内连接
来源：http://bu.huanxung.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://qi.shtwfgs.cn

[Q36] 左连接
来源：http://ga.jianghongdianzi.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://jq.9csxet.cn

[Q37] 右连接
来源：http://nu.lnxyls.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://jm.huixiangedu.cn

[Q38] 全外连接（PostgreSQL）
来源：http://dy.lnxyls.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://jz.shxzukj.cn

[Q39] 自连接（查上下级）
来源：http://du.huixinmuqiang.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://fe.yuexingan06.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://fw.asd995.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://tz.9csxet.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://bi.wgjwhj.cn

[Q41] 多表连接
来源：http://au.newstarts.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://yi.9csxet.cn

JOIN users u ON u.id = o.user_id
来源：http://zv.chemitech.net.cn

JOIN products p ON p.id = o.product_id;
来源：http://jn.shxzukj.cn

[Q42] 连接条件附加过滤
来源：http://yl.huixinmuqiang.cn

SELECT u.name, o.amount FROM users u
来源：http://ya.shxzukj.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ae.521024.cn

[Q43] 标量子查询
来源：http://hp.colortex.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://xv.szxytkj.cn

[Q44] IN 子查询
来源：http://ta.yuexingan06.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wp.huixinmuqiang.cn

[Q45] EXISTS 判断存在
来源：http://vm.gzmigu.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hw.bookmarksfly.cn

[Q46] NOT EXISTS 判断不存在
来源：http://bv.haigaiapp.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://lw.lnxyls.cn

[Q47] 与平均值比较
来源：http://hy.nszjky.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://in.yuntaijiaju.cn

[Q48] CTE 公用表表达式
来源：http://du.hnjuh.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://tr.9csxet.cn

SELECT * FROM t WHERE c > 5;
来源：http://ki.gzmigu.cn

[Q49] 更新单行
来源：http://xl.huixinmuqiang.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://em.yuexingan06.cn

[Q50] 批量更新
来源：http://yy.lnxyls.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://yz.521024.cn

[Q51] 用子查询更新
来源：http://jl.newstarts.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://ak.hnjuh.cn

[Q52] 删除指定行
来源：http://dg.nszjky.cn

DELETE FROM users WHERE id = 10;
来源：http://yl.panjiajie.cn

[Q53] 按条件删除
来源：http://ex.nicolike.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://qd.szsharing.cn

[Q54] 清空表
来源：http://ty.nszjky.cn

TRUNCATE TABLE logs;
来源：http://ag.bookmarksfly.cn

[Q55] 排名（并列占位）
来源：http://bd.521024.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hg.521024.cn

[Q56] 密集排名（并列不占位）
来源：http://ut.shxzukj.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hl.shtwfgs.cn

[Q57] 行号
来源：http://jn.wgjwhj.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wi.huixiangedu.cn

[Q58] 累计求和
来源：http://ht.shtwfgs.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hx.shxzukj.cn

[Q59] 分组内累计
来源：http://ib.521024.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://js.haigaiapp.cn

[Q60] 取上一行 / 下一行
来源：http://yi.szsharing.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://vk.haigaiapp.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://sw.chemitech.net.cn

[Q61] 移动平均
来源：http://zx.panjiajie.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ib.haigaiapp.cn

[Q62] 分组占比
来源：http://tx.szsharing.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wu.shxzukj.cn

[Q63] 开启事务
来源：http://yv.jianghongdianzi.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://yp.szsharing.cn

[Q64] 提交事务
来源：http://cq.szxytkj.cn

COMMIT;
来源：http://es.haigaiapp.cn

[Q65] 回滚事务
来源：http://yz.asd995.cn

ROLLBACK;
来源：http://gy.lnxyls.cn

[Q66] 行锁查询
来源：http://rr.hnjuh.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://gz.huixiangedu.cn

[Q67] 设置隔离级别
来源：http://mq.shxzskj.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ii.521024.cn

[Q68] 保存点
来源：http://gm.jctech888.com.cn

SAVEPOINT sp1;
来源：http://gk.panjiajie.cn

ROLLBACK TO sp1;
来源：http://wy.haigaiapp.cn

[Q69] 查看执行计划
来源：http://wo.shxzukj.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ju.jctech888.com.cn

[Q70] 更新统计信息
来源：http://mn.nszjky.cn

ANALYZE TABLE users;
来源：http://tw.colortex.cn

[Q71] 查看建表语句
来源：http://nq.bjjhwx.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://nm.jianghongdianzi.cn

[Q72] 查看索引
来源：http://al.szsharing.cn

SHOW INDEX FROM users;
来源：http://bk.521024.cn

[Q73] 查看表状态
来源：http://sr.huanxung.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://tv.huixinmuqiang.cn

[Q74] 强制使用索引
来源：http://jw.colortex.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://jc.jianghongdianzi.cn

[Q75] 日期格式化
来源：http://pu.haigaiapp.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://pu.hahajie.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://nt.bookmarksfly.cn

[Q76] 按天统计
来源：http://mb.nszjky.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hc.huanxung.cn

[Q77] 时间加减
来源：http://jk.jianghongdianzi.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://jv.huixinmuqiang.cn

[Q78] 当前时间
来源：http://nu.shxzukj.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://qv.nszjky.cn

[Q79] 字符串拼接
来源：http://am.newstarts.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ow.muxihuayi.cn

[Q80] 字符串截取
来源：http://eb.yuntaijiaju.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://pv.asd995.cn

[Q81] 字符串替换
来源：http://ww.lnxyls.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://dx.huixiangedu.cn

[Q82] 字符长度与字节长度
来源：http://si.jianghongdianzi.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://gs.szxytkj.cn

[Q83] 大小写转换
来源：http://kw.hahajie.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://th.nszjky.cn

[Q84] 去除首尾空格
来源：http://rh.nszjky.cn

SELECT TRIM(name) FROM users;
来源：http://fk.colortex.cn

[Q85] 数值取整
来源：http://rd.hnjuh.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://jm.asd995.cn

[Q86] 读取 JSON 字段
来源：http://ym.huixiangedu.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://pv.chemitech.net.cn

[Q87] JSON 字段做条件
来源：http://wm.521024.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://gv.shxzskj.cn

[Q88] 行转列（条件聚合）
来源：http://hp.chemitech.net.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://sc.wgjwhj.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mv.chemitech.net.cn

[Q89] 判断表是否存在
来源：http://xs.colortex.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://qq.panjiajie.cn

[Q90] 生成序号列
来源：http://pj.hnjuh.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://am.muxihuayi.cn

================================================================================
来源：http://be.521024.cn

R. Bash 专题
来源：http://sj.nicolike.cn

================================================================================
来源：http://nw.jianghongdianzi.cn

[R01] shebang 与严格模式
来源：http://wc.huanxung.cn

#!/usr/bin/env bash
来源：http://mh.panjiajie.cn

set -euo pipefail
来源：http://xh.shxzukj.cn

[R02] 变量赋值与使用
来源：http://by.hnjuh.cn

name="Tom"; echo "$name"
来源：http://xw.shxzukj.cn

[R03] 只读变量
来源：http://re.shxzskj.cn

readonly PI=3.14
来源：http://gx.bjjhwx.cn

[R04] 位置参数
来源：http://wi.yuexingan06.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://pz.nszjky.cn

[R05] 参数默认值
来源：http://os.hnjuh.cn

name="${1:-default}"
来源：http://is.colortex.cn

[R06] 判断命令是否存在
来源：http://gt.jctech888.com.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ez.shxzukj.cn

[R07] if 判断文件
来源：http://os.lnxyls.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://tw.huixinmuqiang.cn

[R08] 数值比较
来源：http://fw.jctech888.com.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://tj.yuntaijiaju.cn

[R09] 字符串比较
来源：http://no.gzmigu.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://xx.szxytkj.cn

[R10] 正则匹配
来源：http://pm.newstarts.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://lu.wgjwhj.cn

[R11] case 多分支
来源：http://wb.shxzskj.cn

case "$1" in
来源：http://pa.huixinmuqiang.cn

start) echo "启动" ;;
来源：http://vu.lnxyls.cn

stop)  echo "停止" ;;
来源：http://ga.huanxung.cn

*)     echo "未知命令" ;;
来源：http://bt.newstarts.cn

esac
来源：http://bi.shtwfgs.cn

[R12] for 遍历文件
来源：http://sd.huixiangedu.cn

for f in *.txt; do echo "$f"; done
来源：http://mf.hahajie.cn

[R13] for 计数循环
来源：http://tp.haigaiapp.cn

for i in {1..10}; do echo "$i"; done
来源：http://mj.szsharing.cn

[R14] C 风格 for
来源：http://mj.bookmarksfly.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://zh.haigaiapp.cn

[R15] while 逐行读文件
来源：http://zl.nicolike.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://di.521024.cn

[R16] until 等待条件
来源：http://nn.shtwfgs.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://yc.lnxyls.cn

[R17] 数组定义与取值
来源：http://tt.huanxung.cn

arr=(a b c); echo "${arr[0]}"
来源：http://ti.huanxung.cn

[R18] 遍历数组
来源：http://vu.newstarts.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wc.huanxung.cn

[R19] 数组长度
来源：http://nw.huixiangedu.cn

echo "${#arr[@]}"
来源：http://bg.szxytkj.cn

[R20] 关联数组（字典）
来源：http://zl.shxzukj.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ap.colortex.cn

[R21] 字符串长度
来源：http://yp.chemitech.net.cn

echo "${#s}"
来源：http://jk.hnjuh.cn

[R22] 截取子串
来源：http://mc.gzmigu.cn

echo "${s:0:5}"
来源：http://ml.bookmarksfly.cn

[R23] 字符串替换
来源：http://lf.yuntaijiaju.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://bo.9csxet.cn

[R24] 大小写转换
来源：http://fv.szsharing.cn

echo "${s^^}"; echo "${s,,}"
来源：http://os.bjjhwx.cn

[R25] 去后缀 / 去前缀
来源：http://ld.szxytkj.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://at.521024.cn

[R26] 命令替换
来源：http://dc.jctech888.com.cn

now=$(date +%F); echo "$now"
来源：http://ns.shxzukj.cn

[R27] 算术展开
来源：http://uo.wgjwhj.cn

echo $((1 + 2 * 3))
来源：http://gd.shxzskj.cn

[R28] 浮点运算
来源：http://ej.lnxyls.cn

echo "scale=2; 10/3" | bc
来源：http://aw.shxzukj.cn

[R29] 定义函数
来源：http://rv.shxzskj.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://dw.bjjhwx.cn

[R30] 函数返回状态码
来源：http://sy.szsharing.cn

f() { return 0; }; f || echo "失败了"
来源：http://sb.huixiangedu.cn

[R31] 局部变量
来源：http://pn.muxihuayi.cn

f() { local x=1; echo "$x"; }
来源：http://tz.hnjuh.cn

[R32] 参数个数校验
来源：http://lj.huixinmuqiang.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://bl.nicolike.cn

[R33] 捕获错误并提示行号
来源：http://hq.bjjhwx.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ut.nszjky.cn

[R34] 退出时清理
来源：http://zr.muxihuayi.cn

trap 'rm -f "$tmp"' EXIT
来源：http://ia.huixiangedu.cn

[R35] 后台执行并等待
来源：http://ts.huixiangedu.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://ib.lnxyls.cn

[R36] 并发执行多个任务
来源：http://wu.szsharing.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://kj.huanxung.cn

[R37] 把输出赋给变量
来源：http://un.nszjky.cn

files=$(ls -1)
来源：http://lu.chemitech.net.cn

[R38] 管道串联
来源：http://nb.bookmarksfly.cn

cat a.txt | grep -i error | wc -l
来源：http://fp.asd995.cn

[R39] 重定向标准输出与错误
来源：http://rk.szsharing.cn

cmd > out.log 2>&1
来源：http://an.szsharing.cn

[R40] 追加写日志
来源：http://fa.hahajie.cn

echo "log" >> out.log
来源：http://bc.shtwfgs.cn

[R41] 丢弃输出
来源：http://tl.colortex.cn

cmd >/dev/null 2>&1
来源：http://fg.bjjhwx.cn

[R42] 输入重定向
来源：http://dh.chemitech.net.cn

wc -l < a.txt
来源：http://wu.panjiajie.cn

[R43] 按名字查找文件
来源：http://rv.chemitech.net.cn

find . -name "*.log" -type f
来源：http://wk.nszjky.cn

[R44] 按修改时间查找
来源：http://zl.yuexingan06.cn

find . -mtime -7 -type f
来源：http://gr.521024.cn

[R45] 批量删除
来源：http://ls.jctech888.com.cn

find . -name "*.tmp" -delete
来源：http://ce.hahajie.cn

[R46] 递归替换文件内容
来源：http://rw.nicolike.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ez.haigaiapp.cn

[R47] sed 单行替换
来源：http://fn.gzmigu.cn

sed -i 's/foo/bar/g' a.txt
来源：http://km.shtwfgs.cn

[R48] awk 取指定列
来源：http://cv.newstarts.cn

awk '{print $1, $3}' a.txt
来源：http://jw.muxihuayi.cn

[R49] awk 带条件
来源：http://qn.szxytkj.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://bc.bjjhwx.cn

[R50] awk 求和
来源：http://mv.lnxyls.cn

awk '{s += $2} END {print s}' a.txt
来源：http://gr.yuntaijiaju.cn

[R51] 排序去重取前几
来源：http://hi.jctech888.com.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://ot.newstarts.cn

[R52] 统计行数
来源：http://rv.yuntaijiaju.cn

wc -l a.txt
来源：http://so.szxytkj.cn

[R53] 查看文件头与实时尾
来源：http://uk.bjjhwx.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://uv.wgjwhj.cn

[R54] 比较两个文件
来源：http://du.panjiajie.cn

diff a.txt b.txt
来源：http://is.panjiajie.cn

[R55] 压缩与解压
来源：http://ui.shxzskj.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://el.yuexingan06.cn

[R56] 远程拷贝
来源：http://hb.jctech888.com.cn

scp file user@host:/path/
来源：http://lc.jctech888.com.cn

[R57] 远程执行命令
来源：http://ao.hnjuh.cn

ssh user@host 'uptime'
来源：http://jg.huixiangedu.cn

[R58] 下载文件
来源：http://jy.hahajie.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://he.hahajie.cn

[R59] 发 POST JSON
来源：http://vt.jctech888.com.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://kz.521024.cn

[R60] 只看 HTTP 状态码
来源：http://em.hnjuh.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://il.muxihuayi.cn

[R61] 磁盘占用
来源：http://an.huixiangedu.cn

df -h;  du -sh *
来源：http://qd.yuexingan06.cn

[R62] 找最占空间的文件
来源：http://pt.yuexingan06.cn

du -ah . | sort -rh | head -10
来源：http://be.jianghongdianzi.cn

[R63] 内存与进程
来源：http://qw.yuexingan06.cn

free -h;  ps aux | grep nginx
来源：http://ds.shxzukj.cn

[R64] 结束进程
来源：http://cr.panjiajie.cn

kill -9 $(pgrep -f app.py)
来源：http://gy.nszjky.cn

[R65] 查看端口占用
来源：http://lu.bookmarksfly.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://rq.huanxung.cn

[R66] 定时任务
来源：http://xz.huanxung.cn

crontab -e;  crontab -l
来源：http://xz.hahajie.cn

[R67] 生成随机十六进制串
来源：http://od.jctech888.com.cn

openssl rand -hex 16
来源：http://rs.panjiajie.cn

[R68] 计算文件校验值
来源：http://mt.lnxyls.cn

sha256sum a.txt;  md5sum a.txt
来源：http://zi.gzmigu.cn

[R69] 生成随机密码
来源：http://ht.bjjhwx.cn

head -c 16 /dev/urandom | base64
来源：http://mh.shxzskj.cn

[R70] 时间戳与互转
来源：http://ja.shxzukj.cn

date +%s;  date -d @1700000000
来源：http://dk.shtwfgs.cn

[R71] 日期格式化
来源：http://yk.lnxyls.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://qd.newstarts.cn

[R72] 等待端口就绪
来源：http://zj.lnxyls.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://vd.bjjhwx.cn

[R73] 分割大日志
来源：http://hd.521024.cn

split -l 1000 big.log part_
来源：http://eu.nicolike.cn

[R74] 批量重命名
来源：http://xa.colortex.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://um.9csxet.cn

[R75] 导出环境变量
来源：http://cy.chemitech.net.cn

export PATH="$HOME/bin:$PATH"
来源：http://tb.szsharing.cn

[R76] 使用临时文件
来源：http://nq.bjjhwx.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ze.shxzskj.cn

[R77] 读取用户输入
来源：http://wo.szxytkj.cn

read -rp "请输入: " ans
来源：http://vr.jianghongdianzi.cn

[R78] 交互式菜单
来源：http://ll.yuntaijiaju.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://ek.wgjwhj.cn

[R79] 解析命令行选项
来源：http://rx.shxzskj.cn


<!-- 参考信息 -->