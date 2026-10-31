代发 wailian999

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://xp.bookmarksfly.cn

[Q26] 计数
来源：http://zc.jctech888.com.cn

SELECT COUNT(*) FROM users;
来源：http://vu.jctech888.com.cn

[Q27] 条件计数
来源：http://mr.shxzukj.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://qh.521024.cn

[Q28] 求和与平均
来源：http://op.hahajie.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://in.szsharing.cn

[Q29] 最大最小值
来源：http://pn.muxihuayi.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://vo.haigaiapp.cn

[Q30] 分组统计
来源：http://wh.jianghongdianzi.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://nw.shxzskj.cn

[Q31] 分组后过滤
来源：http://tr.521024.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://rc.newstarts.cn

[Q32] 分组拼接字符串
来源：http://wb.bjjhwx.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://xb.hahajie.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://al.newstarts.cn

[Q33] 多列分组
来源：http://za.haigaiapp.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ty.shxzskj.cn

[Q34] 每组取第一条
来源：http://ek.bjjhwx.cn

SELECT * FROM (
来源：http://ja.huixinmuqiang.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wq.bjjhwx.cn

) t WHERE rn = 1;
来源：http://pu.nszjky.cn

[Q35] 内连接
来源：http://ym.huixinmuqiang.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ym.yuexingan06.cn

[Q36] 左连接
来源：http://ox.lnxyls.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://os.nicolike.cn

[Q37] 右连接
来源：http://rl.wgjwhj.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mv.nicolike.cn

[Q38] 全外连接（PostgreSQL）
来源：http://fx.jctech888.com.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://fq.szsharing.cn

[Q39] 自连接（查上下级）
来源：http://ga.shtwfgs.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://ic.huixinmuqiang.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ej.muxihuayi.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://ol.huixiangedu.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://gm.jianghongdianzi.cn

[Q41] 多表连接
来源：http://ti.wgjwhj.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://oy.shxzskj.cn

JOIN users u ON u.id = o.user_id
来源：http://vf.yuntaijiaju.cn

JOIN products p ON p.id = o.product_id;
来源：http://zj.nicolike.cn

[Q42] 连接条件附加过滤
来源：http://ws.szxytkj.cn

SELECT u.name, o.amount FROM users u
来源：http://je.jctech888.com.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ry.nszjky.cn

[Q43] 标量子查询
来源：http://rh.shtwfgs.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://rb.shtwfgs.cn

[Q44] IN 子查询
来源：http://pe.shxzukj.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://nr.bookmarksfly.cn

[Q45] EXISTS 判断存在
来源：http://vp.9csxet.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://pj.huixiangedu.cn

[Q46] NOT EXISTS 判断不存在
来源：http://xo.shxzskj.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ym.chemitech.net.cn

[Q47] 与平均值比较
来源：http://cc.szsharing.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://sh.nicolike.cn

[Q48] CTE 公用表表达式
来源：http://my.gzmigu.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ft.jctech888.com.cn

SELECT * FROM t WHERE c > 5;
来源：http://hd.yuexingan06.cn

[Q49] 更新单行
来源：http://ng.bjjhwx.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://jm.yuexingan06.cn

[Q50] 批量更新
来源：http://sn.asd995.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://cy.haigaiapp.cn

[Q51] 用子查询更新
来源：http://ad.jianghongdianzi.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.chemitech.net.cn

[Q52] 删除指定行
来源：http://ac.yuexingan06.cn

DELETE FROM users WHERE id = 10;
来源：http://rh.asd995.cn

[Q53] 按条件删除
来源：http://mx.shtwfgs.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://av.szxytkj.cn

[Q54] 清空表
来源：http://ro.9csxet.cn

TRUNCATE TABLE logs;
来源：http://jo.asd995.cn

[Q55] 排名（并列占位）
来源：http://um.wgjwhj.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://qi.hnjuh.cn

[Q56] 密集排名（并列不占位）
来源：http://is.yuexingan06.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://jc.shxzukj.cn

[Q57] 行号
来源：http://ji.asd995.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://sd.jctech888.com.cn

[Q58] 累计求和
来源：http://wi.nicolike.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://bm.wgjwhj.cn

[Q59] 分组内累计
来源：http://be.hahajie.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://jg.szxytkj.cn

[Q60] 取上一行 / 下一行
来源：http://cx.lnxyls.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://eq.hahajie.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://dq.bookmarksfly.cn

[Q61] 移动平均
来源：http://xw.yuexingan06.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ar.yuntaijiaju.cn

