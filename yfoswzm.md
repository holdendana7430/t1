代发 wailian999

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ls.panjiajie.cn

[Q28] 求和与平均
来源：http://as.hahajie.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://xt.yuexingan06.cn

[Q29] 最大最小值
来源：http://zp.9csxet.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://dr.yuntaijiaju.cn

[Q30] 分组统计
来源：http://pl.gzmigu.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ul.huanxung.cn

[Q31] 分组后过滤
来源：http://fg.muxihuayi.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://vb.szxytkj.cn

[Q32] 分组拼接字符串
来源：http://vc.gzmigu.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://op.muxihuayi.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://xv.chemitech.net.cn

[Q33] 多列分组
来源：http://yd.gzmigu.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://xp.asd995.cn

[Q34] 每组取第一条
来源：http://zq.szsharing.cn

SELECT * FROM (
来源：http://br.gzmigu.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://tu.shxzukj.cn

) t WHERE rn = 1;
来源：http://yi.bookmarksfly.cn

[Q35] 内连接
来源：http://ci.asd995.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://rv.chemitech.net.cn

[Q36] 左连接
来源：http://mo.521024.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://qo.nszjky.cn

[Q37] 右连接
来源：http://ih.huanxung.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://kb.9csxet.cn

[Q38] 全外连接（PostgreSQL）
来源：http://fn.lnxyls.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ac.wgjwhj.cn

[Q39] 自连接（查上下级）
来源：http://ld.9csxet.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://ef.wgjwhj.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ey.yuntaijiaju.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://jc.9csxet.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://si.lnxyls.cn

[Q41] 多表连接
来源：http://ua.panjiajie.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://zr.bjjhwx.cn

JOIN users u ON u.id = o.user_id
来源：http://jm.huanxung.cn

JOIN products p ON p.id = o.product_id;
来源：http://xy.gzmigu.cn

[Q42] 连接条件附加过滤
来源：http://fa.shxzukj.cn

SELECT u.name, o.amount FROM users u
来源：http://ai.szsharing.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wj.muxihuayi.cn

[Q43] 标量子查询
来源：http://if.wgjwhj.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://nb.bookmarksfly.cn

[Q44] IN 子查询
来源：http://ii.huixiangedu.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://pp.yuntaijiaju.cn

[Q45] EXISTS 判断存在
来源：http://vq.colortex.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://jc.huixiangedu.cn

[Q46] NOT EXISTS 判断不存在
来源：http://vy.gzmigu.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mz.9csxet.cn

[Q47] 与平均值比较
来源：http://cu.nszjky.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://jv.colortex.cn

[Q48] CTE 公用表表达式
来源：http://tv.lnxyls.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://cu.szxytkj.cn

SELECT * FROM t WHERE c > 5;
来源：http://xt.hahajie.cn

[Q49] 更新单行
来源：http://ya.yuexingan06.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hb.nszjky.cn

[Q50] 批量更新
来源：http://su.huanxung.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://fy.521024.cn

[Q51] 用子查询更新
来源：http://ua.521024.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://fs.wgjwhj.cn

[Q52] 删除指定行
来源：http://ql.shtwfgs.cn

DELETE FROM users WHERE id = 10;
来源：http://nc.nicolike.cn

[Q53] 按条件删除
来源：http://hl.szsharing.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://eu.jctech888.com.cn

[Q54] 清空表
来源：http://rm.huixinmuqiang.cn

TRUNCATE TABLE logs;
来源：http://cy.huanxung.cn

[Q55] 排名（并列占位）
来源：http://ns.shxzskj.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://oy.bookmarksfly.cn

[Q56] 密集排名（并列不占位）
来源：http://cy.szsharing.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://eh.lnxyls.cn

[Q57] 行号
来源：http://dp.yuntaijiaju.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://pm.huixinmuqiang.cn

[Q58] 累计求和
来源：http://xp.jianghongdianzi.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ew.wgjwhj.cn

[Q59] 分组内累计
来源：http://in.jianghongdianzi.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://un.yuntaijiaju.cn

[Q60] 取上一行 / 下一行
来源：http://oq.521024.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://zc.bjjhwx.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://zz.shxzskj.cn

[Q61] 移动平均
来源：http://sq.newstarts.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://fd.szsharing.cn

[Q62] 分组占比
来源：http://dd.jianghongdianzi.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://pd.newstarts.cn

[Q63] 开启事务
来源：http://uh.9csxet.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://ey.nicolike.cn

[Q64] 提交事务
来源：http://aq.nszjky.cn

