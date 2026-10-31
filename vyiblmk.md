代发 wailian999

[Q36] 左连接
来源：http://kr.gzmigu.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://xt.gzmigu.cn

[Q37] 右连接
来源：http://av.9csxet.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://dy.yuntaijiaju.cn

[Q38] 全外连接（PostgreSQL）
来源：http://ix.yuexingan06.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://jg.yuntaijiaju.cn

[Q39] 自连接（查上下级）
来源：http://ds.jctech888.com.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://bq.wgjwhj.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://sj.hahajie.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://ma.szxytkj.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://jp.jianghongdianzi.cn

[Q41] 多表连接
来源：http://kp.szxytkj.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://va.nszjky.cn

JOIN users u ON u.id = o.user_id
来源：http://mg.nszjky.cn

JOIN products p ON p.id = o.product_id;
来源：http://dx.hahajie.cn

[Q42] 连接条件附加过滤
来源：http://js.szxytkj.cn

SELECT u.name, o.amount FROM users u
来源：http://wx.colortex.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://vt.panjiajie.cn

[Q43] 标量子查询
来源：http://pm.521024.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wo.shxzskj.cn

[Q44] IN 子查询
来源：http://ds.huixinmuqiang.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://xj.chemitech.net.cn

[Q45] EXISTS 判断存在
来源：http://fn.muxihuayi.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://qx.lnxyls.cn

[Q46] NOT EXISTS 判断不存在
来源：http://zq.hnjuh.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://cq.shxzukj.cn

[Q47] 与平均值比较
来源：http://yo.wgjwhj.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://lr.newstarts.cn

[Q48] CTE 公用表表达式
来源：http://xe.nszjky.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://rf.bjjhwx.cn

SELECT * FROM t WHERE c > 5;
来源：http://sv.bookmarksfly.cn

[Q49] 更新单行
来源：http://mo.shxzskj.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://dv.huanxung.cn

[Q50] 批量更新
来源：http://xs.haigaiapp.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://ry.yuexingan06.cn

[Q51] 用子查询更新
来源：http://jd.newstarts.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://ge.bookmarksfly.cn

[Q52] 删除指定行
来源：http://tc.huixinmuqiang.cn

DELETE FROM users WHERE id = 10;
来源：http://wt.asd995.cn

[Q53] 按条件删除
来源：http://wg.shxzukj.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://vp.yuntaijiaju.cn

[Q54] 清空表
来源：http://lt.yuntaijiaju.cn

TRUNCATE TABLE logs;
来源：http://jk.colortex.cn

[Q55] 排名（并列占位）
来源：http://ae.shxzskj.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://uj.shxzskj.cn

[Q56] 密集排名（并列不占位）
来源：http://xh.chemitech.net.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://br.nicolike.cn

[Q57] 行号
来源：http://xy.hahajie.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://rg.huixiangedu.cn

[Q58] 累计求和
来源：http://fb.nszjky.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://tg.bookmarksfly.cn

[Q59] 分组内累计
来源：http://ng.bookmarksfly.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://bu.jctech888.com.cn

[Q60] 取上一行 / 下一行
来源：http://ds.wgjwhj.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://dw.huixinmuqiang.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://vh.yuexingan06.cn

[Q61] 移动平均
来源：http://ml.yuntaijiaju.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://qn.huixiangedu.cn

[Q62] 分组占比
来源：http://iq.huixinmuqiang.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://tw.haigaiapp.cn

[Q63] 开启事务
来源：http://yy.asd995.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://la.jianghongdianzi.cn

[Q64] 提交事务
来源：http://of.asd995.cn

COMMIT;
来源：http://jk.szxytkj.cn

[Q65] 回滚事务
来源：http://aq.newstarts.cn

ROLLBACK;
来源：http://sh.newstarts.cn

[Q66] 行锁查询
来源：http://ql.hnjuh.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://za.asd995.cn

[Q67] 设置隔离级别
来源：http://nu.haigaiapp.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ki.521024.cn

[Q68] 保存点
来源：http://nd.huixinmuqiang.cn

SAVEPOINT sp1;
来源：http://ap.chemitech.net.cn

ROLLBACK TO sp1;
来源：http://dj.jianghongdianzi.cn

[Q69] 查看执行计划
来源：http://tc.jctech888.com.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://oy.wgjwhj.cn

[Q70] 更新统计信息
来源：http://ny.newstarts.cn

ANALYZE TABLE users;
来源：http://cj.panjiajie.cn

[Q71] 查看建表语句
来源：http://ao.wgjwhj.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://si.szxytkj.cn

[Q72] 查看索引
来源：http://hu.bookmarksfly.cn

SHOW INDEX FROM users;
来源：http://kw.shxzskj.cn