[Q62] 分组占比
来源：http://sp.nszjky.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://sv.bjjhwx.cn

[Q63] 开启事务
来源：http://da.wgjwhj.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://lp.gzmigu.cn

[Q64] 提交事务
来源：http://st.shxzskj.cn

COMMIT;
来源：http://nf.gzmigu.cn

[Q65] 回滚事务
来源：http://zb.wgjwhj.cn

ROLLBACK;
来源：http://gv.chemitech.net.cn

[Q66] 行锁查询
来源：http://zr.shtwfgs.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ym.nszjky.cn

[Q67] 设置隔离级别
来源：http://bi.521024.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://fe.shxzskj.cn

[Q68] 保存点
来源：http://xq.wgjwhj.cn

SAVEPOINT sp1;
来源：http://gi.hahajie.cn

ROLLBACK TO sp1;
来源：http://ck.nszjky.cn

[Q69] 查看执行计划
来源：http://of.nszjky.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://of.bookmarksfly.cn

[Q70] 更新统计信息
来源：http://fs.yuntaijiaju.cn

ANALYZE TABLE users;
来源：http://kv.nicolike.cn

[Q71] 查看建表语句
来源：http://gw.bjjhwx.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://kn.asd995.cn

[Q72] 查看索引
来源：http://uh.szsharing.cn

SHOW INDEX FROM users;
来源：http://bw.bookmarksfly.cn

[Q73] 查看表状态
来源：http://io.jianghongdianzi.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://ey.yuntaijiaju.cn

[Q74] 强制使用索引
来源：http://rs.shxzukj.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://iz.huixiangedu.cn

[Q75] 日期格式化
来源：http://ha.asd995.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://te.lnxyls.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ux.muxihuayi.cn

[Q76] 按天统计
来源：http://ou.huixiangedu.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://sh.huixiangedu.cn

[Q77] 时间加减
来源：http://fg.gzmigu.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://zq.chemitech.net.cn

[Q78] 当前时间
来源：http://dt.szxytkj.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://yx.huanxung.cn

[Q79] 字符串拼接
来源：http://ty.muxihuayi.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://lp.szxytkj.cn

[Q80] 字符串截取
来源：http://nj.chemitech.net.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mx.shxzukj.cn

[Q81] 字符串替换
来源：http://ef.jianghongdianzi.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://gv.jianghongdianzi.cn

[Q82] 字符长度与字节长度
来源：http://yz.szxytkj.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://it.newstarts.cn

[Q83] 大小写转换
来源：http://xx.szxytkj.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://db.asd995.cn

[Q84] 去除首尾空格
来源：http://cm.bjjhwx.cn

SELECT TRIM(name) FROM users;
来源：http://qu.bookmarksfly.cn

[Q85] 数值取整
来源：http://up.gzmigu.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ou.gzmigu.cn

[Q86] 读取 JSON 字段
来源：http://qf.asd995.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ra.gzmigu.cn

[Q87] JSON 字段做条件
来源：http://yf.szxytkj.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ue.newstarts.cn

[Q88] 行转列（条件聚合）
来源：http://ab.hahajie.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://gp.521024.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://jo.haigaiapp.cn

[Q89] 判断表是否存在
来源：http://bw.yuexingan06.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mi.shtwfgs.cn

[Q90] 生成序号列
来源：http://ye.shxzukj.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://br.shxzskj.cn

================================================================================
来源：http://eq.nicolike.cn

R. Bash 专题
来源：http://tk.nicolike.cn

================================================================================
来源：http://fx.haigaiapp.cn

[R01] shebang 与严格模式
来源：http://ey.muxihuayi.cn

#!/usr/bin/env bash
来源：http://uk.jianghongdianzi.cn

set -euo pipefail
来源：http://ff.hahajie.cn

[R02] 变量赋值与使用
来源：http://pf.nicolike.cn

name="Tom"; echo "$name"
来源：http://lr.jctech888.com.cn

[R03] 只读变量
来源：http://vs.shxzukj.cn

readonly PI=3.14
来源：http://ye.lnxyls.cn

[R04] 位置参数
来源：http://td.huixiangedu.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://he.bjjhwx.cn

[R05] 参数默认值
来源：http://ph.bookmarksfly.cn

name="${1:-default}"
来源：http://el.shtwfgs.cn

[R06] 判断命令是否存在
来源：http://fj.bjjhwx.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://tp.lnxyls.cn

[R07] if 判断文件
来源：http://th.shtwfgs.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://pa.yuexingan06.cn

[R08] 数值比较
来源：http://jj.bookmarksfly.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://km.bookmarksfly.cn

