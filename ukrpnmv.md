代发 wailian999

[Q33] 多列分组
来源：http://tg.shtwfgs.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://lc.gzmigu.cn

[Q34] 每组取第一条
来源：http://vl.jctech888.com.cn

SELECT * FROM (
来源：http://en.nicolike.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ju.yuexingan06.cn

) t WHERE rn = 1;
来源：http://xf.hnjuh.cn

[Q35] 内连接
来源：http://sn.hahajie.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ly.shtwfgs.cn

[Q36] 左连接
来源：http://nv.nszjky.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://no.shtwfgs.cn

[Q37] 右连接
来源：http://ku.szsharing.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mq.colortex.cn

[Q38] 全外连接（PostgreSQL）
来源：http://ql.yuexingan06.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://gv.shxzukj.cn

[Q39] 自连接（查上下级）
来源：http://kn.wgjwhj.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://yw.muxihuayi.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://kd.haigaiapp.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://my.hnjuh.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://kh.nszjky.cn

[Q41] 多表连接
来源：http://sb.9csxet.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://lk.bjjhwx.cn

JOIN users u ON u.id = o.user_id
来源：http://kg.9csxet.cn

JOIN products p ON p.id = o.product_id;
来源：http://hk.nszjky.cn

[Q42] 连接条件附加过滤
来源：http://wd.shxzukj.cn

SELECT u.name, o.amount FROM users u
来源：http://hh.jianghongdianzi.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://vr.panjiajie.cn

[Q43] 标量子查询
来源：http://ee.shxzukj.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://fd.panjiajie.cn

[Q44] IN 子查询
来源：http://gt.haigaiapp.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://jm.newstarts.cn

[Q45] EXISTS 判断存在
来源：http://lg.hahajie.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://zh.shtwfgs.cn

[Q46] NOT EXISTS 判断不存在
来源：http://br.nszjky.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ob.szxytkj.cn

[Q47] 与平均值比较
来源：http://dy.lnxyls.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ld.jctech888.com.cn

[Q48] CTE 公用表表达式
来源：http://ak.shtwfgs.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wv.jianghongdianzi.cn

SELECT * FROM t WHERE c > 5;
来源：http://zo.chemitech.net.cn

[Q49] 更新单行
来源：http://uo.panjiajie.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ey.hahajie.cn

[Q50] 批量更新
来源：http://sd.9csxet.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://zj.shxzskj.cn

[Q51] 用子查询更新
来源：http://kp.newstarts.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://zp.hahajie.cn

[Q52] 删除指定行
来源：http://pl.asd995.cn

DELETE FROM users WHERE id = 10;
来源：http://zb.panjiajie.cn

[Q53] 按条件删除
来源：http://bs.nszjky.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://kl.yuntaijiaju.cn

[Q54] 清空表
来源：http://kl.jianghongdianzi.cn

TRUNCATE TABLE logs;
来源：http://bq.wgjwhj.cn

[Q55] 排名（并列占位）
来源：http://ev.jianghongdianzi.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://tl.shxzukj.cn

[Q56] 密集排名（并列不占位）
来源：http://zt.jianghongdianzi.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://yn.shtwfgs.cn

[Q57] 行号
来源：http://gv.shtwfgs.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://jm.muxihuayi.cn

[Q58] 累计求和
来源：http://vy.hnjuh.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://td.lnxyls.cn

[Q59] 分组内累计
来源：http://qb.wgjwhj.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://sv.yuntaijiaju.cn

[Q60] 取上一行 / 下一行
来源：http://re.jianghongdianzi.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://oq.newstarts.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://lp.nicolike.cn

[Q61] 移动平均
来源：http://ss.bookmarksfly.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wf.szsharing.cn

[Q62] 分组占比
来源：http://ri.gzmigu.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://lg.yuexingan06.cn

[Q63] 开启事务
来源：http://jk.muxihuayi.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://dd.lnxyls.cn

[Q64] 提交事务
来源：http://dc.nszjky.cn

COMMIT;
来源：http://ll.521024.cn

[Q65] 回滚事务
来源：http://pm.colortex.cn

ROLLBACK;
来源：http://zu.muxihuayi.cn

[Q66] 行锁查询
来源：http://ji.hnjuh.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://bm.colortex.cn

[Q67] 设置隔离级别
来源：http://ma.521024.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://pp.hnjuh.cn

[Q68] 保存点
来源：http://af.huixinmuqiang.cn

SAVEPOINT sp1;
来源：http://th.nicolike.cn

ROLLBACK TO sp1;
来源：http://bb.szsharing.cn

