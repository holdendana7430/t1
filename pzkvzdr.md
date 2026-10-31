代发 wailian999

SELECT MAX(age), MIN(age) FROM users;
来源：http://bl.shxzskj.cn

[Q30] 分组统计
来源：http://fi.jianghongdianzi.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://no.bookmarksfly.cn

[Q31] 分组后过滤
来源：http://hv.shtwfgs.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://fm.huixinmuqiang.cn

[Q32] 分组拼接字符串
来源：http://ki.nicolike.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ig.asd995.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://sx.nszjky.cn

[Q33] 多列分组
来源：http://sl.nszjky.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://yv.haigaiapp.cn

[Q34] 每组取第一条
来源：http://tn.yuexingan06.cn

SELECT * FROM (
来源：http://gt.lnxyls.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mf.shxzukj.cn

) t WHERE rn = 1;
来源：http://mv.szsharing.cn

[Q35] 内连接
来源：http://dz.panjiajie.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://bv.jianghongdianzi.cn

[Q36] 左连接
来源：http://ic.muxihuayi.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hl.huixiangedu.cn

[Q37] 右连接
来源：http://tw.shxzukj.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://vz.szxytkj.cn

[Q38] 全外连接（PostgreSQL）
来源：http://rg.huanxung.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://rt.haigaiapp.cn

[Q39] 自连接（查上下级）
来源：http://yc.haigaiapp.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://qi.shxzukj.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ss.colortex.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://lb.huanxung.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://eh.szxytkj.cn

[Q41] 多表连接
来源：http://ab.shxzukj.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://il.bookmarksfly.cn

JOIN users u ON u.id = o.user_id
来源：http://ry.colortex.cn

JOIN products p ON p.id = o.product_id;
来源：http://bb.huanxung.cn

[Q42] 连接条件附加过滤
来源：http://lo.szsharing.cn

SELECT u.name, o.amount FROM users u
来源：http://ir.huixinmuqiang.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://uv.hahajie.cn

[Q43] 标量子查询
来源：http://jo.szxytkj.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://ti.gzmigu.cn

[Q44] IN 子查询
来源：http://jc.wgjwhj.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://az.nicolike.cn

[Q45] EXISTS 判断存在
来源：http://ko.newstarts.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mx.nicolike.cn

[Q46] NOT EXISTS 判断不存在
来源：http://gw.szsharing.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://fv.gzmigu.cn

[Q47] 与平均值比较
来源：http://ce.newstarts.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://fr.yuntaijiaju.cn

[Q48] CTE 公用表表达式
来源：http://ro.chemitech.net.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://us.colortex.cn

SELECT * FROM t WHERE c > 5;
来源：http://bf.521024.cn

[Q49] 更新单行
来源：http://km.nicolike.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://xt.shxzukj.cn

[Q50] 批量更新
来源：http://pw.wgjwhj.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://cs.haigaiapp.cn

[Q51] 用子查询更新
来源：http://az.nicolike.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://cl.jianghongdianzi.cn

[Q52] 删除指定行
来源：http://dn.newstarts.cn

DELETE FROM users WHERE id = 10;
来源：http://wr.9csxet.cn

[Q53] 按条件删除
来源：http://go.panjiajie.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://tl.newstarts.cn

[Q54] 清空表
来源：http://fo.huixiangedu.cn

TRUNCATE TABLE logs;
来源：http://yv.chemitech.net.cn

[Q55] 排名（并列占位）
来源：http://dh.bookmarksfly.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ls.chemitech.net.cn

[Q56] 密集排名（并列不占位）
来源：http://vv.yuntaijiaju.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://yd.huanxung.cn

[Q57] 行号
来源：http://tm.bjjhwx.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://fm.shxzukj.cn

[Q58] 累计求和
来源：http://gw.szxytkj.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://jd.muxihuayi.cn

[Q59] 分组内累计
来源：http://vh.bjjhwx.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://xn.wgjwhj.cn

[Q60] 取上一行 / 下一行
来源：http://lw.muxihuayi.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://fe.panjiajie.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://vx.szxytkj.cn

[Q61] 移动平均
来源：http://ng.jctech888.com.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://pv.colortex.cn

[Q62] 分组占比
来源：http://jo.hahajie.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://vl.wgjwhj.cn

[Q63] 开启事务
来源：http://cb.huixinmuqiang.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://es.521024.cn

[Q64] 提交事务
来源：http://aw.asd995.cn

COMMIT;
来源：http://dq.lnxyls.cn

[Q65] 回滚事务
来源：http://al.colortex.cn

