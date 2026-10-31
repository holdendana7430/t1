代发 wailian999

SELECT MAX(age), MIN(age) FROM users;
来源：http://te.huixiangedu.cn

[Q30] 分组统计
来源：http://oj.panjiajie.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://uu.wgjwhj.cn

[Q31] 分组后过滤
来源：http://gm.chemitech.net.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ws.asd995.cn

[Q32] 分组拼接字符串
来源：http://wc.bookmarksfly.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://tu.bjjhwx.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hi.shxzukj.cn

[Q33] 多列分组
来源：http://fg.shxzukj.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://cj.huixiangedu.cn

[Q34] 每组取第一条
来源：http://zb.9csxet.cn

SELECT * FROM (
来源：http://dn.yuexingan06.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://lz.shxzskj.cn

) t WHERE rn = 1;
来源：http://ub.huanxung.cn

[Q35] 内连接
来源：http://af.9csxet.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://uy.hahajie.cn

[Q36] 左连接
来源：http://wo.huixinmuqiang.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://in.yuntaijiaju.cn

[Q37] 右连接
来源：http://yz.shxzukj.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ql.huixiangedu.cn

[Q38] 全外连接（PostgreSQL）
来源：http://vi.jctech888.com.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://gk.shtwfgs.cn

[Q39] 自连接（查上下级）
来源：http://ti.huanxung.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://kp.colortex.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://bq.yuexingan06.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://wz.yuntaijiaju.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mk.szsharing.cn

[Q41] 多表连接
来源：http://vp.yuexingan06.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://ci.asd995.cn

JOIN users u ON u.id = o.user_id
来源：http://ld.huixiangedu.cn

JOIN products p ON p.id = o.product_id;
来源：http://qz.huixinmuqiang.cn

[Q42] 连接条件附加过滤
来源：http://yb.lnxyls.cn

SELECT u.name, o.amount FROM users u
来源：http://bh.gzmigu.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://dr.nszjky.cn

[Q43] 标量子查询
来源：http://xv.panjiajie.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://dh.chemitech.net.cn

[Q44] IN 子查询
来源：http://sk.huanxung.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ym.bjjhwx.cn

[Q45] EXISTS 判断存在
来源：http://ui.shxzskj.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hc.huixinmuqiang.cn

[Q46] NOT EXISTS 判断不存在
来源：http://xy.newstarts.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://jh.asd995.cn

[Q47] 与平均值比较
来源：http://if.gzmigu.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://eg.huixinmuqiang.cn

[Q48] CTE 公用表表达式
来源：http://cr.bookmarksfly.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://df.szsharing.cn

SELECT * FROM t WHERE c > 5;
来源：http://ho.chemitech.net.cn

[Q49] 更新单行
来源：http://en.huixinmuqiang.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://zc.jctech888.com.cn

[Q50] 批量更新
来源：http://vd.huanxung.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://no.yuntaijiaju.cn

[Q51] 用子查询更新
来源：http://xq.gzmigu.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://fs.lnxyls.cn

[Q52] 删除指定行
来源：http://ok.hahajie.cn

DELETE FROM users WHERE id = 10;
来源：http://mz.newstarts.cn

[Q53] 按条件删除
来源：http://gc.haigaiapp.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://qj.9csxet.cn

[Q54] 清空表
来源：http://wx.panjiajie.cn

TRUNCATE TABLE logs;
来源：http://ic.newstarts.cn

[Q55] 排名（并列占位）
来源：http://en.gzmigu.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://dz.asd995.cn

[Q56] 密集排名（并列不占位）
来源：http://bm.huixiangedu.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://cu.chemitech.net.cn

[Q57] 行号
来源：http://ry.asd995.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://sx.huixiangedu.cn

[Q58] 累计求和
来源：http://io.lnxyls.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hh.haigaiapp.cn

[Q59] 分组内累计
来源：http://pu.bjjhwx.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://yn.szsharing.cn

[Q60] 取上一行 / 下一行
来源：http://rr.huixiangedu.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://dg.huanxung.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://rt.haigaiapp.cn

[Q61] 移动平均
来源：http://sg.szxytkj.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ce.nszjky.cn

[Q62] 分组占比
来源：http://os.shxzukj.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://zu.gzmigu.cn

[Q63] 开启事务
来源：http://if.yuexingan06.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://sm.yuntaijiaju.cn

[Q64] 提交事务
来源：http://ku.newstarts.cn

COMMIT;
来源：http://sm.521024.cn

[Q65] 回滚事务
来源：http://iy.gzmigu.cn

ROLLBACK;
来源：http://vs.huanxung.cn