[Q73] 查看表状态
来源：http://ii.shxzukj.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://zd.jctech888.com.cn

[Q74] 强制使用索引
来源：http://oj.wgjwhj.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://fp.panjiajie.cn

[Q75] 日期格式化
来源：http://mq.yuntaijiaju.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ah.jianghongdianzi.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://jl.szsharing.cn

[Q76] 按天统计
来源：http://jl.shtwfgs.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://uv.huixinmuqiang.cn

[Q77] 时间加减
来源：http://fl.huixinmuqiang.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ap.hahajie.cn

[Q78] 当前时间
来源：http://su.panjiajie.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://qy.lnxyls.cn

[Q79] 字符串拼接
来源：http://dx.wgjwhj.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://gf.wgjwhj.cn

[Q80] 字符串截取
来源：http://fr.muxihuayi.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ht.szxytkj.cn

[Q81] 字符串替换
来源：http://pk.szxytkj.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://yl.huixinmuqiang.cn

[Q82] 字符长度与字节长度
来源：http://re.huanxung.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://gh.szxytkj.cn

[Q83] 大小写转换
来源：http://ng.bookmarksfly.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://gw.bookmarksfly.cn

[Q84] 去除首尾空格
来源：http://ca.521024.cn

SELECT TRIM(name) FROM users;
来源：http://tm.haigaiapp.cn

[Q85] 数值取整
来源：http://wk.nicolike.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://rj.shxzukj.cn

[Q86] 读取 JSON 字段
来源：http://ry.huixiangedu.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://jx.shtwfgs.cn

[Q87] JSON 字段做条件
来源：http://zr.haigaiapp.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ns.wgjwhj.cn

[Q88] 行转列（条件聚合）
来源：http://yu.yuexingan06.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://zv.bjjhwx.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://pr.newstarts.cn

[Q89] 判断表是否存在
来源：http://gk.bookmarksfly.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://oz.jianghongdianzi.cn

[Q90] 生成序号列
来源：http://ta.huixinmuqiang.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mq.shtwfgs.cn

================================================================================
来源：http://tc.nszjky.cn

R. Bash 专题
来源：http://uw.haigaiapp.cn

================================================================================
来源：http://mg.haigaiapp.cn

[R01] shebang 与严格模式
来源：http://rc.yuntaijiaju.cn

#!/usr/bin/env bash
来源：http://dy.shxzukj.cn

set -euo pipefail
来源：http://qa.yuntaijiaju.cn

[R02] 变量赋值与使用
来源：http://wg.bjjhwx.cn

name="Tom"; echo "$name"
来源：http://ql.chemitech.net.cn

[R03] 只读变量
来源：http://zb.wgjwhj.cn

readonly PI=3.14
来源：http://ad.huixiangedu.cn

[R04] 位置参数
来源：http://py.huixiangedu.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://sq.hnjuh.cn

[R05] 参数默认值
来源：http://rr.colortex.cn

name="${1:-default}"
来源：http://ox.shxzskj.cn

[R06] 判断命令是否存在
来源：http://rz.gzmigu.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ws.bjjhwx.cn

[R07] if 判断文件
来源：http://kf.haigaiapp.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ku.9csxet.cn

[R08] 数值比较
来源：http://ba.shxzskj.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://ks.jianghongdianzi.cn

[R09] 字符串比较
来源：http://ed.bookmarksfly.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://zo.huixiangedu.cn

[R10] 正则匹配
来源：http://hb.jianghongdianzi.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://qr.jctech888.com.cn

[R11] case 多分支
来源：http://tc.shxzskj.cn

case "$1" in
来源：http://hr.panjiajie.cn

start) echo "启动" ;;
来源：http://mc.521024.cn

stop)  echo "停止" ;;
来源：http://wc.newstarts.cn

*)     echo "未知命令" ;;
来源：http://ul.9csxet.cn

esac
来源：http://gj.bjjhwx.cn

[R12] for 遍历文件
来源：http://bs.hnjuh.cn

for f in *.txt; do echo "$f"; done
来源：http://yv.szxytkj.cn

[R13] for 计数循环
来源：http://cy.panjiajie.cn

for i in {1..10}; do echo "$i"; done
来源：http://gj.bjjhwx.cn

[R14] C 风格 for
来源：http://qn.yuexingan06.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://zq.gzmigu.cn

[R15] while 逐行读文件
来源：http://kv.asd995.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://zr.colortex.cn

[R16] until 等待条件
来源：http://dc.huanxung.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://fw.bookmarksfly.cn

[R17] 数组定义与取值
来源：http://ih.huixinmuqiang.cn

arr=(a b c); echo "${arr[0]}"
来源：http://wp.nicolike.cn