ROLLBACK;
来源：http://vy.huanxung.cn

[Q66] 行锁查询
来源：http://ce.muxihuayi.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://zg.colortex.cn

[Q67] 设置隔离级别
来源：http://rw.shxzukj.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ze.nicolike.cn

[Q68] 保存点
来源：http://nd.yuexingan06.cn

SAVEPOINT sp1;
来源：http://sn.yuexingan06.cn

ROLLBACK TO sp1;
来源：http://ok.jianghongdianzi.cn

[Q69] 查看执行计划
来源：http://tv.nszjky.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ry.bookmarksfly.cn

[Q70] 更新统计信息
来源：http://qb.huixiangedu.cn

ANALYZE TABLE users;
来源：http://ii.jctech888.com.cn

[Q71] 查看建表语句
来源：http://re.9csxet.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ra.hnjuh.cn

[Q72] 查看索引
来源：http://ee.wgjwhj.cn

SHOW INDEX FROM users;
来源：http://go.jctech888.com.cn

[Q73] 查看表状态
来源：http://lo.panjiajie.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://un.wgjwhj.cn

[Q74] 强制使用索引
来源：http://lx.shxzukj.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://og.muxihuayi.cn

[Q75] 日期格式化
来源：http://dm.bookmarksfly.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ok.hahajie.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ny.lnxyls.cn

[Q76] 按天统计
来源：http://xv.bookmarksfly.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://co.huanxung.cn

[Q77] 时间加减
来源：http://th.muxihuayi.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wd.chemitech.net.cn

[Q78] 当前时间
来源：http://ob.huixinmuqiang.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://br.colortex.cn

[Q79] 字符串拼接
来源：http://eg.haigaiapp.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hh.jctech888.com.cn

[Q80] 字符串截取
来源：http://le.shtwfgs.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://qo.gzmigu.cn

[Q81] 字符串替换
来源：http://jf.hahajie.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://uw.szxytkj.cn

[Q82] 字符长度与字节长度
来源：http://st.gzmigu.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://vx.huanxung.cn

[Q83] 大小写转换
来源：http://au.nszjky.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://qr.huixiangedu.cn

[Q84] 去除首尾空格
来源：http://mu.wgjwhj.cn

SELECT TRIM(name) FROM users;
来源：http://zh.asd995.cn

[Q85] 数值取整
来源：http://xe.huixinmuqiang.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ty.huixiangedu.cn

[Q86] 读取 JSON 字段
来源：http://fu.haigaiapp.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://bz.9csxet.cn

[Q87] JSON 字段做条件
来源：http://hg.huanxung.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://rj.nicolike.cn

[Q88] 行转列（条件聚合）
来源：http://tm.huixiangedu.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://tz.nicolike.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://yq.shxzukj.cn

[Q89] 判断表是否存在
来源：http://qa.hahajie.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://le.gzmigu.cn

[Q90] 生成序号列
来源：http://dy.521024.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://gt.haigaiapp.cn

================================================================================
来源：http://vz.521024.cn

R. Bash 专题
来源：http://ns.jianghongdianzi.cn

================================================================================
来源：http://si.chemitech.net.cn

[R01] shebang 与严格模式
来源：http://ti.colortex.cn

#!/usr/bin/env bash
来源：http://mx.szsharing.cn

set -euo pipefail
来源：http://hc.huixiangedu.cn

[R02] 变量赋值与使用
来源：http://kc.colortex.cn

name="Tom"; echo "$name"
来源：http://ot.hahajie.cn

[R03] 只读变量
来源：http://xt.bjjhwx.cn

readonly PI=3.14
来源：http://it.huixinmuqiang.cn

[R04] 位置参数
来源：http://bc.chemitech.net.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://tb.newstarts.cn

[R05] 参数默认值
来源：http://bg.yuntaijiaju.cn

name="${1:-default}"
来源：http://kl.shxzukj.cn

[R06] 判断命令是否存在
来源：http://ib.jctech888.com.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://an.shxzskj.cn

[R07] if 判断文件
来源：http://sw.asd995.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://rf.shtwfgs.cn

[R08] 数值比较
来源：http://mt.nszjky.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://ws.szxytkj.cn

[R09] 字符串比较
来源：http://zx.newstarts.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://yg.bjjhwx.cn

[R10] 正则匹配
来源：http://yd.521024.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://lm.asd995.cn

[R11] case 多分支
来源：http://fi.yuexingan06.cn

case "$1" in
来源：http://bv.lnxyls.cn

start) echo "启动" ;;
来源：http://ak.colortex.cn

stop)  echo "停止" ;;
来源：http://ou.521024.cn

