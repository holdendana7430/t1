代发 wailian999

SELECT MAX(age), MIN(age) FROM users;
来源：http://nl.hahajie.cn

[Q30] 分组统计
来源：http://hf.chemitech.net.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://xi.wgjwhj.cn

[Q31] 分组后过滤
来源：http://op.nszjky.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://nd.jianghongdianzi.cn

[Q32] 分组拼接字符串
来源：http://tm.yuntaijiaju.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://pd.yuntaijiaju.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ad.nicolike.cn

[Q33] 多列分组
来源：http://ix.szsharing.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ce.shxzukj.cn

[Q34] 每组取第一条
来源：http://qt.chemitech.net.cn

SELECT * FROM (
来源：http://fi.huixinmuqiang.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ot.shxzukj.cn

) t WHERE rn = 1;
来源：http://nb.bookmarksfly.cn

[Q35] 内连接
来源：http://aw.shxzskj.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://oy.muxihuayi.cn

[Q36] 左连接
来源：http://ls.bjjhwx.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://jc.wgjwhj.cn

[Q37] 右连接
来源：http://ql.bookmarksfly.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://go.huanxung.cn

[Q38] 全外连接（PostgreSQL）
来源：http://vj.huixinmuqiang.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://fe.yuexingan06.cn

[Q39] 自连接（查上下级）
来源：http://hh.hnjuh.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://zn.asd995.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://bd.shxzskj.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://sb.yuexingan06.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ty.shxzskj.cn

[Q41] 多表连接
来源：http://op.shxzskj.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://km.jctech888.com.cn

JOIN users u ON u.id = o.user_id
来源：http://tz.wgjwhj.cn

JOIN products p ON p.id = o.product_id;
来源：http://bu.szsharing.cn

[Q42] 连接条件附加过滤
来源：http://ce.nszjky.cn

SELECT u.name, o.amount FROM users u
来源：http://am.colortex.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://vr.9csxet.cn

[Q43] 标量子查询
来源：http://tv.bjjhwx.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://ib.shxzskj.cn

[Q44] IN 子查询
来源：http://cu.huanxung.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://oy.newstarts.cn

[Q45] EXISTS 判断存在
来源：http://hq.muxihuayi.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ts.newstarts.cn

[Q46] NOT EXISTS 判断不存在
来源：http://du.521024.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ui.shxzukj.cn

[Q47] 与平均值比较
来源：http://ij.asd995.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ex.jctech888.com.cn

[Q48] CTE 公用表表达式
来源：http://qw.muxihuayi.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://qg.huanxung.cn

SELECT * FROM t WHERE c > 5;
来源：http://rb.gzmigu.cn

[Q49] 更新单行
来源：http://lf.nicolike.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ji.panjiajie.cn

[Q50] 批量更新
来源：http://ug.hahajie.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://km.lnxyls.cn

[Q51] 用子查询更新
来源：http://tj.yuexingan06.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://fs.521024.cn

[Q52] 删除指定行
来源：http://ic.yuntaijiaju.cn

DELETE FROM users WHERE id = 10;
来源：http://fj.jctech888.com.cn

[Q53] 按条件删除
来源：http://ka.bookmarksfly.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://of.huixiangedu.cn

[Q54] 清空表
来源：http://lk.521024.cn

TRUNCATE TABLE logs;
来源：http://tm.muxihuayi.cn

[Q55] 排名（并列占位）
来源：http://qv.huixinmuqiang.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hc.huixiangedu.cn

[Q56] 密集排名（并列不占位）
来源：http://ik.jianghongdianzi.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://yw.szxytkj.cn

[Q57] 行号
来源：http://ir.hahajie.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://dh.hahajie.cn

[Q58] 累计求和
来源：http://gf.huanxung.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mc.szxytkj.cn

[Q59] 分组内累计
来源：http://fg.panjiajie.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://nd.huanxung.cn

[Q60] 取上一行 / 下一行
来源：http://yu.jianghongdianzi.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://zz.szsharing.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mi.bjjhwx.cn

[Q61] 移动平均
来源：http://lk.bjjhwx.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://uz.jianghongdianzi.cn

[Q62] 分组占比
来源：http://cq.nicolike.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://qp.shtwfgs.cn

[Q63] 开启事务
来源：http://xz.bookmarksfly.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://ys.jctech888.com.cn

[Q64] 提交事务
来源：http://qp.huixinmuqiang.cn

COMMIT;
来源：http://rz.szsharing.cn

[Q65] 回滚事务
来源：http://ad.huixinmuqiang.cn

ROLLBACK;
来源：http://uw.wgjwhj.cn