[Q69] 查看执行计划
来源：http://ud.yuntaijiaju.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://zg.bookmarksfly.cn

[Q70] 更新统计信息
来源：http://rb.nicolike.cn

ANALYZE TABLE users;
来源：http://ny.yuntaijiaju.cn

[Q71] 查看建表语句
来源：http://he.nszjky.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ad.panjiajie.cn

[Q72] 查看索引
来源：http://ix.huixinmuqiang.cn

SHOW INDEX FROM users;
来源：http://ii.gzmigu.cn

[Q73] 查看表状态
来源：http://et.asd995.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://jx.newstarts.cn

[Q74] 强制使用索引
来源：http://wd.panjiajie.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wq.shxzskj.cn

[Q75] 日期格式化
来源：http://tt.haigaiapp.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ow.asd995.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://cg.muxihuayi.cn

[Q76] 按天统计
来源：http://yr.panjiajie.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://kc.jianghongdianzi.cn

[Q77] 时间加减
来源：http://ni.chemitech.net.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://et.nicolike.cn

[Q78] 当前时间
来源：http://zq.panjiajie.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://pq.lnxyls.cn

[Q79] 字符串拼接
来源：http://py.muxihuayi.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://or.szxytkj.cn

[Q80] 字符串截取
来源：http://ry.bookmarksfly.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://dq.huixiangedu.cn

[Q81] 字符串替换
来源：http://ls.521024.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ig.shxzukj.cn

[Q82] 字符长度与字节长度
来源：http://iy.muxihuayi.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://fs.shtwfgs.cn

[Q83] 大小写转换
来源：http://sd.szxytkj.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://zs.shtwfgs.cn

[Q84] 去除首尾空格
来源：http://je.9csxet.cn

SELECT TRIM(name) FROM users;
来源：http://et.yuexingan06.cn

[Q85] 数值取整
来源：http://rb.wgjwhj.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://sq.huixinmuqiang.cn

[Q86] 读取 JSON 字段
来源：http://ol.9csxet.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://nb.bookmarksfly.cn

[Q87] JSON 字段做条件
来源：http://ug.haigaiapp.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://pr.jctech888.com.cn

[Q88] 行转列（条件聚合）
来源：http://yr.nszjky.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ln.shtwfgs.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://vl.shtwfgs.cn

[Q89] 判断表是否存在
来源：http://an.shxzukj.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://vh.gzmigu.cn

[Q90] 生成序号列
来源：http://ue.9csxet.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://vh.yuntaijiaju.cn

================================================================================
来源：http://qu.lnxyls.cn

R. Bash 专题
来源：http://oc.huanxung.cn

================================================================================
来源：http://fj.wgjwhj.cn

[R01] shebang 与严格模式
来源：http://te.szxytkj.cn

#!/usr/bin/env bash
来源：http://oi.shtwfgs.cn

set -euo pipefail
来源：http://hx.huanxung.cn

[R02] 变量赋值与使用
来源：http://yk.yuexingan06.cn

name="Tom"; echo "$name"
来源：http://gw.jianghongdianzi.cn

[R03] 只读变量
来源：http://zv.shtwfgs.cn

readonly PI=3.14
来源：http://pa.shxzukj.cn

[R04] 位置参数
来源：http://ws.huixiangedu.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://fl.gzmigu.cn

[R05] 参数默认值
来源：http://ja.hnjuh.cn

name="${1:-default}"
来源：http://jk.wgjwhj.cn

[R06] 判断命令是否存在
来源：http://bq.jctech888.com.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://gk.shxzskj.cn

[R07] if 判断文件
来源：http://uy.asd995.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://lc.9csxet.cn

[R08] 数值比较
来源：http://mv.hahajie.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://xz.huanxung.cn

[R09] 字符串比较
来源：http://pd.yuexingan06.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://kl.panjiajie.cn

[R10] 正则匹配
来源：http://md.nicolike.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://gk.asd995.cn

[R11] case 多分支
来源：http://kx.jctech888.com.cn

case "$1" in
来源：http://kv.huanxung.cn

start) echo "启动" ;;
来源：http://ur.wgjwhj.cn

stop)  echo "停止" ;;
来源：http://vw.huixinmuqiang.cn

*)     echo "未知命令" ;;
来源：http://ed.bjjhwx.cn

esac
来源：http://aa.bjjhwx.cn

[R12] for 遍历文件
来源：http://gx.lnxyls.cn

for f in *.txt; do echo "$f"; done
来源：http://oc.hnjuh.cn

[R13] for 计数循环
来源：http://ao.newstarts.cn

for i in {1..10}; do echo "$i"; done
来源：http://cz.bookmarksfly.cn

