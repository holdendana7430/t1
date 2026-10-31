代发 wailian999

SELECT MAX(age), MIN(age) FROM users;
来源：http://qh.521024.cn

[Q30] 分组统计
来源：http://bt.shxzukj.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://vf.gzmigu.cn

[Q31] 分组后过滤
来源：http://ri.gzmigu.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://nz.panjiajie.cn

[Q32] 分组拼接字符串
来源：http://xz.panjiajie.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://pj.nszjky.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ow.jianghongdianzi.cn

[Q33] 多列分组
来源：http://tj.newstarts.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://bn.chemitech.net.cn

[Q34] 每组取第一条
来源：http://gx.hnjuh.cn

SELECT * FROM (
来源：http://qv.bjjhwx.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://xk.chemitech.net.cn

) t WHERE rn = 1;
来源：http://va.newstarts.cn

[Q35] 内连接
来源：http://sz.colortex.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://vd.9csxet.cn

[Q36] 左连接
来源：http://bk.shxzukj.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://lr.yuexingan06.cn

[Q37] 右连接
来源：http://cm.haigaiapp.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://uq.yuexingan06.cn

[Q38] 全外连接（PostgreSQL）
来源：http://wi.muxihuayi.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://eo.yuexingan06.cn

[Q39] 自连接（查上下级）
来源：http://na.gzmigu.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://xd.shtwfgs.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://rq.szsharing.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://tx.huixinmuqiang.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ds.hnjuh.cn

[Q41] 多表连接
来源：http://rn.haigaiapp.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://zh.shxzskj.cn

JOIN users u ON u.id = o.user_id
来源：http://mv.huanxung.cn

JOIN products p ON p.id = o.product_id;
来源：http://fc.shxzukj.cn

[Q42] 连接条件附加过滤
来源：http://oe.lnxyls.cn

SELECT u.name, o.amount FROM users u
来源：http://pv.bookmarksfly.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://dr.panjiajie.cn

[Q43] 标量子查询
来源：http://nn.521024.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://ao.shxzukj.cn

[Q44] IN 子查询
来源：http://cn.jctech888.com.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://pf.newstarts.cn

[Q45] EXISTS 判断存在
来源：http://bx.jctech888.com.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://fo.asd995.cn

[Q46] NOT EXISTS 判断不存在
来源：http://xk.jianghongdianzi.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://cw.jianghongdianzi.cn

[Q47] 与平均值比较
来源：http://pw.521024.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://gu.chemitech.net.cn

[Q48] CTE 公用表表达式
来源：http://di.huanxung.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://lf.wgjwhj.cn

SELECT * FROM t WHERE c > 5;
来源：http://es.haigaiapp.cn

[Q49] 更新单行
来源：http://nt.panjiajie.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://lp.bookmarksfly.cn

[Q50] 批量更新
来源：http://bs.muxihuayi.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://fv.jctech888.com.cn

[Q51] 用子查询更新
来源：http://ek.jctech888.com.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hj.521024.cn

[Q52] 删除指定行
来源：http://cf.szxytkj.cn

DELETE FROM users WHERE id = 10;
来源：http://gn.huanxung.cn

[Q53] 按条件删除
来源：http://nm.huanxung.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ls.szxytkj.cn

[Q54] 清空表
来源：http://hc.newstarts.cn

TRUNCATE TABLE logs;
来源：http://ww.shtwfgs.cn

[Q55] 排名（并列占位）
来源：http://zt.hnjuh.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ki.lnxyls.cn

[Q56] 密集排名（并列不占位）
来源：http://ap.nszjky.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://yf.9csxet.cn

[Q57] 行号
来源：http://wz.gzmigu.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://cu.huanxung.cn

[Q58] 累计求和
来源：http://aw.szsharing.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://aw.muxihuayi.cn

[Q59] 分组内累计
来源：http://xs.shtwfgs.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://th.nicolike.cn

[Q60] 取上一行 / 下一行
来源：http://bl.hnjuh.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://uh.chemitech.net.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mb.jctech888.com.cn

[Q61] 移动平均
来源：http://le.yuntaijiaju.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ah.521024.cn

[Q62] 分组占比
来源：http://tu.yuexingan06.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mc.huixinmuqiang.cn

[Q63] 开启事务
来源：http://fk.szxytkj.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://hf.bjjhwx.cn

[Q64] 提交事务
来源：http://ae.yuexingan06.cn

COMMIT;
来源：http://xn.shtwfgs.cn

[Q65] 回滚事务
来源：http://av.9csxet.cn

ROLLBACK;
来源：http://az.shxzukj.cn