*)     echo "未知命令" ;;
来源：http://ca.wgjwhj.cn

esac
来源：http://no.yuntaijiaju.cn

[R12] for 遍历文件
来源：http://ny.asd995.cn

for f in *.txt; do echo "$f"; done
来源：http://cl.gzmigu.cn

[R13] for 计数循环
来源：http://xw.521024.cn

for i in {1..10}; do echo "$i"; done
来源：http://ia.gzmigu.cn

[R14] C 风格 for
来源：http://dz.shxzskj.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ew.yuntaijiaju.cn

[R15] while 逐行读文件
来源：http://hj.521024.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ti.bjjhwx.cn

[R16] until 等待条件
来源：http://fq.hahajie.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://gk.haigaiapp.cn

[R17] 数组定义与取值
来源：http://fo.haigaiapp.cn

arr=(a b c); echo "${arr[0]}"
来源：http://oo.newstarts.cn

[R18] 遍历数组
来源：http://tn.szsharing.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://yt.shtwfgs.cn

[R19] 数组长度
来源：http://qu.colortex.cn

echo "${#arr[@]}"
来源：http://sg.gzmigu.cn

[R20] 关联数组（字典）
来源：http://vx.yuexingan06.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://cl.wgjwhj.cn

[R21] 字符串长度
来源：http://sm.shtwfgs.cn

echo "${#s}"
来源：http://vz.huanxung.cn

[R22] 截取子串
来源：http://nj.shxzukj.cn

echo "${s:0:5}"
来源：http://lf.haigaiapp.cn

[R23] 字符串替换
来源：http://fn.shxzukj.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://pv.szsharing.cn

[R24] 大小写转换
来源：http://kx.jctech888.com.cn

echo "${s^^}"; echo "${s,,}"
来源：http://bp.nszjky.cn

[R25] 去后缀 / 去前缀
来源：http://hz.huanxung.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://mv.wgjwhj.cn

[R26] 命令替换
来源：http://ip.9csxet.cn

now=$(date +%F); echo "$now"
来源：http://nu.huixinmuqiang.cn

[R27] 算术展开
来源：http://sx.jctech888.com.cn

echo $((1 + 2 * 3))
来源：http://jn.colortex.cn

[R28] 浮点运算
来源：http://cf.yuexingan06.cn

echo "scale=2; 10/3" | bc
来源：http://fc.gzmigu.cn

[R29] 定义函数
来源：http://yb.newstarts.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://pg.panjiajie.cn

[R30] 函数返回状态码
来源：http://wb.huanxung.cn

f() { return 0; }; f || echo "失败了"
来源：http://fb.wgjwhj.cn

[R31] 局部变量
来源：http://sz.panjiajie.cn

f() { local x=1; echo "$x"; }
来源：http://nf.shtwfgs.cn

[R32] 参数个数校验
来源：http://ti.wgjwhj.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://pz.haigaiapp.cn

[R33] 捕获错误并提示行号
来源：http://pu.yuntaijiaju.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ee.bjjhwx.cn

[R34] 退出时清理
来源：http://rh.huixiangedu.cn

trap 'rm -f "$tmp"' EXIT
来源：http://xu.hnjuh.cn

[R35] 后台执行并等待
来源：http://di.shxzskj.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://ms.szsharing.cn

[R36] 并发执行多个任务
来源：http://ie.yuntaijiaju.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://qz.shxzukj.cn

[R37] 把输出赋给变量
来源：http://si.szxytkj.cn

files=$(ls -1)
来源：http://ta.hnjuh.cn

[R38] 管道串联
来源：http://fm.huixinmuqiang.cn

cat a.txt | grep -i error | wc -l
来源：http://le.hnjuh.cn

[R39] 重定向标准输出与错误
来源：http://wj.nicolike.cn

cmd > out.log 2>&1
来源：http://bj.szsharing.cn

[R40] 追加写日志
来源：http://nz.bookmarksfly.cn

echo "log" >> out.log
来源：http://og.muxihuayi.cn

[R41] 丢弃输出
来源：http://ws.yuexingan06.cn

cmd >/dev/null 2>&1
来源：http://jf.nszjky.cn

[R42] 输入重定向
来源：http://md.asd995.cn

wc -l < a.txt
来源：http://bv.bjjhwx.cn

[R43] 按名字查找文件
来源：http://uo.huixinmuqiang.cn

find . -name "*.log" -type f
来源：http://tl.wgjwhj.cn

[R44] 按修改时间查找
来源：http://jc.colortex.cn

find . -mtime -7 -type f
来源：http://zn.hnjuh.cn