[R09] 字符串比较
来源：http://ct.wgjwhj.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hs.shtwfgs.cn

[R10] 正则匹配
来源：http://xj.hnjuh.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://oq.nszjky.cn

[R11] case 多分支
来源：http://nn.shxzskj.cn

case "$1" in
来源：http://gk.huixiangedu.cn

start) echo "启动" ;;
来源：http://jn.shtwfgs.cn

stop)  echo "停止" ;;
来源：http://dk.gzmigu.cn

*)     echo "未知命令" ;;
来源：http://db.szxytkj.cn

esac
来源：http://so.haigaiapp.cn

[R12] for 遍历文件
来源：http://ct.huixinmuqiang.cn

for f in *.txt; do echo "$f"; done
来源：http://so.lnxyls.cn

[R13] for 计数循环
来源：http://ib.nicolike.cn

for i in {1..10}; do echo "$i"; done
来源：http://gh.nicolike.cn

[R14] C 风格 for
来源：http://bf.huanxung.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ky.shxzskj.cn

[R15] while 逐行读文件
来源：http://su.521024.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://lz.nszjky.cn

[R16] until 等待条件
来源：http://ha.jianghongdianzi.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ep.colortex.cn

[R17] 数组定义与取值
来源：http://vc.jianghongdianzi.cn

arr=(a b c); echo "${arr[0]}"
来源：http://jv.nszjky.cn

[R18] 遍历数组
来源：http://lc.haigaiapp.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://pa.bjjhwx.cn

[R19] 数组长度
来源：http://jk.shxzskj.cn

echo "${#arr[@]}"
来源：http://nb.nicolike.cn

[R20] 关联数组（字典）
来源：http://az.wgjwhj.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mj.wgjwhj.cn

[R21] 字符串长度
来源：http://yz.haigaiapp.cn

echo "${#s}"
来源：http://ow.hnjuh.cn

[R22] 截取子串
来源：http://mi.jianghongdianzi.cn

echo "${s:0:5}"
来源：http://bj.521024.cn

[R23] 字符串替换
来源：http://cz.lnxyls.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://as.shxzskj.cn

[R24] 大小写转换
来源：http://lc.huanxung.cn

echo "${s^^}"; echo "${s,,}"
来源：http://yw.hnjuh.cn

[R25] 去后缀 / 去前缀
来源：http://wp.huixiangedu.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://ka.huixiangedu.cn

[R26] 命令替换
来源：http://bt.hnjuh.cn

now=$(date +%F); echo "$now"
来源：http://qk.hahajie.cn

[R27] 算术展开
来源：http://nc.9csxet.cn

echo $((1 + 2 * 3))
来源：http://yl.gzmigu.cn

[R28] 浮点运算
来源：http://qr.hnjuh.cn

echo "scale=2; 10/3" | bc
来源：http://im.haigaiapp.cn

[R29] 定义函数
来源：http://fm.gzmigu.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mx.nicolike.cn

[R30] 函数返回状态码
来源：http://we.huixiangedu.cn

f() { return 0; }; f || echo "失败了"
来源：http://sl.bookmarksfly.cn

[R31] 局部变量
来源：http://yu.shxzskj.cn

f() { local x=1; echo "$x"; }
来源：http://un.jctech888.com.cn

[R32] 参数个数校验
来源：http://ns.hnjuh.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://je.jianghongdianzi.cn

[R33] 捕获错误并提示行号
来源：http://dk.szsharing.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://rl.shtwfgs.cn

[R34] 退出时清理
来源：http://xy.huixiangedu.cn

trap 'rm -f "$tmp"' EXIT
来源：http://zf.bjjhwx.cn

[R35] 后台执行并等待
来源：http://oz.haigaiapp.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://js.nicolike.cn

[R36] 并发执行多个任务
来源：http://tr.muxihuayi.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://qr.wgjwhj.cn

[R37] 把输出赋给变量
来源：http://ke.yuexingan06.cn

files=$(ls -1)
来源：http://uc.wgjwhj.cn

[R38] 管道串联
来源：http://zo.chemitech.net.cn

cat a.txt | grep -i error | wc -l
来源：http://as.asd995.cn

[R39] 重定向标准输出与错误
来源：http://dy.lnxyls.cn

cmd > out.log 2>&1
来源：http://wi.huixiangedu.cn

[R40] 追加写日志
来源：http://sy.shxzskj.cn

echo "log" >> out.log
来源：http://fv.newstarts.cn

[R41] 丢弃输出
来源：http://jy.lnxyls.cn

