代发 wailian999

SELECT MAX(age), MIN(age) FROM users;
来源：http://zb.yuntaijiaju.cn

[Q30] 分组统计
来源：http://wv.asd995.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://nx.shxzukj.cn

[Q31] 分组后过滤
来源：http://jd.huixiangedu.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://sb.shxzskj.cn

[Q32] 分组拼接字符串
来源：http://hs.huixiangedu.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://qg.shxzukj.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://pt.bookmarksfly.cn

[Q33] 多列分组
来源：http://uv.521024.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://pw.muxihuayi.cn

[Q34] 每组取第一条
来源：http://po.lnxyls.cn

SELECT * FROM (
来源：http://mz.shtwfgs.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://om.gzmigu.cn

) t WHERE rn = 1;
来源：http://kg.szsharing.cn

[Q35] 内连接
来源：http://bg.jctech888.com.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://fj.wgjwhj.cn

[Q36] 左连接
来源：http://yu.lnxyls.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ga.shtwfgs.cn

[Q37] 右连接
来源：http://oq.colortex.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://uq.newstarts.cn

[Q38] 全外连接（PostgreSQL）
来源：http://kg.chemitech.net.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mo.nicolike.cn

[Q39] 自连接（查上下级）
来源：http://kr.chemitech.net.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://ha.9csxet.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://aa.haigaiapp.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://ya.newstarts.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://do.haigaiapp.cn

[Q41] 多表连接
来源：http://ya.newstarts.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://el.huixinmuqiang.cn

JOIN users u ON u.id = o.user_id
来源：http://jz.gzmigu.cn

JOIN products p ON p.id = o.product_id;
来源：http://ch.hahajie.cn

[Q42] 连接条件附加过滤
来源：http://tn.lnxyls.cn

SELECT u.name, o.amount FROM users u
来源：http://us.muxihuayi.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://nq.newstarts.cn

[Q43] 标量子查询
来源：http://st.hnjuh.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://zb.nszjky.cn

[Q44] IN 子查询
来源：http://ha.yuntaijiaju.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://xq.shxzukj.cn

[Q45] EXISTS 判断存在
来源：http://yc.panjiajie.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://eu.haigaiapp.cn

[Q46] NOT EXISTS 判断不存在
来源：http://wg.yuntaijiaju.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://fn.9csxet.cn

[Q47] 与平均值比较
来源：http://ba.muxihuayi.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://gi.bookmarksfly.cn

[Q48] CTE 公用表表达式
来源：http://bl.gzmigu.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://bf.bookmarksfly.cn

SELECT * FROM t WHERE c > 5;
来源：http://xu.haigaiapp.cn

[Q49] 更新单行
来源：http://kc.wgjwhj.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://iz.nszjky.cn

[Q50] 批量更新
来源：http://bq.huanxung.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://tk.bjjhwx.cn

[Q51] 用子查询更新
来源：http://pv.huixiangedu.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://dw.szxytkj.cn

[Q52] 删除指定行
来源：http://sf.szxytkj.cn

DELETE FROM users WHERE id = 10;
来源：http://ag.nicolike.cn

[Q53] 按条件删除
来源：http://ic.huixinmuqiang.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://nz.szsharing.cn

[Q54] 清空表
来源：http://uw.shxzukj.cn

TRUNCATE TABLE logs;
来源：http://sm.huanxung.cn

[Q55] 排名（并列占位）
来源：http://pc.shxzukj.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ew.shxzukj.cn

[Q56] 密集排名（并列不占位）
来源：http://cd.wgjwhj.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://dn.shtwfgs.cn

[Q57] 行号
来源：http://pt.szsharing.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://cz.jianghongdianzi.cn

[Q58] 累计求和
来源：http://of.colortex.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ox.gzmigu.cn

[Q59] 分组内累计
来源：http://ne.shtwfgs.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://nz.hahajie.cn

[Q60] 取上一行 / 下一行
来源：http://am.asd995.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://zr.haigaiapp.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://nj.haigaiapp.cn

[Q61] 移动平均
来源：http://rc.huixiangedu.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://th.hnjuh.cn

[Q62] 分组占比
来源：http://xl.yuexingan06.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ms.panjiajie.cn

[Q63] 开启事务
来源：http://mh.szsharing.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://if.lnxyls.cn

[Q64] 提交事务
来源：http://oh.lnxyls.cn

COMMIT;
来源：http://vh.nicolike.cn

[Q65] 回滚事务
来源：http://mz.shxzukj.cn

ROLLBACK;
来源：http://jq.panjiajie.cn