[R14] C 风格 for
来源：http://bg.shtwfgs.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://tv.colortex.cn

[R15] while 逐行读文件
来源：http://za.jianghongdianzi.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://vl.hnjuh.cn

[R16] until 等待条件
来源：http://ft.hahajie.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://qs.yuntaijiaju.cn

[R17] 数组定义与取值
来源：http://on.9csxet.cn

arr=(a b c); echo "${arr[0]}"
来源：http://wa.szsharing.cn

[R18] 遍历数组
来源：http://ye.nszjky.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://qc.hnjuh.cn

[R19] 数组长度
来源：http://hn.huanxung.cn

echo "${#arr[@]}"
来源：http://rf.lnxyls.cn

[R20] 关联数组（字典）
来源：http://lo.bookmarksfly.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://kh.chemitech.net.cn

[R21] 字符串长度
来源：http://jx.wgjwhj.cn

echo "${#s}"
来源：http://ko.nicolike.cn

[R22] 截取子串
来源：http://cb.nicolike.cn

echo "${s:0:5}"
来源：http://ft.wgjwhj.cn

[R23] 字符串替换
来源：http://hp.huixiangedu.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://gq.nicolike.cn

[R24] 大小写转换
来源：http://tt.hahajie.cn

echo "${s^^}"; echo "${s,,}"
来源：http://jy.bjjhwx.cn

[R25] 去后缀 / 去前缀
来源：http://xu.shxzukj.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://ym.9csxet.cn

[R26] 命令替换
来源：http://rm.521024.cn

now=$(date +%F); echo "$now"
来源：http://ut.shxzukj.cn

[R27] 算术展开
来源：http://hp.huixinmuqiang.cn

echo $((1 + 2 * 3))
来源：http://mb.nicolike.cn

[R28] 浮点运算
来源：http://dw.9csxet.cn

echo "scale=2; 10/3" | bc
来源：http://cd.nszjky.cn

[R29] 定义函数
来源：http://vn.521024.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://rj.huixiangedu.cn

[R30] 函数返回状态码
来源：http://xw.jctech888.com.cn

f() { return 0; }; f || echo "失败了"
来源：http://wk.haigaiapp.cn

[R31] 局部变量
来源：http://ue.chemitech.net.cn

f() { local x=1; echo "$x"; }
来源：http://th.szsharing.cn

[R32] 参数个数校验
来源：http://fr.huixinmuqiang.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://tb.szsharing.cn

[R33] 捕获错误并提示行号
来源：http://ah.9csxet.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://nd.shxzukj.cn

[R34] 退出时清理
来源：http://ei.bookmarksfly.cn

trap 'rm -f "$tmp"' EXIT
来源：http://wt.wgjwhj.cn

[R35] 后台执行并等待
来源：http://wb.lnxyls.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://fp.521024.cn

[R36] 并发执行多个任务
来源：http://qz.nicolike.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ig.bjjhwx.cn

[R37] 把输出赋给变量
来源：http://hh.szsharing.cn

files=$(ls -1)
来源：http://lo.huixinmuqiang.cn

[R38] 管道串联
来源：http://fw.9csxet.cn

cat a.txt | grep -i error | wc -l
来源：http://hg.huixiangedu.cn

[R39] 重定向标准输出与错误
来源：http://nv.jianghongdianzi.cn

cmd > out.log 2>&1
来源：http://gy.muxihuayi.cn

[R40] 追加写日志
来源：http://ta.asd995.cn

echo "log" >> out.log
来源：http://kv.bookmarksfly.cn

[R41] 丢弃输出
来源：http://ff.9csxet.cn

cmd >/dev/null 2>&1
来源：http://rw.szxytkj.cn

[R42] 输入重定向
来源：http://zw.huixinmuqiang.cn

wc -l < a.txt
来源：http://mw.jianghongdianzi.cn

[R43] 按名字查找文件
来源：http://dk.hahajie.cn

find . -name "*.log" -type f
来源：http://oh.shtwfgs.cn

[R44] 按修改时间查找
来源：http://gr.shtwfgs.cn

find . -mtime -7 -type f
来源：http://fu.szxytkj.cn

[R45] 批量删除
来源：http://eg.colortex.cn

find . -name "*.tmp" -delete
来源：http://uo.bookmarksfly.cn

[R46] 递归替换文件内容
来源：http://pd.huixinmuqiang.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hw.shtwfgs.cn

[R47] sed 单行替换
来源：http://qk.lnxyls.cn

sed -i 's/foo/bar/g' a.txt
来源：http://we.jctech888.com.cn

[R48] awk 取指定列
来源：http://in.hahajie.cn