[Q66] 行锁查询
来源：http://ta.gzmigu.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://sk.nszjky.cn

[Q67] 设置隔离级别
来源：http://zy.nicolike.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://vz.yuexingan06.cn

[Q68] 保存点
来源：http://wo.wgjwhj.cn

SAVEPOINT sp1;
来源：http://cu.shtwfgs.cn

ROLLBACK TO sp1;
来源：http://ku.muxihuayi.cn

[Q69] 查看执行计划
来源：http://sy.huixiangedu.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://bb.shtwfgs.cn

[Q70] 更新统计信息
来源：http://zd.shtwfgs.cn

ANALYZE TABLE users;
来源：http://yi.szxytkj.cn

[Q71] 查看建表语句
来源：http://mf.szsharing.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://cm.colortex.cn

[Q72] 查看索引
来源：http://ss.newstarts.cn

SHOW INDEX FROM users;
来源：http://uh.huixinmuqiang.cn

[Q73] 查看表状态
来源：http://js.huanxung.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://bz.newstarts.cn

[Q74] 强制使用索引
来源：http://lh.bookmarksfly.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://dj.huixinmuqiang.cn

[Q75] 日期格式化
来源：http://py.szsharing.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mf.newstarts.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://nd.panjiajie.cn

[Q76] 按天统计
来源：http://cy.9csxet.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://zr.yuntaijiaju.cn

[Q77] 时间加减
来源：http://ox.chemitech.net.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ul.jctech888.com.cn

[Q78] 当前时间
来源：http://ax.shxzukj.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://oe.colortex.cn

[Q79] 字符串拼接
来源：http://qj.yuexingan06.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://or.hnjuh.cn

[Q80] 字符串截取
来源：http://lx.asd995.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://sx.hahajie.cn

[Q81] 字符串替换
来源：http://ti.szxytkj.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://yl.shtwfgs.cn

[Q82] 字符长度与字节长度
来源：http://fa.panjiajie.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://cu.hahajie.cn

[Q83] 大小写转换
来源：http://rg.shtwfgs.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://xz.lnxyls.cn

[Q84] 去除首尾空格
来源：http://gq.haigaiapp.cn

SELECT TRIM(name) FROM users;
来源：http://xy.shtwfgs.cn

[Q85] 数值取整
来源：http://pk.shtwfgs.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://qt.huixiangedu.cn

[Q86] 读取 JSON 字段
来源：http://bd.521024.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://gk.yuexingan06.cn

[Q87] JSON 字段做条件
来源：http://bf.jctech888.com.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://oy.yuntaijiaju.cn

[Q88] 行转列（条件聚合）
来源：http://lr.9csxet.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://fn.nszjky.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://dr.colortex.cn

[Q89] 判断表是否存在
来源：http://kh.chemitech.net.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://dz.shtwfgs.cn

[Q90] 生成序号列
来源：http://bl.huixinmuqiang.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ux.nicolike.cn

================================================================================
来源：http://jc.jianghongdianzi.cn

R. Bash 专题
来源：http://so.hnjuh.cn

================================================================================
来源：http://mt.nszjky.cn

[R01] shebang 与严格模式
来源：http://se.haigaiapp.cn

#!/usr/bin/env bash
来源：http://mw.newstarts.cn

set -euo pipefail
来源：http://bo.panjiajie.cn

[R02] 变量赋值与使用
来源：http://jq.shtwfgs.cn

name="Tom"; echo "$name"
来源：http://kn.hnjuh.cn

[R03] 只读变量
来源：http://ij.newstarts.cn

readonly PI=3.14
来源：http://zz.bookmarksfly.cn

[R04] 位置参数
来源：http://ma.huixiangedu.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://fz.gzmigu.cn

[R05] 参数默认值
来源：http://uw.newstarts.cn

name="${1:-default}"
来源：http://zx.colortex.cn

[R06] 判断命令是否存在
来源：http://za.521024.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://zl.muxihuayi.cn

[R07] if 判断文件
来源：http://xi.nszjky.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://uv.shtwfgs.cn

[R08] 数值比较
来源：http://zh.bjjhwx.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://cu.yuntaijiaju.cn

[R09] 字符串比较
来源：http://yp.haigaiapp.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ho.bookmarksfly.cn

[R10] 正则匹配
来源：http://hq.huanxung.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://cp.chemitech.net.cn

[R11] case 多分支
来源：http://bg.szsharing.cn

case "$1" in
来源：http://jm.bookmarksfly.cn

start) echo "启动" ;;
来源：http://rz.lnxyls.cn

stop)  echo "停止" ;;
来源：http://td.szxytkj.cn