[Q66] 行锁查询
来源：http://mz.haigaiapp.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ue.jctech888.com.cn

[Q67] 设置隔离级别
来源：http://wn.shtwfgs.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hh.bjjhwx.cn

[Q68] 保存点
来源：http://xn.bjjhwx.cn

SAVEPOINT sp1;
来源：http://uf.nicolike.cn

ROLLBACK TO sp1;
来源：http://bf.chemitech.net.cn

[Q69] 查看执行计划
来源：http://yf.panjiajie.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ab.lnxyls.cn

[Q70] 更新统计信息
来源：http://pp.asd995.cn

ANALYZE TABLE users;
来源：http://pf.gzmigu.cn

[Q71] 查看建表语句
来源：http://nu.huixiangedu.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ik.huixinmuqiang.cn

[Q72] 查看索引
来源：http://ia.colortex.cn

SHOW INDEX FROM users;
来源：http://rq.yuexingan06.cn

[Q73] 查看表状态
来源：http://si.asd995.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://lo.haigaiapp.cn

[Q74] 强制使用索引
来源：http://uy.shxzukj.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://rz.shxzukj.cn

[Q75] 日期格式化
来源：http://io.shtwfgs.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://um.lnxyls.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://rr.yuntaijiaju.cn

[Q76] 按天统计
来源：http://yn.bjjhwx.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://vr.muxihuayi.cn

[Q77] 时间加减
来源：http://qk.521024.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ig.hnjuh.cn

[Q78] 当前时间
来源：http://os.colortex.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://yj.szsharing.cn

[Q79] 字符串拼接
来源：http://tm.huixiangedu.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://nk.haigaiapp.cn

[Q80] 字符串截取
来源：http://gu.yuntaijiaju.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://aq.yuexingan06.cn

[Q81] 字符串替换
来源：http://qt.huanxung.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hk.yuexingan06.cn

[Q82] 字符长度与字节长度
来源：http://da.muxihuayi.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://tj.hahajie.cn

[Q83] 大小写转换
来源：http://lv.szxytkj.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://qb.szsharing.cn

[Q84] 去除首尾空格
来源：http://uc.gzmigu.cn

SELECT TRIM(name) FROM users;
来源：http://ah.huixinmuqiang.cn

[Q85] 数值取整
来源：http://nm.gzmigu.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://kl.shxzukj.cn

[Q86] 读取 JSON 字段
来源：http://wd.newstarts.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hi.huanxung.cn

[Q87] JSON 字段做条件
来源：http://lr.shtwfgs.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://pz.hahajie.cn

[Q88] 行转列（条件聚合）
来源：http://yv.szsharing.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mh.bjjhwx.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://vg.lnxyls.cn

[Q89] 判断表是否存在
来源：http://su.huanxung.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://rc.szsharing.cn

[Q90] 生成序号列
来源：http://pe.gzmigu.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://zw.yuexingan06.cn

================================================================================
来源：http://vq.szxytkj.cn

R. Bash 专题
来源：http://cy.yuexingan06.cn

================================================================================
来源：http://ae.panjiajie.cn

[R01] shebang 与严格模式
来源：http://jl.yuntaijiaju.cn

#!/usr/bin/env bash
来源：http://al.hahajie.cn

set -euo pipefail
来源：http://vf.shtwfgs.cn

[R02] 变量赋值与使用
来源：http://tq.yuexingan06.cn

name="Tom"; echo "$name"
来源：http://qw.colortex.cn

[R03] 只读变量
来源：http://lc.newstarts.cn

readonly PI=3.14
来源：http://mg.bookmarksfly.cn

[R04] 位置参数
来源：http://ld.shtwfgs.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://pl.huixiangedu.cn

[R05] 参数默认值
来源：http://tf.shxzskj.cn

name="${1:-default}"
来源：http://ht.lnxyls.cn

[R06] 判断命令是否存在
来源：http://wo.shxzskj.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://fk.muxihuayi.cn

[R07] if 判断文件
来源：http://lc.wgjwhj.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hd.jctech888.com.cn

[R08] 数值比较
来源：http://rq.yuexingan06.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://jc.shxzukj.cn

[R09] 字符串比较
来源：http://xb.jianghongdianzi.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://lj.yuexingan06.cn

[R10] 正则匹配
来源：http://ju.gzmigu.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ov.hahajie.cn

[R11] case 多分支
来源：http://zm.bookmarksfly.cn

case "$1" in
来源：http://vf.panjiajie.cn

start) echo "启动" ;;
来源：http://xb.gzmigu.cn

stop)  echo "停止" ;;
来源：http://yw.bookmarksfly.cn