[Q66] 行锁查询
来源：http://vf.9csxet.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://tk.shxzukj.cn

[Q67] 设置隔离级别
来源：http://da.szxytkj.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://bo.huixiangedu.cn

[Q68] 保存点
来源：http://hn.chemitech.net.cn

SAVEPOINT sp1;
来源：http://ty.wgjwhj.cn

ROLLBACK TO sp1;
来源：http://uf.szsharing.cn

[Q69] 查看执行计划
来源：http://rf.szxytkj.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wv.huixiangedu.cn

[Q70] 更新统计信息
来源：http://be.newstarts.cn

ANALYZE TABLE users;
来源：http://uk.muxihuayi.cn

[Q71] 查看建表语句
来源：http://xn.lnxyls.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://po.hahajie.cn

[Q72] 查看索引
来源：http://yz.bjjhwx.cn

SHOW INDEX FROM users;
来源：http://xp.newstarts.cn

[Q73] 查看表状态
来源：http://vp.chemitech.net.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://qw.shtwfgs.cn

[Q74] 强制使用索引
来源：http://ok.jctech888.com.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://kx.bookmarksfly.cn

[Q75] 日期格式化
来源：http://we.lnxyls.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://zs.yuntaijiaju.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://go.hahajie.cn

[Q76] 按天统计
来源：http://yv.jianghongdianzi.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://bd.shtwfgs.cn

[Q77] 时间加减
来源：http://qr.bjjhwx.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ek.shtwfgs.cn

[Q78] 当前时间
来源：http://eg.szxytkj.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://fv.bjjhwx.cn

[Q79] 字符串拼接
来源：http://ji.shxzskj.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://xb.nszjky.cn

[Q80] 字符串截取
来源：http://fo.shxzukj.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ap.jianghongdianzi.cn

[Q81] 字符串替换
来源：http://oz.jianghongdianzi.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ic.gzmigu.cn

[Q82] 字符长度与字节长度
来源：http://aq.nicolike.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://qn.hahajie.cn

[Q83] 大小写转换
来源：http://ds.bookmarksfly.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ex.muxihuayi.cn

[Q84] 去除首尾空格
来源：http://yf.haigaiapp.cn

SELECT TRIM(name) FROM users;
来源：http://yz.shxzskj.cn

[Q85] 数值取整
来源：http://eu.szxytkj.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ah.huanxung.cn

[Q86] 读取 JSON 字段
来源：http://ag.colortex.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://jk.nszjky.cn

[Q87] JSON 字段做条件
来源：http://rn.bjjhwx.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://qa.gzmigu.cn

[Q88] 行转列（条件聚合）
来源：http://ze.521024.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://iy.nszjky.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://yu.jctech888.com.cn

[Q89] 判断表是否存在
来源：http://pv.bjjhwx.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://yo.szsharing.cn

[Q90] 生成序号列
来源：http://js.shxzskj.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://vt.chemitech.net.cn

================================================================================
来源：http://nk.asd995.cn

R. Bash 专题
来源：http://ia.shxzskj.cn

================================================================================
来源：http://pc.jctech888.com.cn

[R01] shebang 与严格模式
来源：http://fr.bjjhwx.cn

#!/usr/bin/env bash
来源：http://ku.szsharing.cn

set -euo pipefail
来源：http://xn.bookmarksfly.cn

[R02] 变量赋值与使用
来源：http://kj.szsharing.cn

name="Tom"; echo "$name"
来源：http://gx.haigaiapp.cn

[R03] 只读变量
来源：http://qh.shxzskj.cn

readonly PI=3.14
来源：http://fy.haigaiapp.cn

[R04] 位置参数
来源：http://ku.9csxet.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://om.bookmarksfly.cn

[R05] 参数默认值
来源：http://jx.yuexingan06.cn

name="${1:-default}"
来源：http://us.szsharing.cn

[R06] 判断命令是否存在
来源：http://oa.huixinmuqiang.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://jn.521024.cn

[R07] if 判断文件
来源：http://xz.bjjhwx.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://lw.hahajie.cn

[R08] 数值比较
来源：http://ds.szsharing.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://ir.huanxung.cn

[R09] 字符串比较
来源：http://cc.9csxet.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://gp.jianghongdianzi.cn

[R10] 正则匹配
来源：http://ra.shxzskj.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://cv.shxzukj.cn

[R11] case 多分支
来源：http://zi.bjjhwx.cn

case "$1" in
来源：http://hh.lnxyls.cn

start) echo "启动" ;;
来源：http://rk.lnxyls.cn

stop)  echo "停止" ;;
来源：http://us.shxzukj.cn