[R45] 批量删除
来源：http://in.nszjky.cn

find . -name "*.tmp" -delete
来源：http://ze.hnjuh.cn

[R46] 递归替换文件内容
来源：http://js.szsharing.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://af.jctech888.com.cn

[R47] sed 单行替换
来源：http://zo.bookmarksfly.cn

sed -i 's/foo/bar/g' a.txt
来源：http://kw.hahajie.cn

[R48] awk 取指定列
来源：http://ud.bjjhwx.cn

awk '{print $1, $3}' a.txt
来源：http://ia.shxzukj.cn

[R49] awk 带条件
来源：http://op.newstarts.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://bi.shxzskj.cn

[R50] awk 求和
来源：http://zn.gzmigu.cn

awk '{s += $2} END {print s}' a.txt
来源：http://rn.9csxet.cn

[R51] 排序去重取前几
来源：http://nu.szxytkj.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://ey.9csxet.cn

[R52] 统计行数
来源：http://jq.panjiajie.cn

wc -l a.txt
来源：http://yl.muxihuayi.cn

[R53] 查看文件头与实时尾
来源：http://gd.nicolike.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ca.huixiangedu.cn

[R54] 比较两个文件
来源：http://qv.wgjwhj.cn

diff a.txt b.txt
来源：http://fm.9csxet.cn

[R55] 压缩与解压
来源：http://it.bookmarksfly.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wq.yuexingan06.cn

[R56] 远程拷贝
来源：http://ic.panjiajie.cn

scp file user@host:/path/
来源：http://on.521024.cn

[R57] 远程执行命令
来源：http://pa.shxzskj.cn

ssh user@host 'uptime'
来源：http://qj.huixinmuqiang.cn

[R58] 下载文件
来源：http://rx.szsharing.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ik.521024.cn

[R59] 发 POST JSON
来源：http://qa.lnxyls.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://dc.panjiajie.cn

[R60] 只看 HTTP 状态码
来源：http://qj.asd995.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ht.jianghongdianzi.cn

[R61] 磁盘占用
来源：http://lv.huanxung.cn

df -h;  du -sh *
来源：http://vk.hnjuh.cn

[R62] 找最占空间的文件
来源：http://gk.szxytkj.cn

du -ah . | sort -rh | head -10
来源：http://nd.shxzskj.cn

[R63] 内存与进程
来源：http://yi.colortex.cn

free -h;  ps aux | grep nginx
来源：http://uq.bookmarksfly.cn

[R64] 结束进程
来源：http://ui.chemitech.net.cn

kill -9 $(pgrep -f app.py)
来源：http://if.szsharing.cn

[R65] 查看端口占用
来源：http://kl.9csxet.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://no.521024.cn

[R66] 定时任务
来源：http://yp.huanxung.cn

crontab -e;  crontab -l
来源：http://ex.szxytkj.cn

[R67] 生成随机十六进制串
来源：http://is.shxzukj.cn

openssl rand -hex 16
来源：http://lx.hnjuh.cn

[R68] 计算文件校验值
来源：http://id.shtwfgs.cn

sha256sum a.txt;  md5sum a.txt
来源：http://pt.chemitech.net.cn

[R69] 生成随机密码
来源：http://fw.shxzskj.cn

head -c 16 /dev/urandom | base64
来源：http://rw.shxzukj.cn

[R70] 时间戳与互转
来源：http://jh.chemitech.net.cn

date +%s;  date -d @1700000000
来源：http://cc.bookmarksfly.cn

[R71] 日期格式化
来源：http://iu.panjiajie.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://em.gzmigu.cn

[R72] 等待端口就绪
来源：http://gt.huixiangedu.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://ub.szsharing.cn

[R73] 分割大日志
来源：http://kq.nszjky.cn

split -l 1000 big.log part_
来源：http://cq.yuntaijiaju.cn

[R74] 批量重命名
来源：http://wm.shxzskj.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://lg.panjiajie.cn

[R75] 导出环境变量
来源：http://mr.9csxet.cn

export PATH="$HOME/bin:$PATH"
来源：http://ch.huanxung.cn

[R76] 使用临时文件
来源：http://hz.shxzskj.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://fw.huixinmuqiang.cn

[R77] 读取用户输入
来源：http://em.lnxyls.cn

read -rp "请输入: " ans
来源：http://kk.nszjky.cn

[R78] 交互式菜单
来源：http://gi.nszjky.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://gk.shxzukj.cn

[R79] 解析命令行选项
来源：http://uk.yuntaijiaju.cn


<!-- 参考信息 -->