*)     echo "未知命令" ;;
来源：http://hc.asd995.cn

esac
来源：http://fk.panjiajie.cn

[R12] for 遍历文件
来源：http://jz.panjiajie.cn

for f in *.txt; do echo "$f"; done
来源：http://mz.huanxung.cn

[R13] for 计数循环
来源：http://fr.huixiangedu.cn

for i in {1..10}; do echo "$i"; done
来源：http://vx.nicolike.cn

[R14] C 风格 for
来源：http://yq.yuntaijiaju.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://cr.colortex.cn

[R15] while 逐行读文件
来源：http://to.nicolike.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://jq.9csxet.cn

[R16] until 等待条件
来源：http://hn.asd995.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://md.muxihuayi.cn

[R17] 数组定义与取值
来源：http://cd.huanxung.cn

arr=(a b c); echo "${arr[0]}"
来源：http://xw.chemitech.net.cn

[R18] 遍历数组
来源：http://pr.muxihuayi.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://in.shxzskj.cn

[R19] 数组长度
来源：http://cg.jianghongdianzi.cn

echo "${#arr[@]}"
来源：http://ub.wgjwhj.cn

[R20] 关联数组（字典）
来源：http://mp.asd995.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mf.bookmarksfly.cn

[R21] 字符串长度
来源：http://yh.huixinmuqiang.cn

echo "${#s}"
来源：http://db.nicolike.cn

[R22] 截取子串
来源：http://ax.huixiangedu.cn

echo "${s:0:5}"
来源：http://bp.shxzskj.cn

[R23] 字符串替换
来源：http://jf.huixiangedu.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://pe.szsharing.cn

[R24] 大小写转换
来源：http://by.shxzskj.cn

echo "${s^^}"; echo "${s,,}"
来源：http://wb.shtwfgs.cn

[R25] 去后缀 / 去前缀
来源：http://dp.nszjky.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://rv.lnxyls.cn

[R26] 命令替换
来源：http://ud.muxihuayi.cn

now=$(date +%F); echo "$now"
来源：http://hk.panjiajie.cn

[R27] 算术展开
来源：http://ri.bjjhwx.cn

echo $((1 + 2 * 3))
来源：http://gs.huanxung.cn

[R28] 浮点运算
来源：http://op.haigaiapp.cn

echo "scale=2; 10/3" | bc
来源：http://ht.asd995.cn

[R29] 定义函数
来源：http://fc.newstarts.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://vt.chemitech.net.cn

[R30] 函数返回状态码
来源：http://sk.lnxyls.cn

f() { return 0; }; f || echo "失败了"
来源：http://wz.hnjuh.cn

[R31] 局部变量
来源：http://zy.jianghongdianzi.cn

f() { local x=1; echo "$x"; }
来源：http://nc.wgjwhj.cn

[R32] 参数个数校验
来源：http://zm.jctech888.com.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://th.nicolike.cn

[R33] 捕获错误并提示行号
来源：http://ir.szxytkj.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ry.haigaiapp.cn

[R34] 退出时清理
来源：http://ng.jctech888.com.cn

trap 'rm -f "$tmp"' EXIT
来源：http://fe.haigaiapp.cn

[R35] 后台执行并等待
来源：http://zr.wgjwhj.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://dt.shtwfgs.cn

[R36] 并发执行多个任务
来源：http://zm.hahajie.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://qh.haigaiapp.cn

[R37] 把输出赋给变量
来源：http://ur.wgjwhj.cn

files=$(ls -1)
来源：http://hd.muxihuayi.cn

[R38] 管道串联
来源：http://ug.521024.cn

cat a.txt | grep -i error | wc -l
来源：http://ji.huixinmuqiang.cn

[R39] 重定向标准输出与错误
来源：http://xu.panjiajie.cn

cmd > out.log 2>&1
来源：http://xf.lnxyls.cn

[R40] 追加写日志
来源：http://ur.huixiangedu.cn

echo "log" >> out.log
来源：http://uz.huixiangedu.cn

[R41] 丢弃输出
来源：http://ps.szsharing.cn

cmd >/dev/null 2>&1
来源：http://vw.nicolike.cn

[R42] 输入重定向
来源：http://ce.asd995.cn

wc -l < a.txt
来源：http://lc.shtwfgs.cn

[R43] 按名字查找文件
来源：http://sy.asd995.cn

find . -name "*.log" -type f
来源：http://qs.shtwfgs.cn

[R44] 按修改时间查找
来源：http://gc.huixinmuqiang.cn

find . -mtime -7 -type f
来源：http://fe.lnxyls.cn