[R18] 遍历数组
来源：http://wi.hahajie.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://dn.nicolike.cn

[R19] 数组长度
来源：http://hd.chemitech.net.cn

echo "${#arr[@]}"
来源：http://rs.shxzskj.cn

[R20] 关联数组（字典）
来源：http://ni.jianghongdianzi.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://tf.shxzskj.cn

[R21] 字符串长度
来源：http://sp.huanxung.cn

echo "${#s}"
来源：http://zk.haigaiapp.cn

[R22] 截取子串
来源：http://vw.lnxyls.cn

echo "${s:0:5}"
来源：http://kd.muxihuayi.cn

[R23] 字符串替换
来源：http://lv.huixiangedu.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://rc.jianghongdianzi.cn

[R24] 大小写转换
来源：http://pb.muxihuayi.cn

echo "${s^^}"; echo "${s,,}"
来源：http://lo.yuexingan06.cn

[R25] 去后缀 / 去前缀
来源：http://nz.521024.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://qc.huixinmuqiang.cn

[R26] 命令替换
来源：http://jo.panjiajie.cn

now=$(date +%F); echo "$now"
来源：http://ex.nszjky.cn

[R27] 算术展开
来源：http://hi.yuexingan06.cn

echo $((1 + 2 * 3))
来源：http://os.huixiangedu.cn

[R28] 浮点运算
来源：http://ht.521024.cn

echo "scale=2; 10/3" | bc
来源：http://qg.shxzukj.cn

[R29] 定义函数
来源：http://ds.shxzukj.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ca.yuexingan06.cn

[R30] 函数返回状态码
来源：http://vl.newstarts.cn

f() { return 0; }; f || echo "失败了"
来源：http://sl.wgjwhj.cn

[R31] 局部变量
来源：http://la.521024.cn

f() { local x=1; echo "$x"; }
来源：http://sx.yuntaijiaju.cn

[R32] 参数个数校验
来源：http://ln.szsharing.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://vt.9csxet.cn

[R33] 捕获错误并提示行号
来源：http://zn.nszjky.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://kr.muxihuayi.cn

[R34] 退出时清理
来源：http://km.hnjuh.cn

trap 'rm -f "$tmp"' EXIT
来源：http://ii.9csxet.cn

[R35] 后台执行并等待
来源：http://el.521024.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://qc.9csxet.cn

[R36] 并发执行多个任务
来源：http://pi.huixinmuqiang.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://id.panjiajie.cn

[R37] 把输出赋给变量
来源：http://wp.haigaiapp.cn

files=$(ls -1)
来源：http://yx.szsharing.cn

[R38] 管道串联
来源：http://id.panjiajie.cn

cat a.txt | grep -i error | wc -l
来源：http://eg.lnxyls.cn

[R39] 重定向标准输出与错误
来源：http://zn.lnxyls.cn

cmd > out.log 2>&1
来源：http://tb.gzmigu.cn

[R40] 追加写日志
来源：http://gt.huanxung.cn

echo "log" >> out.log
来源：http://xo.asd995.cn

[R41] 丢弃输出
来源：http://ui.colortex.cn

cmd >/dev/null 2>&1
来源：http://kd.newstarts.cn

[R42] 输入重定向
来源：http://al.jctech888.com.cn

wc -l < a.txt
来源：http://yy.shtwfgs.cn

[R43] 按名字查找文件
来源：http://mc.muxihuayi.cn

find . -name "*.log" -type f
来源：http://di.shxzskj.cn

[R44] 按修改时间查找
来源：http://qt.nicolike.cn

find . -mtime -7 -type f
来源：http://fe.chemitech.net.cn

[R45] 批量删除
来源：http://kx.yuexingan06.cn

find . -name "*.tmp" -delete
来源：http://rq.panjiajie.cn

[R46] 递归替换文件内容
来源：http://hc.jianghongdianzi.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://he.shxzskj.cn

[R47] sed 单行替换
来源：http://xt.nicolike.cn

sed -i 's/foo/bar/g' a.txt
来源：http://yf.jianghongdianzi.cn

[R48] awk 取指定列
来源：http://sr.huixinmuqiang.cn

awk '{print $1, $3}' a.txt
来源：http://ec.bookmarksfly.cn

[R49] awk 带条件
来源：http://xu.haigaiapp.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://fd.asd995.cn

[R50] awk 求和
来源：http://fs.panjiajie.cn

awk '{s += $2} END {print s}' a.txt
来源：http://jr.chemitech.net.cn

[R51] 排序去重取前几
来源：http://dq.hnjuh.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://pi.bookmarksfly.cn

[R52] 统计行数
来源：http://la.shtwfgs.cn