*)     echo "未知命令" ;;
来源：http://pk.hahajie.cn

esac
来源：http://ri.hahajie.cn

[R12] for 遍历文件
来源：http://es.lnxyls.cn

for f in *.txt; do echo "$f"; done
来源：http://qf.shtwfgs.cn

[R13] for 计数循环
来源：http://rq.bjjhwx.cn

for i in {1..10}; do echo "$i"; done
来源：http://dr.chemitech.net.cn

[R14] C 风格 for
来源：http://lw.asd995.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://go.9csxet.cn

[R15] while 逐行读文件
来源：http://mc.yuntaijiaju.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ed.chemitech.net.cn

[R16] until 等待条件
来源：http://su.huixiangedu.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://eh.hahajie.cn

[R17] 数组定义与取值
来源：http://aq.chemitech.net.cn

arr=(a b c); echo "${arr[0]}"
来源：http://ab.wgjwhj.cn

[R18] 遍历数组
来源：http://fn.huixinmuqiang.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://pc.asd995.cn

[R19] 数组长度
来源：http://uw.bookmarksfly.cn

echo "${#arr[@]}"
来源：http://jb.yuntaijiaju.cn

[R20] 关联数组（字典）
来源：http://gr.jctech888.com.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://je.szsharing.cn

[R21] 字符串长度
来源：http://rv.chemitech.net.cn

echo "${#s}"
来源：http://jl.bjjhwx.cn

[R22] 截取子串
来源：http://wj.9csxet.cn

echo "${s:0:5}"
来源：http://da.muxihuayi.cn

[R23] 字符串替换
来源：http://qc.yuexingan06.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://st.panjiajie.cn

[R24] 大小写转换
来源：http://qr.9csxet.cn

echo "${s^^}"; echo "${s,,}"
来源：http://gt.haigaiapp.cn

[R25] 去后缀 / 去前缀
来源：http://za.szxytkj.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://eg.nszjky.cn

[R26] 命令替换
来源：http://fl.jianghongdianzi.cn

now=$(date +%F); echo "$now"
来源：http://px.bjjhwx.cn

[R27] 算术展开
来源：http://sb.yuntaijiaju.cn

echo $((1 + 2 * 3))
来源：http://vl.nicolike.cn

[R28] 浮点运算
来源：http://te.szxytkj.cn

echo "scale=2; 10/3" | bc
来源：http://sx.gzmigu.cn

[R29] 定义函数
来源：http://br.newstarts.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ao.lnxyls.cn

[R30] 函数返回状态码
来源：http://nf.haigaiapp.cn

f() { return 0; }; f || echo "失败了"
来源：http://vg.nicolike.cn

[R31] 局部变量
来源：http://xu.bjjhwx.cn

f() { local x=1; echo "$x"; }
来源：http://vm.muxihuayi.cn

[R32] 参数个数校验
来源：http://qf.asd995.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://kr.panjiajie.cn

[R33] 捕获错误并提示行号
来源：http://qz.lnxyls.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ep.szsharing.cn

[R34] 退出时清理
来源：http://so.szsharing.cn

trap 'rm -f "$tmp"' EXIT
来源：http://jk.colortex.cn

[R35] 后台执行并等待
来源：http://dm.szxytkj.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://ko.newstarts.cn

[R36] 并发执行多个任务
来源：http://pm.lnxyls.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://vo.gzmigu.cn

[R37] 把输出赋给变量
来源：http://nh.muxihuayi.cn

files=$(ls -1)
来源：http://xd.szxytkj.cn

[R38] 管道串联
来源：http://kr.muxihuayi.cn

cat a.txt | grep -i error | wc -l
来源：http://yy.szsharing.cn

[R39] 重定向标准输出与错误
来源：http://be.yuexingan06.cn

cmd > out.log 2>&1
来源：http://id.huanxung.cn

[R40] 追加写日志
来源：http://zs.hahajie.cn

echo "log" >> out.log
来源：http://tf.shxzskj.cn

[R41] 丢弃输出
来源：http://te.bookmarksfly.cn

cmd >/dev/null 2>&1
来源：http://ih.jianghongdianzi.cn

[R42] 输入重定向
来源：http://pj.jianghongdianzi.cn

wc -l < a.txt
来源：http://gh.gzmigu.cn

[R43] 按名字查找文件
来源：http://dd.shtwfgs.cn

find . -name "*.log" -type f
来源：http://nx.gzmigu.cn

[R44] 按修改时间查找
来源：http://gn.hnjuh.cn

find . -mtime -7 -type f
来源：http://xn.bjjhwx.cn