COMMIT;
来源：http://xj.9csxet.cn

[Q65] 回滚事务
来源：http://av.yuntaijiaju.cn

ROLLBACK;
来源：http://td.9csxet.cn

[Q66] 行锁查询
来源：http://qy.bookmarksfly.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://pu.szsharing.cn

[Q67] 设置隔离级别
来源：http://wj.wgjwhj.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://vm.szsharing.cn

[Q68] 保存点
来源：http://ys.521024.cn

SAVEPOINT sp1;
来源：http://ra.shxzukj.cn

ROLLBACK TO sp1;
来源：http://zo.muxihuayi.cn

[Q69] 查看执行计划
来源：http://tv.nszjky.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://sp.jianghongdianzi.cn

[Q70] 更新统计信息
来源：http://er.muxihuayi.cn

ANALYZE TABLE users;
来源：http://fy.huanxung.cn

[Q71] 查看建表语句
来源：http://es.521024.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://dj.521024.cn

[Q72] 查看索引
来源：http://dh.colortex.cn

SHOW INDEX FROM users;
来源：http://fb.huanxung.cn

[Q73] 查看表状态
来源：http://je.wgjwhj.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://ro.chemitech.net.cn

[Q74] 强制使用索引
来源：http://vl.hahajie.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://yx.yuntaijiaju.cn

[Q75] 日期格式化
来源：http://sn.szxytkj.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://dr.nszjky.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://rd.hahajie.cn

[Q76] 按天统计
来源：http://ck.wgjwhj.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://at.shxzskj.cn

[Q77] 时间加减
来源：http://vc.asd995.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://tl.nicolike.cn

[Q78] 当前时间
来源：http://je.bjjhwx.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://lv.gzmigu.cn

[Q79] 字符串拼接
来源：http://bc.szsharing.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ie.gzmigu.cn

[Q80] 字符串截取
来源：http://qc.521024.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://vo.shxzskj.cn

[Q81] 字符串替换
来源：http://kb.colortex.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://xp.hnjuh.cn

[Q82] 字符长度与字节长度
来源：http://li.huixiangedu.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wg.huanxung.cn

[Q83] 大小写转换
来源：http://td.shtwfgs.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ho.huixinmuqiang.cn

[Q84] 去除首尾空格
来源：http://bi.wgjwhj.cn

SELECT TRIM(name) FROM users;
来源：http://ru.shxzukj.cn

[Q85] 数值取整
来源：http://hg.muxihuayi.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ve.muxihuayi.cn

[Q86] 读取 JSON 字段
来源：http://ft.jianghongdianzi.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://sv.bookmarksfly.cn

[Q87] JSON 字段做条件
来源：http://tp.nszjky.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://jo.jctech888.com.cn

[Q88] 行转列（条件聚合）
来源：http://wh.muxihuayi.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ud.colortex.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://pr.hahajie.cn

[Q89] 判断表是否存在
来源：http://ru.gzmigu.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ba.jctech888.com.cn

[Q90] 生成序号列
来源：http://fp.colortex.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://no.yuexingan06.cn

================================================================================
来源：http://ei.haigaiapp.cn

R. Bash 专题
来源：http://hh.jctech888.com.cn

================================================================================
来源：http://lv.jianghongdianzi.cn

[R01] shebang 与严格模式
来源：http://rl.9csxet.cn

#!/usr/bin/env bash
来源：http://td.9csxet.cn

set -euo pipefail
来源：http://re.hnjuh.cn

[R02] 变量赋值与使用
来源：http://mi.panjiajie.cn

name="Tom"; echo "$name"
来源：http://tr.shxzskj.cn

[R03] 只读变量
来源：http://pe.bookmarksfly.cn

readonly PI=3.14
来源：http://ss.gzmigu.cn

[R04] 位置参数
来源：http://xf.bookmarksfly.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://lg.gzmigu.cn

[R05] 参数默认值
来源：http://nm.hahajie.cn

name="${1:-default}"
来源：http://kp.huixinmuqiang.cn

[R06] 判断命令是否存在
来源：http://xn.muxihuayi.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://pk.huixiangedu.cn

[R07] if 判断文件
来源：http://nk.szxytkj.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://xe.gzmigu.cn

[R08] 数值比较
来源：http://ux.yuexingan06.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://tc.shxzukj.cn

[R09] 字符串比较
来源：http://mr.huixinmuqiang.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ss.huanxung.cn

[R10] 正则匹配
来源：http://ey.szxytkj.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://zp.szsharing.cn

[R11] case 多分支
来源：http://wb.gzmigu.cn