wc -l a.txt
来源：http://tc.yuntaijiaju.cn

[R53] 查看文件头与实时尾
来源：http://hm.wgjwhj.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://qj.521024.cn

[R54] 比较两个文件
来源：http://ur.shxzukj.cn

diff a.txt b.txt
来源：http://ey.asd995.cn

[R55] 压缩与解压
来源：http://jh.bjjhwx.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://cb.521024.cn

[R56] 远程拷贝
来源：http://qh.nszjky.cn

scp file user@host:/path/
来源：http://hx.yuntaijiaju.cn

[R57] 远程执行命令
来源：http://yk.muxihuayi.cn

ssh user@host 'uptime'
来源：http://wi.shtwfgs.cn

[R58] 下载文件
来源：http://ui.jianghongdianzi.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://he.hahajie.cn

[R59] 发 POST JSON
来源：http://iv.colortex.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ni.wgjwhj.cn

[R60] 只看 HTTP 状态码
来源：http://vt.szxytkj.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://za.chemitech.net.cn

[R61] 磁盘占用
来源：http://nd.jctech888.com.cn

df -h;  du -sh *
来源：http://lt.hahajie.cn

[R62] 找最占空间的文件
来源：http://bu.colortex.cn

du -ah . | sort -rh | head -10
来源：http://gb.huanxung.cn

[R63] 内存与进程
来源：http://xb.szsharing.cn

free -h;  ps aux | grep nginx
来源：http://zk.wgjwhj.cn

[R64] 结束进程
来源：http://xn.jctech888.com.cn

kill -9 $(pgrep -f app.py)
来源：http://ka.yuexingan06.cn

[R65] 查看端口占用
来源：http://uk.bookmarksfly.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ch.panjiajie.cn

[R66] 定时任务
来源：http://ej.9csxet.cn

crontab -e;  crontab -l
来源：http://yz.wgjwhj.cn

[R67] 生成随机十六进制串
来源：http://dw.nszjky.cn

openssl rand -hex 16
来源：http://du.haigaiapp.cn

[R68] 计算文件校验值
来源：http://ja.asd995.cn

sha256sum a.txt;  md5sum a.txt
来源：http://al.yuexingan06.cn

[R69] 生成随机密码
来源：http://dv.jianghongdianzi.cn

head -c 16 /dev/urandom | base64
来源：http://ni.shtwfgs.cn

[R70] 时间戳与互转
来源：http://kh.chemitech.net.cn

date +%s;  date -d @1700000000
来源：http://yl.shxzskj.cn

[R71] 日期格式化
来源：http://dc.newstarts.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://ge.9csxet.cn

[R72] 等待端口就绪
来源：http://rf.huixinmuqiang.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://ku.yuntaijiaju.cn

[R73] 分割大日志
来源：http://ne.lnxyls.cn

split -l 1000 big.log part_
来源：http://ov.521024.cn

[R74] 批量重命名
来源：http://ma.jctech888.com.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://iv.9csxet.cn

[R75] 导出环境变量
来源：http://eo.shxzskj.cn

export PATH="$HOME/bin:$PATH"
来源：http://lg.shxzukj.cn

[R76] 使用临时文件
来源：http://xh.chemitech.net.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://qf.huixiangedu.cn

[R77] 读取用户输入
来源：http://ou.shtwfgs.cn

read -rp "请输入: " ans
来源：http://fk.yuexingan06.cn

[R78] 交互式菜单
来源：http://lz.hnjuh.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://yb.yuntaijiaju.cn

[R79] 解析命令行选项
来源：http://lu.haigaiapp.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ad.jctech888.com.cn

[R80] 查看脚本执行耗时
来源：http://xn.newstarts.cn

time ./run.sh
来源：http://qt.szxytkj.cn

================================================================================
来源：http://zw.szxytkj.cn

S. C / C++ 专题
来源：http://if.szxytkj.cn

================================================================================
来源：http://bs.yuntaijiaju.cn

[S01] C：Hello World
来源：http://mo.jctech888.com.cn

#include <stdio.h>
来源：http://uh.521024.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://oe.yuntaijiaju.cn

[S02] C：变量与格式化输出
来源：http://jm.nszjky.cn

int a = 10; printf("%d\n", a);
来源：http://xp.szsharing.cn

[S03] C：读入整数
来源：http://vo.shxzskj.cn

int x; scanf("%d", &x);
来源：http://qq.shxzskj.cn

[S04] C：字符串复制
来源：http://cv.huanxung.cn

char dst[32]; strcpy(dst, "hi");
来源：http://th.nicolike.cn

[S05] C：字符串长度
来源：http://lf.gzmigu.cn


<!-- 参考信息 -->