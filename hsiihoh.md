代发 wailian999

[Q33] 多列分组
来源：http://vg.nicolike.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://uh.yuntaijiaju.cn

[Q34] 每组取第一条
来源：http://ac.colortex.cn

SELECT * FROM (
来源：http://wb.shtwfgs.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://qc.9csxet.cn

) t WHERE rn = 1;
来源：http://sl.haigaiapp.cn

[Q35] 内连接
来源：http://iu.szxytkj.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wj.jctech888.com.cn

[Q36] 左连接
来源：http://au.yuexingan06.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ry.nszjky.cn

[Q37] 右连接
来源：http://hu.muxihuayi.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://os.jctech888.com.cn

[Q38] 全外连接（PostgreSQL）
来源：http://pn.newstarts.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://cq.jctech888.com.cn

[Q39] 自连接（查上下级）
来源：http://qc.haigaiapp.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://zq.hnjuh.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ae.huixiangedu.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://xz.muxihuayi.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wr.nicolike.cn

[Q41] 多表连接
来源：http://ei.lnxyls.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://uu.gzmigu.cn

JOIN users u ON u.id = o.user_id
来源：http://tn.bjjhwx.cn

JOIN products p ON p.id = o.product_id;
来源：http://hq.shxzskj.cn

[Q42] 连接条件附加过滤
来源：http://pl.bookmarksfly.cn

SELECT u.name, o.amount FROM users u
来源：http://db.asd995.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wv.yuntaijiaju.cn

[Q43] 标量子查询
来源：http://hv.yuexingan06.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://fk.huixiangedu.cn

[Q44] IN 子查询
来源：http://th.huixiangedu.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://fe.gzmigu.cn

[Q45] EXISTS 判断存在
来源：http://ez.panjiajie.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://po.gzmigu.cn

[Q46] NOT EXISTS 判断不存在
来源：http://yb.panjiajie.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://um.panjiajie.cn

[Q47] 与平均值比较
来源：http://co.nicolike.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ww.nicolike.cn

[Q48] CTE 公用表表达式
来源：http://hp.gzmigu.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hr.haigaiapp.cn

SELECT * FROM t WHERE c > 5;
来源：http://nh.huixiangedu.cn

[Q49] 更新单行
来源：http://tv.lnxyls.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ew.shxzukj.cn

[Q50] 批量更新
来源：http://lw.haigaiapp.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://vf.asd995.cn

[Q51] 用子查询更新
来源：http://on.hnjuh.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://ov.huixiangedu.cn

[Q52] 删除指定行
来源：http://yl.asd995.cn

DELETE FROM users WHERE id = 10;
来源：http://kv.wgjwhj.cn

[Q53] 按条件删除
来源：http://py.521024.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://te.jctech888.com.cn

[Q54] 清空表
来源：http://hw.521024.cn

TRUNCATE TABLE logs;
来源：http://dl.yuexingan06.cn

[Q55] 排名（并列占位）
来源：http://iv.bookmarksfly.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://re.bookmarksfly.cn

[Q56] 密集排名（并列不占位）
来源：http://bu.huixiangedu.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ab.wgjwhj.cn

[Q57] 行号
来源：http://ku.newstarts.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://vi.nicolike.cn

[Q58] 累计求和
来源：http://ec.huanxung.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ig.panjiajie.cn

[Q59] 分组内累计
来源：http://om.haigaiapp.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ja.hahajie.cn

[Q60] 取上一行 / 下一行
来源：http://kb.muxihuayi.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://pc.jctech888.com.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ui.szsharing.cn

[Q61] 移动平均
来源：http://gu.huixinmuqiang.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://qf.panjiajie.cn

[Q62] 分组占比
来源：http://di.panjiajie.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://rf.yuexingan06.cn

[Q63] 开启事务
来源：http://vo.nszjky.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://ol.chemitech.net.cn

[Q64] 提交事务
来源：http://th.nszjky.cn

COMMIT;
来源：http://hi.huanxung.cn

[Q65] 回滚事务
来源：http://dn.lnxyls.cn

ROLLBACK;
来源：http://gg.hahajie.cn

[Q66] 行锁查询
来源：http://tp.lnxyls.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://eb.colortex.cn

[Q67] 设置隔离级别
来源：http://ow.haigaiapp.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mc.bookmarksfly.cn

[Q68] 保存点
来源：http://pq.panjiajie.cn

SAVEPOINT sp1;
来源：http://zu.lnxyls.cn

ROLLBACK TO sp1;
来源：http://tj.hnjuh.cn

[Q69] 查看执行计划
来源：http://qt.yuexingan06.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://lo.9csxet.cn