case "$1" in
来源：http://cq.9csxet.cn

start) echo "启动" ;;
来源：http://qn.newstarts.cn

stop)  echo "停止" ;;
来源：http://dx.jctech888.com.cn

*)     echo "未知命令" ;;
来源：http://gk.gzmigu.cn

esac
来源：http://hs.newstarts.cn

[R12] for 遍历文件
来源：http://ux.panjiajie.cn

for f in *.txt; do echo "$f"; done
来源：http://gp.huixiangedu.cn

[R13] for 计数循环
来源：http://xj.huanxung.cn

for i in {1..10}; do echo "$i"; done
来源：http://cb.muxihuayi.cn

[R14] C 风格 for
来源：http://cr.muxihuayi.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://um.nszjky.cn

[R15] while 逐行读文件
来源：http://ti.muxihuayi.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://jn.gzmigu.cn

[R16] until 等待条件
来源：http://uc.nszjky.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ap.hnjuh.cn

[R17] 数组定义与取值
来源：http://ff.nicolike.cn

arr=(a b c); echo "${arr[0]}"
来源：http://uw.haigaiapp.cn

[R18] 遍历数组
来源：http://jr.jctech888.com.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mb.huixiangedu.cn

[R19] 数组长度
来源：http://rb.huixinmuqiang.cn

echo "${#arr[@]}"
来源：http://hl.chemitech.net.cn

[R20] 关联数组（字典）
来源：http://oa.yuntaijiaju.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://dt.shtwfgs.cn

[R21] 字符串长度
来源：http://by.9csxet.cn

echo "${#s}"
来源：http://vi.haigaiapp.cn

[R22] 截取子串
来源：http://jw.colortex.cn

echo "${s:0:5}"
来源：http://sa.bookmarksfly.cn

[R23] 字符串替换
来源：http://pf.muxihuayi.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ky.gzmigu.cn

[R24] 大小写转换
来源：http://fn.nszjky.cn

echo "${s^^}"; echo "${s,,}"
来源：http://nc.szsharing.cn

[R25] 去后缀 / 去前缀
来源：http://pk.colortex.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://mc.bjjhwx.cn

[R26] 命令替换
来源：http://sn.huixiangedu.cn

now=$(date +%F); echo "$now"
来源：http://zm.gzmigu.cn

[R27] 算术展开
来源：http://cq.szsharing.cn

echo $((1 + 2 * 3))
来源：http://zf.hahajie.cn

[R28] 浮点运算
来源：http://zj.lnxyls.cn

echo "scale=2; 10/3" | bc
来源：http://qj.jianghongdianzi.cn

[R29] 定义函数
来源：http://bq.lnxyls.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://as.521024.cn

[R30] 函数返回状态码
来源：http://cy.gzmigu.cn

f() { return 0; }; f || echo "失败了"
来源：http://mo.521024.cn

[R31] 局部变量
来源：http://po.szsharing.cn

f() { local x=1; echo "$x"; }
来源：http://os.yuexingan06.cn

[R32] 参数个数校验
来源：http://fh.shxzskj.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://vy.huanxung.cn

[R33] 捕获错误并提示行号
来源：http://mw.bjjhwx.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://uz.colortex.cn

[R34] 退出时清理
来源：http://bl.bjjhwx.cn

trap 'rm -f "$tmp"' EXIT
来源：http://vd.bjjhwx.cn

[R35] 后台执行并等待
来源：http://qt.huixiangedu.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://wo.chemitech.net.cn

[R36] 并发执行多个任务
来源：http://qd.yuntaijiaju.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ii.lnxyls.cn

[R37] 把输出赋给变量
来源：http://ed.huixinmuqiang.cn

files=$(ls -1)
来源：http://ii.hahajie.cn

[R38] 管道串联
来源：http://mq.szxytkj.cn

cat a.txt | grep -i error | wc -l
来源：http://ze.huixiangedu.cn

[R39] 重定向标准输出与错误
来源：http://on.nszjky.cn

cmd > out.log 2>&1
来源：http://mx.9csxet.cn

[R40] 追加写日志
来源：http://qj.521024.cn

echo "log" >> out.log
来源：http://cp.hahajie.cn

[R41] 丢弃输出
来源：http://gt.521024.cn

cmd >/dev/null 2>&1
来源：http://aq.szxytkj.cn

[R42] 输入重定向
来源：http://rw.bookmarksfly.cn

wc -l < a.txt
来源：http://ko.szxytkj.cn

[R43] 按名字查找文件
来源：http://yz.szxytkj.cn