[R45] 批量删除
来源：http://tv.yuexingan06.cn

find . -name "*.tmp" -delete
来源：http://ma.huanxung.cn

[R46] 递归替换文件内容
来源：http://aw.yuntaijiaju.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ml.szxytkj.cn

[R47] sed 单行替换
来源：http://is.9csxet.cn

sed -i 's/foo/bar/g' a.txt
来源：http://mg.hnjuh.cn

[R48] awk 取指定列
来源：http://go.nszjky.cn

awk '{print $1, $3}' a.txt
来源：http://pd.szxytkj.cn

[R49] awk 带条件
来源：http://bn.jctech888.com.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://zb.szsharing.cn

[R50] awk 求和
来源：http://zk.yuntaijiaju.cn

awk '{s += $2} END {print s}' a.txt
来源：http://bo.szsharing.cn

[R51] 排序去重取前几
来源：http://yx.asd995.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://ay.newstarts.cn

[R52] 统计行数
来源：http://tb.jctech888.com.cn

wc -l a.txt
来源：http://db.nszjky.cn

[R53] 查看文件头与实时尾
来源：http://qt.szsharing.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ot.gzmigu.cn

[R54] 比较两个文件
来源：http://ll.hnjuh.cn

diff a.txt b.txt
来源：http://gb.shxzukj.cn

[R55] 压缩与解压
来源：http://bo.huanxung.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://qq.szsharing.cn

[R56] 远程拷贝
来源：http://vi.bjjhwx.cn

scp file user@host:/path/
来源：http://xa.asd995.cn

[R57] 远程执行命令
来源：http://cx.jianghongdianzi.cn

ssh user@host 'uptime'
来源：http://nz.colortex.cn

[R58] 下载文件
来源：http://so.chemitech.net.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ky.muxihuayi.cn

[R59] 发 POST JSON
来源：http://xw.asd995.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://dj.huanxung.cn

[R60] 只看 HTTP 状态码
来源：http://tc.hnjuh.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://sr.wgjwhj.cn

[R61] 磁盘占用
来源：http://vq.yuexingan06.cn

df -h;  du -sh *
来源：http://uz.shxzskj.cn

[R62] 找最占空间的文件
来源：http://xf.shxzskj.cn

du -ah . | sort -rh | head -10
来源：http://yq.9csxet.cn

[R63] 内存与进程
来源：http://zm.hnjuh.cn

free -h;  ps aux | grep nginx
来源：http://vs.yuexingan06.cn

[R64] 结束进程
来源：http://ry.szxytkj.cn

kill -9 $(pgrep -f app.py)
来源：http://io.gzmigu.cn

[R65] 查看端口占用
来源：http://nr.szxytkj.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ol.shxzskj.cn

[R66] 定时任务
来源：http://fo.shtwfgs.cn

crontab -e;  crontab -l
来源：http://pr.shtwfgs.cn

[R67] 生成随机十六进制串
来源：http://fp.szxytkj.cn

openssl rand -hex 16
来源：http://kp.panjiajie.cn

[R68] 计算文件校验值
来源：http://bh.nicolike.cn

sha256sum a.txt;  md5sum a.txt
来源：http://ca.shxzskj.cn

[R69] 生成随机密码
来源：http://rq.jianghongdianzi.cn

head -c 16 /dev/urandom | base64
来源：http://tj.9csxet.cn

[R70] 时间戳与互转
来源：http://ah.shtwfgs.cn

date +%s;  date -d @1700000000
来源：http://sv.szxytkj.cn

[R71] 日期格式化
来源：http://sb.yuntaijiaju.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://ba.szxytkj.cn

[R72] 等待端口就绪
来源：http://bf.muxihuayi.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://sd.huixinmuqiang.cn

[R73] 分割大日志
来源：http://pe.yuntaijiaju.cn

split -l 1000 big.log part_
来源：http://ev.chemitech.net.cn

[R74] 批量重命名
来源：http://vs.asd995.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://bu.panjiajie.cn

[R75] 导出环境变量
来源：http://tx.panjiajie.cn

export PATH="$HOME/bin:$PATH"
来源：http://us.yuntaijiaju.cn

[R76] 使用临时文件
来源：http://kl.huanxung.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mr.jctech888.com.cn

[R77] 读取用户输入
来源：http://gd.panjiajie.cn

read -rp "请输入: " ans
来源：http://lh.lnxyls.cn

[R78] 交互式菜单
来源：http://vz.bjjhwx.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://na.muxihuayi.cn

[R79] 解析命令行选项
来源：http://om.bookmarksfly.cn


<!-- 参考信息 -->