[Q66] 行锁查询
来源：http://wg.hnjuh.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://dn.nszjky.cn

[Q67] 设置隔离级别
来源：http://jd.hnjuh.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ly.shtwfgs.cn

[Q68] 保存点
来源：http://kn.newstarts.cn

SAVEPOINT sp1;
来源：http://rq.shtwfgs.cn

ROLLBACK TO sp1;
来源：http://sk.bookmarksfly.cn

[Q69] 查看执行计划
来源：http://yf.jctech888.com.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://im.panjiajie.cn

[Q70] 更新统计信息
来源：http://lf.colortex.cn

ANALYZE TABLE users;
来源：http://ir.szsharing.cn

[Q71] 查看建表语句
来源：http://bp.panjiajie.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://zj.huanxung.cn

[Q72] 查看索引
来源：http://un.shxzukj.cn

SHOW INDEX FROM users;
来源：http://bb.bookmarksfly.cn

[Q73] 查看表状态
来源：http://ck.hnjuh.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://gu.huanxung.cn

[Q74] 强制使用索引
来源：http://td.jctech888.com.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://co.shtwfgs.cn

[Q75] 日期格式化
来源：http://fw.jianghongdianzi.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://gf.asd995.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hp.szxytkj.cn

[Q76] 按天统计
来源：http://oj.wgjwhj.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://qq.szxytkj.cn

[Q77] 时间加减
来源：http://pt.shtwfgs.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ua.huixinmuqiang.cn

[Q78] 当前时间
来源：http://op.shxzukj.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wf.huixiangedu.cn

[Q79] 字符串拼接
来源：http://pk.9csxet.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://oa.shxzukj.cn

[Q80] 字符串截取
来源：http://ud.nszjky.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://de.lnxyls.cn

[Q81] 字符串替换
来源：http://jp.huixinmuqiang.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://kx.colortex.cn

[Q82] 字符长度与字节长度
来源：http://kg.newstarts.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://vu.szsharing.cn

[Q83] 大小写转换
来源：http://hp.huixinmuqiang.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://co.shxzskj.cn

[Q84] 去除首尾空格
来源：http://zz.newstarts.cn

SELECT TRIM(name) FROM users;
来源：http://by.wgjwhj.cn

[Q85] 数值取整
来源：http://xx.jctech888.com.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ay.nszjky.cn

[Q86] 读取 JSON 字段
来源：http://uy.gzmigu.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://nf.muxihuayi.cn

[Q87] JSON 字段做条件
来源：http://oi.muxihuayi.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ur.lnxyls.cn

[Q88] 行转列（条件聚合）
来源：http://yb.yuexingan06.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://jp.shxzukj.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://cr.bookmarksfly.cn

[Q89] 判断表是否存在
来源：http://ph.gzmigu.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://gi.haigaiapp.cn

[Q90] 生成序号列
来源：http://vo.szxytkj.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://kp.colortex.cn

================================================================================
来源：http://st.huixinmuqiang.cn

R. Bash 专题
来源：http://zb.bjjhwx.cn

================================================================================
来源：http://jg.hahajie.cn

[R01] shebang 与严格模式
来源：http://qv.muxihuayi.cn

#!/usr/bin/env bash
来源：http://dn.szxytkj.cn

set -euo pipefail
来源：http://lj.bjjhwx.cn

[R02] 变量赋值与使用
来源：http://vx.haigaiapp.cn

name="Tom"; echo "$name"
来源：http://vj.jctech888.com.cn

[R03] 只读变量
来源：http://dr.chemitech.net.cn

readonly PI=3.14
来源：http://jx.lnxyls.cn

[R04] 位置参数
来源：http://pe.newstarts.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ca.chemitech.net.cn

[R05] 参数默认值
来源：http://ty.bookmarksfly.cn

name="${1:-default}"
来源：http://lz.huixinmuqiang.cn

[R06] 判断命令是否存在
来源：http://qd.szsharing.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://os.huixiangedu.cn

[R07] if 判断文件
来源：http://xv.521024.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://tn.chemitech.net.cn

[R08] 数值比较
来源：http://ub.chemitech.net.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://ii.huanxung.cn

[R09] 字符串比较
来源：http://fp.yuntaijiaju.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://cu.shxzskj.cn

[R10] 正则匹配
来源：http://qb.9csxet.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://pb.huixiangedu.cn

[R11] case 多分支
来源：http://xm.hahajie.cn

case "$1" in
来源：http://xg.muxihuayi.cn

start) echo "启动" ;;
来源：http://ei.jianghongdianzi.cn

stop)  echo "停止" ;;
来源：http://wc.haigaiapp.cn