[Q70] 更新统计信息
来源：http://ce.wgjwhj.cn

ANALYZE TABLE users;
来源：http://wm.szsharing.cn

[Q71] 查看建表语句
来源：http://al.huixiangedu.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://gz.szsharing.cn

[Q72] 查看索引
来源：http://lu.panjiajie.cn

SHOW INDEX FROM users;
来源：http://tr.newstarts.cn

[Q73] 查看表状态
来源：http://lm.haigaiapp.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://iy.hnjuh.cn

[Q74] 强制使用索引
来源：http://ag.newstarts.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://dn.szxytkj.cn

[Q75] 日期格式化
来源：http://nn.yuntaijiaju.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://yz.haigaiapp.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://rk.nszjky.cn

[Q76] 按天统计
来源：http://iz.hahajie.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://lc.gzmigu.cn

[Q77] 时间加减
来源：http://iy.muxihuayi.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://al.jctech888.com.cn

[Q78] 当前时间
来源：http://by.jctech888.com.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://gm.shxzskj.cn

[Q79] 字符串拼接
来源：http://jd.panjiajie.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://jw.szxytkj.cn

[Q80] 字符串截取
来源：http://en.wgjwhj.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://bw.bjjhwx.cn

[Q81] 字符串替换
来源：http://ag.gzmigu.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mw.wgjwhj.cn

[Q82] 字符长度与字节长度
来源：http://kh.yuntaijiaju.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://qs.szxytkj.cn

[Q83] 大小写转换
来源：http://hr.colortex.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ta.huixiangedu.cn

[Q84] 去除首尾空格
来源：http://yr.chemitech.net.cn

SELECT TRIM(name) FROM users;
来源：http://qn.hahajie.cn

[Q85] 数值取整
来源：http://iv.chemitech.net.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ib.huixiangedu.cn

[Q86] 读取 JSON 字段
来源：http://wv.jianghongdianzi.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://cy.9csxet.cn

[Q87] JSON 字段做条件
来源：http://dp.wgjwhj.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ht.nicolike.cn

[Q88] 行转列（条件聚合）
来源：http://fu.shxzskj.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://rc.bjjhwx.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://vc.chemitech.net.cn

[Q89] 判断表是否存在
来源：http://ab.jctech888.com.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://un.521024.cn

[Q90] 生成序号列
来源：http://ar.521024.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://nl.jctech888.com.cn

================================================================================
来源：http://ba.asd995.cn

R. Bash 专题
来源：http://de.newstarts.cn

================================================================================
来源：http://td.muxihuayi.cn

[R01] shebang 与严格模式
来源：http://ra.jianghongdianzi.cn

#!/usr/bin/env bash
来源：http://jg.huixinmuqiang.cn

set -euo pipefail
来源：http://je.haigaiapp.cn

[R02] 变量赋值与使用
来源：http://we.asd995.cn

name="Tom"; echo "$name"
来源：http://sk.huixinmuqiang.cn

[R03] 只读变量
来源：http://mv.shtwfgs.cn

readonly PI=3.14
来源：http://mh.jianghongdianzi.cn

[R04] 位置参数
来源：http://vl.hnjuh.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://bd.hnjuh.cn

[R05] 参数默认值
来源：http://ek.hahajie.cn

name="${1:-default}"
来源：http://go.wgjwhj.cn

[R06] 判断命令是否存在
来源：http://iv.colortex.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://gb.jctech888.com.cn

[R07] if 判断文件
来源：http://wd.gzmigu.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hn.gzmigu.cn

[R08] 数值比较
来源：http://fg.bjjhwx.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://kt.colortex.cn

[R09] 字符串比较
来源：http://bj.hahajie.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hr.wgjwhj.cn

[R10] 正则匹配
来源：http://fl.szsharing.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://jh.hahajie.cn

[R11] case 多分支
来源：http://ih.chemitech.net.cn

case "$1" in
来源：http://oj.bookmarksfly.cn

start) echo "启动" ;;
来源：http://np.shxzskj.cn

stop)  echo "停止" ;;
来源：http://vz.shxzskj.cn

*)     echo "未知命令" ;;
来源：http://iw.gzmigu.cn

esac
来源：http://dg.jctech888.com.cn

[R12] for 遍历文件
来源：http://ra.muxihuayi.cn

for f in *.txt; do echo "$f"; done
来源：http://ou.shxzukj.cn

[R13] for 计数循环
来源：http://vt.shtwfgs.cn

for i in {1..10}; do echo "$i"; done
来源：http://vb.huixinmuqiang.cn