awk '{print $1, $3}' a.txt
来源：http://xu.haigaiapp.cn

[R49] awk 带条件
来源：http://hr.szxytkj.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://oy.haigaiapp.cn

[R50] awk 求和
来源：http://mz.colortex.cn

awk '{s += $2} END {print s}' a.txt
来源：http://nf.szxytkj.cn

[R51] 排序去重取前几
来源：http://mz.szxytkj.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://wd.chemitech.net.cn

[R52] 统计行数
来源：http://am.shtwfgs.cn

wc -l a.txt
来源：http://oe.asd995.cn

[R53] 查看文件头与实时尾
来源：http://oh.asd995.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ez.gzmigu.cn

[R54] 比较两个文件
来源：http://ow.521024.cn

diff a.txt b.txt
来源：http://mn.newstarts.cn

[R55] 压缩与解压
来源：http://wm.muxihuayi.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://yf.newstarts.cn

[R56] 远程拷贝
来源：http://ce.yuntaijiaju.cn

scp file user@host:/path/
来源：http://jf.newstarts.cn

[R57] 远程执行命令
来源：http://if.newstarts.cn

ssh user@host 'uptime'
来源：http://tu.lnxyls.cn

[R58] 下载文件
来源：http://st.shtwfgs.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ak.shxzskj.cn

[R59] 发 POST JSON
来源：http://cd.bjjhwx.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ia.huanxung.cn

[R60] 只看 HTTP 状态码
来源：http://bl.9csxet.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://cp.huixinmuqiang.cn

[R61] 磁盘占用
来源：http://oh.panjiajie.cn

df -h;  du -sh *
来源：http://vt.colortex.cn

[R62] 找最占空间的文件
来源：http://bz.bookmarksfly.cn

du -ah . | sort -rh | head -10
来源：http://fl.wgjwhj.cn

[R63] 内存与进程
来源：http://zn.wgjwhj.cn

free -h;  ps aux | grep nginx
来源：http://ae.yuexingan06.cn

[R64] 结束进程
来源：http://hj.shtwfgs.cn

kill -9 $(pgrep -f app.py)
来源：http://du.lnxyls.cn

[R65] 查看端口占用
来源：http://qb.shtwfgs.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://yy.szxytkj.cn

[R66] 定时任务
来源：http://un.szsharing.cn

crontab -e;  crontab -l
来源：http://lj.nicolike.cn

[R67] 生成随机十六进制串
来源：http://vg.szsharing.cn

openssl rand -hex 16
来源：http://pc.nicolike.cn

[R68] 计算文件校验值
来源：http://vc.yuntaijiaju.cn

sha256sum a.txt;  md5sum a.txt
来源：http://mx.asd995.cn

[R69] 生成随机密码
来源：http://zi.hnjuh.cn

head -c 16 /dev/urandom | base64
来源：http://ph.shxzskj.cn

[R70] 时间戳与互转
来源：http://qa.muxihuayi.cn

date +%s;  date -d @1700000000
来源：http://te.colortex.cn

[R71] 日期格式化
来源：http://xc.521024.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://ya.shxzskj.cn

[R72] 等待端口就绪
来源：http://qw.chemitech.net.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://th.bookmarksfly.cn

[R73] 分割大日志
来源：http://ft.yuntaijiaju.cn

split -l 1000 big.log part_
来源：http://zo.shxzukj.cn

[R74] 批量重命名
来源：http://xn.chemitech.net.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://fm.panjiajie.cn

[R75] 导出环境变量
来源：http://cf.szsharing.cn

export PATH="$HOME/bin:$PATH"
来源：http://xe.muxihuayi.cn

[R76] 使用临时文件
来源：http://jt.9csxet.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://gx.colortex.cn

[R77] 读取用户输入
来源：http://rz.shxzukj.cn

read -rp "请输入: " ans
来源：http://cb.panjiajie.cn

[R78] 交互式菜单
来源：http://ft.haigaiapp.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://ok.hnjuh.cn

[R79] 解析命令行选项
来源：http://wj.hnjuh.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://gr.huixinmuqiang.cn

[R80] 查看脚本执行耗时
来源：http://ab.shxzukj.cn

time ./run.sh
来源：http://ei.haigaiapp.cn

================================================================================
来源：http://zm.yuntaijiaju.cn

S. C / C++ 专题
来源：http://dp.szxytkj.cn

================================================================================
来源：http://ow.yuntaijiaju.cn

[S01] C：Hello World
来源：http://de.jctech888.com.cn

#include <stdio.h>
来源：http://uo.yuexingan06.cn


<!-- 参考信息 -->