*)     echo "未知命令" ;;
来源：http://sw.lnxyls.cn

esac
来源：http://kd.shxzukj.cn

[R12] for 遍历文件
来源：http://sm.bjjhwx.cn

for f in *.txt; do echo "$f"; done
来源：http://pw.shxzskj.cn

[R13] for 计数循环
来源：http://ig.jctech888.com.cn

for i in {1..10}; do echo "$i"; done
来源：http://lm.bookmarksfly.cn

[R14] C 风格 for
来源：http://qp.szxytkj.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://gk.huixiangedu.cn

[R15] while 逐行读文件
来源：http://jp.nszjky.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://dh.bjjhwx.cn

[R16] until 等待条件
来源：http://mp.gzmigu.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://my.szsharing.cn

[R17] 数组定义与取值
来源：http://oy.asd995.cn

arr=(a b c); echo "${arr[0]}"
来源：http://rh.nicolike.cn

[R18] 遍历数组
来源：http://wy.nszjky.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ky.bjjhwx.cn

[R19] 数组长度
来源：http://wo.hahajie.cn

echo "${#arr[@]}"
来源：http://dc.asd995.cn

[R20] 关联数组（字典）
来源：http://og.521024.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ed.bookmarksfly.cn

[R21] 字符串长度
来源：http://cm.bookmarksfly.cn

echo "${#s}"
来源：http://jx.huixinmuqiang.cn

[R22] 截取子串
来源：http://ge.hahajie.cn

echo "${s:0:5}"
来源：http://qz.yuexingan06.cn

[R23] 字符串替换
来源：http://jg.nicolike.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://tu.asd995.cn

[R24] 大小写转换
来源：http://or.yuexingan06.cn

echo "${s^^}"; echo "${s,,}"
来源：http://je.bookmarksfly.cn

[R25] 去后缀 / 去前缀
来源：http://cj.shxzskj.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://ie.huanxung.cn

[R26] 命令替换
来源：http://mh.hnjuh.cn

now=$(date +%F); echo "$now"
来源：http://ua.haigaiapp.cn

[R27] 算术展开
来源：http://dm.jctech888.com.cn

echo $((1 + 2 * 3))
来源：http://qh.chemitech.net.cn

[R28] 浮点运算
来源：http://nq.chemitech.net.cn

echo "scale=2; 10/3" | bc
来源：http://qa.chemitech.net.cn

[R29] 定义函数
来源：http://nh.bookmarksfly.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://bq.panjiajie.cn

[R30] 函数返回状态码
来源：http://dn.shxzukj.cn

f() { return 0; }; f || echo "失败了"
来源：http://in.jctech888.com.cn

[R31] 局部变量
来源：http://tf.muxihuayi.cn

f() { local x=1; echo "$x"; }
来源：http://iu.shxzskj.cn

[R32] 参数个数校验
来源：http://xk.newstarts.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://sy.haigaiapp.cn

[R33] 捕获错误并提示行号
来源：http://mq.yuntaijiaju.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://oi.jctech888.com.cn

[R34] 退出时清理
来源：http://df.wgjwhj.cn

trap 'rm -f "$tmp"' EXIT
来源：http://cq.jctech888.com.cn

[R35] 后台执行并等待
来源：http://na.huixinmuqiang.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://ce.shxzukj.cn

[R36] 并发执行多个任务
来源：http://dn.521024.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ff.bookmarksfly.cn

[R37] 把输出赋给变量
来源：http://fe.shxzskj.cn

files=$(ls -1)
来源：http://qg.huixinmuqiang.cn

[R38] 管道串联
来源：http://kd.hahajie.cn

cat a.txt | grep -i error | wc -l
来源：http://qv.jctech888.com.cn

[R39] 重定向标准输出与错误
来源：http://bp.huanxung.cn

cmd > out.log 2>&1
来源：http://ks.lnxyls.cn

[R40] 追加写日志
来源：http://gm.hnjuh.cn

echo "log" >> out.log
来源：http://fj.asd995.cn

[R41] 丢弃输出
来源：http://lg.panjiajie.cn

cmd >/dev/null 2>&1
来源：http://qg.yuntaijiaju.cn

[R42] 输入重定向
来源：http://aw.newstarts.cn

wc -l < a.txt
来源：http://mc.gzmigu.cn

[R43] 按名字查找文件
来源：http://vy.jctech888.com.cn

find . -name "*.log" -type f
来源：http://bw.9csxet.cn

[R44] 按修改时间查找
来源：http://pf.huanxung.cn

find . -mtime -7 -type f
来源：http://ka.hahajie.cn