[R14] C 风格 for
来源：http://zr.yuexingan06.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://rw.lnxyls.cn

[R15] while 逐行读文件
来源：http://ut.nicolike.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hk.wgjwhj.cn

[R16] until 等待条件
来源：http://oa.hahajie.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://xm.chemitech.net.cn

[R17] 数组定义与取值
来源：http://cz.gzmigu.cn

arr=(a b c); echo "${arr[0]}"
来源：http://rm.jctech888.com.cn

[R18] 遍历数组
来源：http://uc.yuntaijiaju.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hu.yuexingan06.cn

[R19] 数组长度
来源：http://iw.chemitech.net.cn

echo "${#arr[@]}"
来源：http://wc.shxzukj.cn

[R20] 关联数组（字典）
来源：http://gg.haigaiapp.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://qm.yuexingan06.cn

[R21] 字符串长度
来源：http://cc.muxihuayi.cn

echo "${#s}"
来源：http://oz.jctech888.com.cn

[R22] 截取子串
来源：http://gb.asd995.cn

echo "${s:0:5}"
来源：http://yl.lnxyls.cn

[R23] 字符串替换
来源：http://wc.nszjky.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ux.bjjhwx.cn

[R24] 大小写转换
来源：http://hi.chemitech.net.cn

echo "${s^^}"; echo "${s,,}"
来源：http://mt.bookmarksfly.cn

[R25] 去后缀 / 去前缀
来源：http://mc.gzmigu.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://al.huixinmuqiang.cn

[R26] 命令替换
来源：http://xj.colortex.cn

now=$(date +%F); echo "$now"
来源：http://mi.yuexingan06.cn

[R27] 算术展开
来源：http://gm.szsharing.cn

echo $((1 + 2 * 3))
来源：http://th.colortex.cn

[R28] 浮点运算
来源：http://sh.haigaiapp.cn

echo "scale=2; 10/3" | bc
来源：http://em.shxzskj.cn

[R29] 定义函数
来源：http://xv.szxytkj.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://yc.gzmigu.cn

[R30] 函数返回状态码
来源：http://bo.szxytkj.cn

f() { return 0; }; f || echo "失败了"
来源：http://ct.colortex.cn

[R31] 局部变量
来源：http://hu.jianghongdianzi.cn

f() { local x=1; echo "$x"; }
来源：http://jh.huixinmuqiang.cn

[R32] 参数个数校验
来源：http://td.bjjhwx.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://jl.jctech888.com.cn

[R33] 捕获错误并提示行号
来源：http://ol.yuntaijiaju.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ey.nicolike.cn

[R34] 退出时清理
来源：http://am.jctech888.com.cn

trap 'rm -f "$tmp"' EXIT
来源：http://ci.shxzukj.cn

[R35] 后台执行并等待
来源：http://tp.9csxet.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://hg.bjjhwx.cn

[R36] 并发执行多个任务
来源：http://tq.newstarts.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://jm.panjiajie.cn

[R37] 把输出赋给变量
来源：http://pp.huixinmuqiang.cn

files=$(ls -1)
来源：http://lt.huanxung.cn

[R38] 管道串联
来源：http://uc.colortex.cn

cat a.txt | grep -i error | wc -l
来源：http://qn.shxzukj.cn

[R39] 重定向标准输出与错误
来源：http://og.colortex.cn

cmd > out.log 2>&1
来源：http://lr.gzmigu.cn

[R40] 追加写日志
来源：http://lk.panjiajie.cn

echo "log" >> out.log
来源：http://kw.shtwfgs.cn

[R41] 丢弃输出
来源：http://ay.wgjwhj.cn

cmd >/dev/null 2>&1
来源：http://ah.wgjwhj.cn

[R42] 输入重定向
来源：http://bc.yuexingan06.cn

wc -l < a.txt
来源：http://dq.colortex.cn

[R43] 按名字查找文件
来源：http://gl.huixiangedu.cn

find . -name "*.log" -type f
来源：http://kv.nicolike.cn

[R44] 按修改时间查找
来源：http://qr.shxzukj.cn

find . -mtime -7 -type f
来源：http://ku.bjjhwx.cn

[R45] 批量删除
来源：http://zk.hnjuh.cn

find . -name "*.tmp" -delete
来源：http://wo.shxzukj.cn

[R46] 递归替换文件内容
来源：http://ck.jctech888.com.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ye.wgjwhj.cn

[R47] sed 单行替换
来源：http://fp.jctech888.com.cn

sed -i 's/foo/bar/g' a.txt
来源：http://tr.huixiangedu.cn

[R48] awk 取指定列
来源：http://ru.jctech888.com.cn