find . -name "*.log" -type f
来源：http://ft.muxihuayi.cn

[R44] 按修改时间查找
来源：http://kr.nicolike.cn

find . -mtime -7 -type f
来源：http://zl.bjjhwx.cn

[R45] 批量删除
来源：http://du.521024.cn

find . -name "*.tmp" -delete
来源：http://nh.nicolike.cn

[R46] 递归替换文件内容
来源：http://wf.shxzukj.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ra.hahajie.cn

[R47] sed 单行替换
来源：http://pl.nszjky.cn

sed -i 's/foo/bar/g' a.txt
来源：http://gh.jctech888.com.cn

[R48] awk 取指定列
来源：http://tl.gzmigu.cn

awk '{print $1, $3}' a.txt
来源：http://pa.hnjuh.cn

[R49] awk 带条件
来源：http://do.shxzskj.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://xq.521024.cn

[R50] awk 求和
来源：http://dd.gzmigu.cn

awk '{s += $2} END {print s}' a.txt
来源：http://zj.muxihuayi.cn

[R51] 排序去重取前几
来源：http://zi.9csxet.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://yi.szxytkj.cn

[R52] 统计行数
来源：http://sf.jctech888.com.cn

wc -l a.txt
来源：http://do.nszjky.cn

[R53] 查看文件头与实时尾
来源：http://li.jctech888.com.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://kl.panjiajie.cn

[R54] 比较两个文件
来源：http://sj.jianghongdianzi.cn

diff a.txt b.txt
来源：http://ib.panjiajie.cn

[R55] 压缩与解压
来源：http://ea.gzmigu.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://yu.newstarts.cn

[R56] 远程拷贝
来源：http://fi.521024.cn

scp file user@host:/path/
来源：http://xi.huixiangedu.cn

[R57] 远程执行命令
来源：http://rn.nszjky.cn

ssh user@host 'uptime'
来源：http://xo.yuexingan06.cn

[R58] 下载文件
来源：http://vx.asd995.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://oh.muxihuayi.cn

[R59] 发 POST JSON
来源：http://jx.newstarts.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://pl.chemitech.net.cn

[R60] 只看 HTTP 状态码
来源：http://hg.jianghongdianzi.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://dx.bookmarksfly.cn

[R61] 磁盘占用
来源：http://et.muxihuayi.cn

df -h;  du -sh *
来源：http://wj.shtwfgs.cn

[R62] 找最占空间的文件
来源：http://nc.gzmigu.cn

du -ah . | sort -rh | head -10
来源：http://ri.muxihuayi.cn

[R63] 内存与进程
来源：http://ri.huixiangedu.cn

free -h;  ps aux | grep nginx
来源：http://km.lnxyls.cn

[R64] 结束进程
来源：http://oy.521024.cn

kill -9 $(pgrep -f app.py)
来源：http://hc.nicolike.cn

[R65] 查看端口占用
来源：http://hu.shxzukj.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://oi.yuexingan06.cn

[R66] 定时任务
来源：http://ip.jianghongdianzi.cn

crontab -e;  crontab -l
来源：http://jd.huixiangedu.cn

[R67] 生成随机十六进制串
来源：http://za.shxzskj.cn

openssl rand -hex 16
来源：http://gu.muxihuayi.cn

[R68] 计算文件校验值
来源：http://rx.521024.cn

sha256sum a.txt;  md5sum a.txt
来源：http://yu.yuntaijiaju.cn

[R69] 生成随机密码
来源：http://mk.asd995.cn

head -c 16 /dev/urandom | base64
来源：http://mc.yuntaijiaju.cn

[R70] 时间戳与互转
来源：http://ol.lnxyls.cn

date +%s;  date -d @1700000000
来源：http://ur.newstarts.cn

[R71] 日期格式化
来源：http://jz.haigaiapp.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://uw.muxihuayi.cn

[R72] 等待端口就绪
来源：http://dd.newstarts.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://iw.521024.cn

[R73] 分割大日志
来源：http://on.nicolike.cn

split -l 1000 big.log part_
来源：http://wb.bjjhwx.cn

[R74] 批量重命名
来源：http://du.wgjwhj.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://kq.huixinmuqiang.cn

[R75] 导出环境变量
来源：http://bz.hnjuh.cn

export PATH="$HOME/bin:$PATH"
来源：http://qm.shtwfgs.cn

[R76] 使用临时文件
来源：http://oo.gzmigu.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://tm.asd995.cn

[R77] 读取用户输入
来源：http://rn.wgjwhj.cn


<!-- 参考信息 -->