*)     echo "未知命令" ;;
来源：http://ch.shxzukj.cn

esac
来源：http://ur.bjjhwx.cn

[R12] for 遍历文件
来源：http://mn.asd995.cn

for f in *.txt; do echo "$f"; done
来源：http://ee.hahajie.cn

[R13] for 计数循环
来源：http://rc.yuntaijiaju.cn

for i in {1..10}; do echo "$i"; done
来源：http://zs.nicolike.cn

[R14] C 风格 for
来源：http://xk.yuexingan06.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://lk.shtwfgs.cn

[R15] while 逐行读文件
来源：http://zs.huixinmuqiang.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://bu.asd995.cn

[R16] until 等待条件
来源：http://ev.szsharing.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ue.szxytkj.cn

[R17] 数组定义与取值
来源：http://ci.hahajie.cn

arr=(a b c); echo "${arr[0]}"
来源：http://eb.szsharing.cn

[R18] 遍历数组
来源：http://bv.shxzukj.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://sb.yuexingan06.cn

[R19] 数组长度
来源：http://ot.521024.cn

echo "${#arr[@]}"
来源：http://hj.asd995.cn

[R20] 关联数组（字典）
来源：http://xz.yuntaijiaju.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://kk.hahajie.cn

[R21] 字符串长度
来源：http://cm.colortex.cn

echo "${#s}"
来源：http://av.shtwfgs.cn

[R22] 截取子串
来源：http://xo.hnjuh.cn

echo "${s:0:5}"
来源：http://lp.yuntaijiaju.cn

[R23] 字符串替换
来源：http://ms.wgjwhj.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://nq.newstarts.cn

[R24] 大小写转换
来源：http://vj.huixiangedu.cn

echo "${s^^}"; echo "${s,,}"
来源：http://fa.shxzskj.cn

[R25] 去后缀 / 去前缀
来源：http://xc.huixiangedu.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://md.szxytkj.cn

[R26] 命令替换
来源：http://gb.bjjhwx.cn

now=$(date +%F); echo "$now"
来源：http://ke.nszjky.cn

[R27] 算术展开
来源：http://uv.hahajie.cn

echo $((1 + 2 * 3))
来源：http://mq.hahajie.cn

[R28] 浮点运算
来源：http://bq.shtwfgs.cn

echo "scale=2; 10/3" | bc
来源：http://bn.chemitech.net.cn

[R29] 定义函数
来源：http://pl.521024.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://oo.nszjky.cn

[R30] 函数返回状态码
来源：http://bg.nicolike.cn

f() { return 0; }; f || echo "失败了"
来源：http://xo.szsharing.cn

[R31] 局部变量
来源：http://kw.szsharing.cn

f() { local x=1; echo "$x"; }
来源：http://vu.shxzukj.cn

[R32] 参数个数校验
来源：http://mn.gzmigu.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://qs.jianghongdianzi.cn

[R33] 捕获错误并提示行号
来源：http://mg.shtwfgs.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://yy.huixiangedu.cn

[R34] 退出时清理
来源：http://gy.newstarts.cn

trap 'rm -f "$tmp"' EXIT
来源：http://ic.muxihuayi.cn

[R35] 后台执行并等待
来源：http://ct.bjjhwx.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://xg.huixinmuqiang.cn

[R36] 并发执行多个任务
来源：http://ru.muxihuayi.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hq.521024.cn

[R37] 把输出赋给变量
来源：http://lx.panjiajie.cn

files=$(ls -1)
来源：http://dt.haigaiapp.cn

[R38] 管道串联
来源：http://di.shxzskj.cn

cat a.txt | grep -i error | wc -l
来源：http://ni.hahajie.cn

[R39] 重定向标准输出与错误
来源：http://mn.yuexingan06.cn

cmd > out.log 2>&1
来源：http://yb.shxzskj.cn

[R40] 追加写日志
来源：http://mb.haigaiapp.cn

echo "log" >> out.log
来源：http://rx.huixiangedu.cn

[R41] 丢弃输出
来源：http://ta.panjiajie.cn

cmd >/dev/null 2>&1
来源：http://qj.gzmigu.cn

[R42] 输入重定向
来源：http://tb.wgjwhj.cn

wc -l < a.txt
来源：http://aj.yuntaijiaju.cn

[R43] 按名字查找文件
来源：http://ei.nicolike.cn

find . -name "*.log" -type f
来源：http://qj.hahajie.cn

[R44] 按修改时间查找
来源：http://na.jianghongdianzi.cn

find . -mtime -7 -type f
来源：http://ze.nszjky.cn