awk '{print $1, $3}' a.txt
来源：http://ck.bookmarksfly.cn

[R49] awk 带条件
来源：http://ql.chemitech.net.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ge.huanxung.cn

[R50] awk 求和
来源：http://tv.huixinmuqiang.cn

awk '{s += $2} END {print s}' a.txt
来源：http://ht.shxzukj.cn

[R51] 排序去重取前几
来源：http://ax.bjjhwx.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://aa.jctech888.com.cn

[R52] 统计行数
来源：http://fx.szxytkj.cn

wc -l a.txt
来源：http://is.huixiangedu.cn

[R53] 查看文件头与实时尾
来源：http://mx.lnxyls.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://qf.asd995.cn

[R54] 比较两个文件
来源：http://pd.yuexingan06.cn

diff a.txt b.txt
来源：http://fh.szsharing.cn

[R55] 压缩与解压
来源：http://dv.gzmigu.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://fp.szxytkj.cn

[R56] 远程拷贝
来源：http://qe.muxihuayi.cn

scp file user@host:/path/
来源：http://dw.wgjwhj.cn

[R57] 远程执行命令
来源：http://rh.huanxung.cn

ssh user@host 'uptime'
来源：http://tp.yuntaijiaju.cn

[R58] 下载文件
来源：http://nt.asd995.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://et.gzmigu.cn

[R59] 发 POST JSON
来源：http://as.nszjky.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://nm.szxytkj.cn

[R60] 只看 HTTP 状态码
来源：http://vh.huixiangedu.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://nz.panjiajie.cn

[R61] 磁盘占用
来源：http://hi.wgjwhj.cn

df -h;  du -sh *
来源：http://xr.nicolike.cn

[R62] 找最占空间的文件
来源：http://ql.chemitech.net.cn

du -ah . | sort -rh | head -10
来源：http://pk.haigaiapp.cn

[R63] 内存与进程
来源：http://lz.9csxet.cn

free -h;  ps aux | grep nginx
来源：http://eq.asd995.cn

[R64] 结束进程
来源：http://ej.huanxung.cn

kill -9 $(pgrep -f app.py)
来源：http://ju.szsharing.cn

[R65] 查看端口占用
来源：http://tw.muxihuayi.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://cb.huixinmuqiang.cn

[R66] 定时任务
来源：http://qw.chemitech.net.cn

crontab -e;  crontab -l
来源：http://lh.521024.cn

[R67] 生成随机十六进制串
来源：http://mn.9csxet.cn

openssl rand -hex 16
来源：http://oa.shxzskj.cn

[R68] 计算文件校验值
来源：http://dh.yuntaijiaju.cn

sha256sum a.txt;  md5sum a.txt
来源：http://ch.jctech888.com.cn

[R69] 生成随机密码
来源：http://iv.newstarts.cn

head -c 16 /dev/urandom | base64
来源：http://oj.521024.cn

[R70] 时间戳与互转
来源：http://id.gzmigu.cn

date +%s;  date -d @1700000000
来源：http://ud.9csxet.cn

[R71] 日期格式化
来源：http://qw.muxihuayi.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://lz.chemitech.net.cn

[R72] 等待端口就绪
来源：http://cn.huanxung.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://jy.nszjky.cn

[R73] 分割大日志
来源：http://hp.hahajie.cn

split -l 1000 big.log part_
来源：http://qu.yuexingan06.cn

[R74] 批量重命名
来源：http://tf.hahajie.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://kb.nszjky.cn

[R75] 导出环境变量
来源：http://yu.yuexingan06.cn

export PATH="$HOME/bin:$PATH"
来源：http://wa.nicolike.cn

[R76] 使用临时文件
来源：http://gh.muxihuayi.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ga.panjiajie.cn

[R77] 读取用户输入
来源：http://go.colortex.cn

read -rp "请输入: " ans
来源：http://al.newstarts.cn

[R78] 交互式菜单
来源：http://lo.jctech888.com.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://mp.lnxyls.cn

[R79] 解析命令行选项
来源：http://ew.lnxyls.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://me.jianghongdianzi.cn

[R80] 查看脚本执行耗时
来源：http://qn.szsharing.cn

time ./run.sh
来源：http://ye.szsharing.cn

================================================================================
来源：http://xt.yuntaijiaju.cn

S. C / C++ 专题
来源：http://si.521024.cn

================================================================================
来源：http://fl.shxzskj.cn

[S01] C：Hello World
来源：http://qh.haigaiapp.cn

#include <stdio.h>
来源：http://an.lnxyls.cn


<!-- 参考信息 -->