[R45] 批量删除
来源：http://lp.bjjhwx.cn

find . -name "*.tmp" -delete
来源：http://nl.colortex.cn

[R46] 递归替换文件内容
来源：http://ys.szsharing.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hf.colortex.cn

[R47] sed 单行替换
来源：http://je.yuexingan06.cn

sed -i 's/foo/bar/g' a.txt
来源：http://zy.jianghongdianzi.cn

[R48] awk 取指定列
来源：http://in.hnjuh.cn

awk '{print $1, $3}' a.txt
来源：http://ao.lnxyls.cn

[R49] awk 带条件
来源：http://ho.9csxet.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://bu.shtwfgs.cn

[R50] awk 求和
来源：http://mk.muxihuayi.cn

awk '{s += $2} END {print s}' a.txt
来源：http://ny.jianghongdianzi.cn

[R51] 排序去重取前几
来源：http://lm.bjjhwx.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://ra.huanxung.cn

[R52] 统计行数
来源：http://tc.nszjky.cn

wc -l a.txt
来源：http://xw.haigaiapp.cn

[R53] 查看文件头与实时尾
来源：http://sc.wgjwhj.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://dx.hnjuh.cn

[R54] 比较两个文件
来源：http://pe.521024.cn

diff a.txt b.txt
来源：http://pq.shxzskj.cn

[R55] 压缩与解压
来源：http://lv.shxzukj.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ux.yuexingan06.cn

[R56] 远程拷贝
来源：http://zq.shxzukj.cn

scp file user@host:/path/
来源：http://bc.nicolike.cn

[R57] 远程执行命令
来源：http://nw.szsharing.cn

ssh user@host 'uptime'
来源：http://cd.gzmigu.cn

[R58] 下载文件
来源：http://zj.szxytkj.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ab.521024.cn

[R59] 发 POST JSON
来源：http://jf.hnjuh.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://tr.9csxet.cn

[R60] 只看 HTTP 状态码
来源：http://ad.chemitech.net.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://dw.asd995.cn

[R61] 磁盘占用
来源：http://qn.9csxet.cn

df -h;  du -sh *
来源：http://sq.bjjhwx.cn

[R62] 找最占空间的文件
来源：http://ys.hahajie.cn

du -ah . | sort -rh | head -10
来源：http://jq.chemitech.net.cn

[R63] 内存与进程
来源：http://wn.shxzukj.cn

free -h;  ps aux | grep nginx
来源：http://ih.yuexingan06.cn

[R64] 结束进程
来源：http://hb.gzmigu.cn

kill -9 $(pgrep -f app.py)
来源：http://kr.9csxet.cn

[R65] 查看端口占用
来源：http://yy.yuntaijiaju.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://rc.muxihuayi.cn

[R66] 定时任务
来源：http://hq.haigaiapp.cn

crontab -e;  crontab -l
来源：http://cu.huixiangedu.cn

[R67] 生成随机十六进制串
来源：http://tq.muxihuayi.cn

openssl rand -hex 16
来源：http://uu.muxihuayi.cn

[R68] 计算文件校验值
来源：http://hy.hahajie.cn

sha256sum a.txt;  md5sum a.txt
来源：http://wo.huixinmuqiang.cn

[R69] 生成随机密码
来源：http://ym.huixinmuqiang.cn

head -c 16 /dev/urandom | base64
来源：http://ed.jianghongdianzi.cn

[R70] 时间戳与互转
来源：http://yi.szxytkj.cn

date +%s;  date -d @1700000000
来源：http://ip.szsharing.cn

[R71] 日期格式化
来源：http://mj.yuexingan06.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://ei.haigaiapp.cn

[R72] 等待端口就绪
来源：http://ri.9csxet.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://tl.haigaiapp.cn

[R73] 分割大日志
来源：http://xk.huixiangedu.cn

split -l 1000 big.log part_
来源：http://rs.haigaiapp.cn

[R74] 批量重命名
来源：http://ng.bookmarksfly.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://gs.jctech888.com.cn

[R75] 导出环境变量
来源：http://xx.jianghongdianzi.cn

export PATH="$HOME/bin:$PATH"
来源：http://kv.gzmigu.cn

[R76] 使用临时文件
来源：http://iq.szsharing.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mf.newstarts.cn

[R77] 读取用户输入
来源：http://rh.panjiajie.cn

read -rp "请输入: " ans
来源：http://zq.bjjhwx.cn

[R78] 交互式菜单
来源：http://xr.nicolike.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://ux.bookmarksfly.cn

[R79] 解析命令行选项
来源：http://tq.hnjuh.cn


<!-- 参考信息 -->