cmd >/dev/null 2>&1
来源：http://sl.szxytkj.cn

[R42] 输入重定向
来源：http://ad.shxzukj.cn

wc -l < a.txt
来源：http://qs.hnjuh.cn

[R43] 按名字查找文件
来源：http://jg.lnxyls.cn

find . -name "*.log" -type f
来源：http://mj.panjiajie.cn

[R44] 按修改时间查找
来源：http://jb.hnjuh.cn

find . -mtime -7 -type f
来源：http://we.lnxyls.cn

[R45] 批量删除
来源：http://km.huanxung.cn

find . -name "*.tmp" -delete
来源：http://cf.yuexingan06.cn

[R46] 递归替换文件内容
来源：http://cd.gzmigu.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ns.newstarts.cn

[R47] sed 单行替换
来源：http://jv.huixinmuqiang.cn

sed -i 's/foo/bar/g' a.txt
来源：http://pz.jianghongdianzi.cn

[R48] awk 取指定列
来源：http://nx.haigaiapp.cn

awk '{print $1, $3}' a.txt
来源：http://yf.jctech888.com.cn

[R49] awk 带条件
来源：http://fc.9csxet.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://qz.asd995.cn

[R50] awk 求和
来源：http://ya.yuntaijiaju.cn

awk '{s += $2} END {print s}' a.txt
来源：http://xo.jctech888.com.cn

[R51] 排序去重取前几
来源：http://xb.shtwfgs.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://tz.chemitech.net.cn

[R52] 统计行数
来源：http://vg.szxytkj.cn

wc -l a.txt
来源：http://ur.lnxyls.cn

[R53] 查看文件头与实时尾
来源：http://gp.yuexingan06.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mc.hnjuh.cn

[R54] 比较两个文件
来源：http://ga.shxzskj.cn

diff a.txt b.txt
来源：http://yx.521024.cn

[R55] 压缩与解压
来源：http://dn.huanxung.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ai.szsharing.cn

[R56] 远程拷贝
来源：http://yb.yuexingan06.cn

scp file user@host:/path/
来源：http://eh.nicolike.cn

[R57] 远程执行命令
来源：http://ik.shtwfgs.cn

ssh user@host 'uptime'
来源：http://vs.9csxet.cn

[R58] 下载文件
来源：http://mc.521024.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://fi.hahajie.cn

[R59] 发 POST JSON
来源：http://fi.asd995.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ty.wgjwhj.cn

[R60] 只看 HTTP 状态码
来源：http://rn.panjiajie.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://bk.panjiajie.cn

[R61] 磁盘占用
来源：http://kc.newstarts.cn

df -h;  du -sh *
来源：http://kb.wgjwhj.cn

[R62] 找最占空间的文件
来源：http://xm.panjiajie.cn

du -ah . | sort -rh | head -10
来源：http://zq.nszjky.cn

[R63] 内存与进程
来源：http://xh.newstarts.cn

free -h;  ps aux | grep nginx
来源：http://aa.jianghongdianzi.cn

[R64] 结束进程
来源：http://nf.yuexingan06.cn

kill -9 $(pgrep -f app.py)
来源：http://xj.szsharing.cn

[R65] 查看端口占用
来源：http://uz.huanxung.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mu.wgjwhj.cn

[R66] 定时任务
来源：http://kt.asd995.cn

crontab -e;  crontab -l
来源：http://pf.nszjky.cn

[R67] 生成随机十六进制串
来源：http://ge.yuexingan06.cn

openssl rand -hex 16
来源：http://xo.jctech888.com.cn

[R68] 计算文件校验值
来源：http://dh.haigaiapp.cn

sha256sum a.txt;  md5sum a.txt
来源：http://mw.huanxung.cn

[R69] 生成随机密码
来源：http://tf.huixinmuqiang.cn

head -c 16 /dev/urandom | base64
来源：http://ux.chemitech.net.cn

[R70] 时间戳与互转
来源：http://ga.chemitech.net.cn

date +%s;  date -d @1700000000
来源：http://lt.colortex.cn

[R71] 日期格式化
来源：http://cx.muxihuayi.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://jh.jctech888.com.cn

[R72] 等待端口就绪
来源：http://mf.muxihuayi.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://lo.shxzskj.cn

[R73] 分割大日志
来源：http://we.asd995.cn

split -l 1000 big.log part_
来源：http://sr.shtwfgs.cn

[R74] 批量重命名
来源：http://eh.nicolike.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://qm.shxzskj.cn

[R75] 导出环境变量
来源：http://fm.chemitech.net.cn


<!-- 参考信息 -->