[R45] 批量删除
来源：http://gs.bjjhwx.cn

find . -name "*.tmp" -delete
来源：http://rh.hahajie.cn

[R46] 递归替换文件内容
来源：http://rg.bjjhwx.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://xo.jctech888.com.cn

[R47] sed 单行替换
来源：http://yy.chemitech.net.cn

sed -i 's/foo/bar/g' a.txt
来源：http://xe.asd995.cn

[R48] awk 取指定列
来源：http://rq.huanxung.cn

awk '{print $1, $3}' a.txt
来源：http://yy.yuexingan06.cn

[R49] awk 带条件
来源：http://wt.colortex.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ia.newstarts.cn

[R50] awk 求和
来源：http://cj.hnjuh.cn

awk '{s += $2} END {print s}' a.txt
来源：http://lq.szsharing.cn

[R51] 排序去重取前几
来源：http://qw.haigaiapp.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://nr.panjiajie.cn

[R52] 统计行数
来源：http://ly.jctech888.com.cn

wc -l a.txt
来源：http://hx.asd995.cn

[R53] 查看文件头与实时尾
来源：http://sy.wgjwhj.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://kv.panjiajie.cn

[R54] 比较两个文件
来源：http://ek.huanxung.cn

diff a.txt b.txt
来源：http://rq.szxytkj.cn

[R55] 压缩与解压
来源：http://ld.hahajie.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://qw.shtwfgs.cn

[R56] 远程拷贝
来源：http://ac.chemitech.net.cn

scp file user@host:/path/
来源：http://up.huixiangedu.cn

[R57] 远程执行命令
来源：http://qd.jctech888.com.cn

ssh user@host 'uptime'
来源：http://bi.jianghongdianzi.cn

[R58] 下载文件
来源：http://je.panjiajie.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://yb.lnxyls.cn

[R59] 发 POST JSON
来源：http://jf.hnjuh.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ck.lnxyls.cn

[R60] 只看 HTTP 状态码
来源：http://tc.huanxung.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://xt.jctech888.com.cn

[R61] 磁盘占用
来源：http://hs.jianghongdianzi.cn

df -h;  du -sh *
来源：http://du.nicolike.cn

[R62] 找最占空间的文件
来源：http://uv.hahajie.cn

du -ah . | sort -rh | head -10
来源：http://kj.szsharing.cn

[R63] 内存与进程
来源：http://et.newstarts.cn

free -h;  ps aux | grep nginx
来源：http://bi.lnxyls.cn

[R64] 结束进程
来源：http://gs.panjiajie.cn

kill -9 $(pgrep -f app.py)
来源：http://qo.haigaiapp.cn

[R65] 查看端口占用
来源：http://na.huixiangedu.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://dj.lnxyls.cn

[R66] 定时任务
来源：http://xq.szsharing.cn

crontab -e;  crontab -l
来源：http://nd.nicolike.cn

[R67] 生成随机十六进制串
来源：http://qa.szxytkj.cn

openssl rand -hex 16
来源：http://kz.shxzskj.cn

[R68] 计算文件校验值
来源：http://cc.yuexingan06.cn

sha256sum a.txt;  md5sum a.txt
来源：http://bn.bookmarksfly.cn

[R69] 生成随机密码
来源：http://nn.shxzskj.cn

head -c 16 /dev/urandom | base64
来源：http://nj.bjjhwx.cn

[R70] 时间戳与互转
来源：http://km.yuntaijiaju.cn

date +%s;  date -d @1700000000
来源：http://qh.colortex.cn

[R71] 日期格式化
来源：http://md.szxytkj.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://eu.lnxyls.cn

[R72] 等待端口就绪
来源：http://wl.panjiajie.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://lq.bookmarksfly.cn

[R73] 分割大日志
来源：http://bk.hnjuh.cn

split -l 1000 big.log part_
来源：http://fu.muxihuayi.cn

[R74] 批量重命名
来源：http://sb.huanxung.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://xc.shxzukj.cn

[R75] 导出环境变量
来源：http://bh.huanxung.cn

export PATH="$HOME/bin:$PATH"
来源：http://gm.nszjky.cn

[R76] 使用临时文件
来源：http://me.yuntaijiaju.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://is.huixiangedu.cn

[R77] 读取用户输入
来源：http://fr.panjiajie.cn

read -rp "请输入: " ans
来源：http://mg.szsharing.cn

[R78] 交互式菜单
来源：http://fh.newstarts.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://md.nicolike.cn

[R79] 解析命令行选项
来源：http://gy.chemitech.net.cn


<!-- 参考信息 -->