[R45] 批量删除
来源：http://ev.shxzukj.cn

find . -name "*.tmp" -delete
来源：http://zy.newstarts.cn

[R46] 递归替换文件内容
来源：http://ug.haigaiapp.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://bp.muxihuayi.cn

[R47] sed 单行替换
来源：http://sk.bookmarksfly.cn

sed -i 's/foo/bar/g' a.txt
来源：http://wg.chemitech.net.cn

[R48] awk 取指定列
来源：http://pu.521024.cn

awk '{print $1, $3}' a.txt
来源：http://cu.hahajie.cn

[R49] awk 带条件
来源：http://ab.9csxet.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://vh.asd995.cn

[R50] awk 求和
来源：http://br.nicolike.cn

awk '{s += $2} END {print s}' a.txt
来源：http://fd.bookmarksfly.cn

[R51] 排序去重取前几
来源：http://qb.panjiajie.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://bw.521024.cn

[R52] 统计行数
来源：http://yq.shtwfgs.cn

wc -l a.txt
来源：http://jo.yuexingan06.cn

[R53] 查看文件头与实时尾
来源：http://li.nszjky.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://eo.521024.cn

[R54] 比较两个文件
来源：http://eu.szsharing.cn

diff a.txt b.txt
来源：http://ei.nicolike.cn

[R55] 压缩与解压
来源：http://ml.huixiangedu.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ip.nszjky.cn

[R56] 远程拷贝
来源：http://ya.panjiajie.cn

scp file user@host:/path/
来源：http://to.colortex.cn

[R57] 远程执行命令
来源：http://bj.shxzskj.cn

ssh user@host 'uptime'
来源：http://vl.jianghongdianzi.cn

[R58] 下载文件
来源：http://ms.wgjwhj.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mg.szsharing.cn

[R59] 发 POST JSON
来源：http://gm.yuntaijiaju.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://fg.shtwfgs.cn

[R60] 只看 HTTP 状态码
来源：http://ee.muxihuayi.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://nc.yuntaijiaju.cn

[R61] 磁盘占用
来源：http://ig.nicolike.cn

df -h;  du -sh *
来源：http://ww.jianghongdianzi.cn

[R62] 找最占空间的文件
来源：http://xo.hnjuh.cn

du -ah . | sort -rh | head -10
来源：http://bq.huixinmuqiang.cn

[R63] 内存与进程
来源：http://ha.asd995.cn

free -h;  ps aux | grep nginx
来源：http://mh.nicolike.cn

[R64] 结束进程
来源：http://az.newstarts.cn

kill -9 $(pgrep -f app.py)
来源：http://sh.gzmigu.cn

[R65] 查看端口占用
来源：http://um.9csxet.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://vg.szxytkj.cn

[R66] 定时任务
来源：http://ra.huixiangedu.cn

crontab -e;  crontab -l
来源：http://uz.yuexingan06.cn

[R67] 生成随机十六进制串
来源：http://wk.panjiajie.cn

openssl rand -hex 16
来源：http://fe.bookmarksfly.cn

[R68] 计算文件校验值
来源：http://ca.newstarts.cn

sha256sum a.txt;  md5sum a.txt
来源：http://bq.wgjwhj.cn

[R69] 生成随机密码
来源：http://xf.panjiajie.cn

head -c 16 /dev/urandom | base64
来源：http://lx.521024.cn

[R70] 时间戳与互转
来源：http://fh.lnxyls.cn

date +%s;  date -d @1700000000
来源：http://mo.9csxet.cn

[R71] 日期格式化
来源：http://dn.haigaiapp.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://rg.newstarts.cn

[R72] 等待端口就绪
来源：http://eh.huixiangedu.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://ec.huixinmuqiang.cn

[R73] 分割大日志
来源：http://kz.newstarts.cn

split -l 1000 big.log part_
来源：http://tk.colortex.cn

[R74] 批量重命名
来源：http://pk.szxytkj.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://vc.colortex.cn

[R75] 导出环境变量
来源：http://fh.panjiajie.cn

export PATH="$HOME/bin:$PATH"
来源：http://ae.wgjwhj.cn

[R76] 使用临时文件
来源：http://ce.colortex.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ip.wgjwhj.cn

[R77] 读取用户输入
来源：http://nk.jianghongdianzi.cn

read -rp "请输入: " ans
来源：http://ym.jianghongdianzi.cn

[R78] 交互式菜单
来源：http://mu.szxytkj.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://zl.chemitech.net.cn

[R79] 解析命令行选项
来源：http://dx.shxzskj.cn


<!-- 参考信息 -->