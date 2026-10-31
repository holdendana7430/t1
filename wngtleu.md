代发 wailian999

[Q36] 左连接
来源：http://fh.newstarts.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://vh.szsharing.cn

[Q37] 右连接
来源：http://gq.bookmarksfly.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://cx.bookmarksfly.cn

[Q38] 全外连接（PostgreSQL）
来源：http://sl.huixinmuqiang.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://kn.lnxyls.cn

[Q39] 自连接（查上下级）
来源：http://lo.huixiangedu.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://ew.yuexingan06.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ui.nszjky.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://zo.9csxet.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://yb.szxytkj.cn

[Q41] 多表连接
来源：http://qe.yuexingan06.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://in.jctech888.com.cn

JOIN users u ON u.id = o.user_id
来源：http://lz.asd995.cn

JOIN products p ON p.id = o.product_id;
来源：http://an.shtwfgs.cn

[Q42] 连接条件附加过滤
来源：http://rm.lnxyls.cn

SELECT u.name, o.amount FROM users u
来源：http://iw.nicolike.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://il.muxihuayi.cn

[Q43] 标量子查询
来源：http://km.bjjhwx.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://zv.yuexingan06.cn

[Q44] IN 子查询
来源：http://dh.newstarts.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://xc.jianghongdianzi.cn

[Q45] EXISTS 判断存在
来源：http://xm.yuntaijiaju.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mp.chemitech.net.cn

[Q46] NOT EXISTS 判断不存在
来源：http://oa.yuntaijiaju.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://dh.bookmarksfly.cn

[Q47] 与平均值比较
来源：http://md.bjjhwx.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://je.shtwfgs.cn

[Q48] CTE 公用表表达式
来源：http://jb.9csxet.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://kl.huixiangedu.cn

SELECT * FROM t WHERE c > 5;
来源：http://nv.shxzskj.cn

[Q49] 更新单行
来源：http://ba.nicolike.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://cv.huixinmuqiang.cn

[Q50] 批量更新
来源：http://yl.shxzukj.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://xb.jctech888.com.cn

[Q51] 用子查询更新
来源：http://so.shxzukj.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://jt.huixiangedu.cn

[Q52] 删除指定行
来源：http://ul.huixinmuqiang.cn

DELETE FROM users WHERE id = 10;
来源：http://it.asd995.cn

[Q53] 按条件删除
来源：http://gu.jianghongdianzi.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://vp.shxzskj.cn

[Q54] 清空表
来源：http://hc.asd995.cn

TRUNCATE TABLE logs;
来源：http://ds.jianghongdianzi.cn

[Q55] 排名（并列占位）
来源：http://hp.hahajie.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://pg.9csxet.cn

[Q56] 密集排名（并列不占位）
来源：http://oc.9csxet.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://gk.hnjuh.cn

[Q57] 行号
来源：http://tg.nszjky.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://na.hnjuh.cn

[Q58] 累计求和
来源：http://ii.yuexingan06.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://re.nszjky.cn

[Q59] 分组内累计
来源：http://wj.shxzukj.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ss.shxzukj.cn

[Q60] 取上一行 / 下一行
来源：http://lc.colortex.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://dl.9csxet.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://uq.jctech888.com.cn

[Q61] 移动平均
来源：http://rp.shxzskj.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wk.nicolike.cn

[Q62] 分组占比
来源：http://ja.jctech888.com.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mp.nszjky.cn

[Q63] 开启事务
来源：http://hu.huixinmuqiang.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://xb.nicolike.cn

[Q64] 提交事务
来源：http://zt.haigaiapp.cn

COMMIT;
来源：http://dh.yuntaijiaju.cn

[Q65] 回滚事务
来源：http://qc.hnjuh.cn

ROLLBACK;
来源：http://mj.haigaiapp.cn

[Q66] 行锁查询
来源：http://yy.shxzukj.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://nf.wgjwhj.cn

[Q67] 设置隔离级别
来源：http://wr.jianghongdianzi.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://cr.bjjhwx.cn

[Q68] 保存点
来源：http://bb.colortex.cn

SAVEPOINT sp1;
来源：http://ar.newstarts.cn

ROLLBACK TO sp1;
来源：http://zt.chemitech.net.cn

[Q69] 查看执行计划
来源：http://ko.colortex.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://qc.shxzukj.cn

[Q70] 更新统计信息
来源：http://eg.bookmarksfly.cn

ANALYZE TABLE users;
来源：http://ov.hahajie.cn

[Q71] 查看建表语句
来源：http://vf.bjjhwx.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://fd.hnjuh.cn

[Q72] 查看索引
来源：http://vx.bookmarksfly.cn

SHOW INDEX FROM users;
来源：http://hg.chemitech.net.cn

[Q73] 查看表状态
来源：http://cu.lnxyls.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://sh.nszjky.cn

[Q74] 强制使用索引
来源：http://xq.jianghongdianzi.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://yd.huixinmuqiang.cn

[Q75] 日期格式化
来源：http://vk.shxzskj.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://me.shtwfgs.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://te.521024.cn

[Q76] 按天统计
来源：http://jz.yuntaijiaju.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://dr.szsharing.cn

[Q77] 时间加减
来源：http://zh.lnxyls.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hb.szsharing.cn

[Q78] 当前时间
来源：http://pl.shxzskj.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ma.huanxung.cn

[Q79] 字符串拼接
来源：http://jk.yuexingan06.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://nk.bjjhwx.cn

[Q80] 字符串截取
来源：http://ia.9csxet.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://pd.panjiajie.cn

[Q81] 字符串替换
来源：http://po.9csxet.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ik.panjiajie.cn

[Q82] 字符长度与字节长度
来源：http://xl.nszjky.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://tp.nszjky.cn

[Q83] 大小写转换
来源：http://np.shxzskj.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://bu.shxzskj.cn

[Q84] 去除首尾空格
来源：http://yj.shxzukj.cn

SELECT TRIM(name) FROM users;
来源：http://wp.hahajie.cn

[Q85] 数值取整
来源：http://zy.muxihuayi.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://yr.szsharing.cn

[Q86] 读取 JSON 字段
来源：http://hv.szsharing.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ev.lnxyls.cn

[Q87] JSON 字段做条件
来源：http://el.lnxyls.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ce.521024.cn

[Q88] 行转列（条件聚合）
来源：http://wk.wgjwhj.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://xd.nicolike.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wv.huixinmuqiang.cn

[Q89] 判断表是否存在
来源：http://nt.521024.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://cc.huanxung.cn

[Q90] 生成序号列
来源：http://eh.nszjky.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mn.szsharing.cn

================================================================================
来源：http://xi.wgjwhj.cn

R. Bash 专题
来源：http://zp.shxzskj.cn

================================================================================
来源：http://df.gzmigu.cn

[R01] shebang 与严格模式
来源：http://rx.hnjuh.cn

#!/usr/bin/env bash
来源：http://zg.bjjhwx.cn

set -euo pipefail
来源：http://fs.haigaiapp.cn

[R02] 变量赋值与使用
来源：http://le.huixinmuqiang.cn

name="Tom"; echo "$name"
来源：http://it.nszjky.cn

[R03] 只读变量
来源：http://tf.shtwfgs.cn

readonly PI=3.14
来源：http://xd.hahajie.cn

[R04] 位置参数
来源：http://yw.huixinmuqiang.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://sh.colortex.cn

[R05] 参数默认值
来源：http://ik.nicolike.cn

name="${1:-default}"
来源：http://xf.bjjhwx.cn

[R06] 判断命令是否存在
来源：http://jx.shxzukj.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://vd.hahajie.cn

[R07] if 判断文件
来源：http://bu.szsharing.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://du.shxzukj.cn

[R08] 数值比较
来源：http://il.yuexingan06.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://eu.huixinmuqiang.cn

[R09] 字符串比较
来源：http://uq.shxzskj.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://zj.chemitech.net.cn

[R10] 正则匹配
来源：http://yt.chemitech.net.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://gx.yuexingan06.cn

[R11] case 多分支
来源：http://of.yuexingan06.cn

case "$1" in
来源：http://yx.shxzukj.cn

start) echo "启动" ;;
来源：http://gn.huixiangedu.cn

stop)  echo "停止" ;;
来源：http://sx.panjiajie.cn

*)     echo "未知命令" ;;
来源：http://np.bjjhwx.cn

esac
来源：http://cc.muxihuayi.cn

[R12] for 遍历文件
来源：http://cq.wgjwhj.cn

for f in *.txt; do echo "$f"; done
来源：http://wj.hahajie.cn

[R13] for 计数循环
来源：http://eh.chemitech.net.cn

for i in {1..10}; do echo "$i"; done
来源：http://kv.haigaiapp.cn

[R14] C 风格 for
来源：http://yr.huixinmuqiang.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://zd.newstarts.cn

[R15] while 逐行读文件
来源：http://sx.lnxyls.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://bd.chemitech.net.cn

[R16] until 等待条件
来源：http://jo.yuexingan06.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://rq.nszjky.cn

[R17] 数组定义与取值
来源：http://fo.huanxung.cn

arr=(a b c); echo "${arr[0]}"
来源：http://ud.gzmigu.cn

[R18] 遍历数组
来源：http://sr.chemitech.net.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://xa.nszjky.cn

[R19] 数组长度
来源：http://vh.huixiangedu.cn

echo "${#arr[@]}"
来源：http://vr.nicolike.cn

[R20] 关联数组（字典）
来源：http://cg.szsharing.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://fy.jianghongdianzi.cn

[R21] 字符串长度
来源：http://et.9csxet.cn

echo "${#s}"
来源：http://ix.jctech888.com.cn

[R22] 截取子串
来源：http://et.yuexingan06.cn

echo "${s:0:5}"
来源：http://cu.colortex.cn

[R23] 字符串替换
来源：http://gq.lnxyls.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://yc.bjjhwx.cn

[R24] 大小写转换
来源：http://nj.bookmarksfly.cn

echo "${s^^}"; echo "${s,,}"
来源：http://ou.lnxyls.cn

[R25] 去后缀 / 去前缀
来源：http://iz.szsharing.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://xw.yuntaijiaju.cn

[R26] 命令替换
来源：http://rk.521024.cn

now=$(date +%F); echo "$now"
来源：http://ra.gzmigu.cn

[R27] 算术展开
来源：http://zt.hnjuh.cn

echo $((1 + 2 * 3))
来源：http://bq.nicolike.cn

[R28] 浮点运算
来源：http://xk.yuntaijiaju.cn

echo "scale=2; 10/3" | bc
来源：http://ce.muxihuayi.cn

[R29] 定义函数
来源：http://ai.hnjuh.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://kr.asd995.cn

[R30] 函数返回状态码
来源：http://at.shtwfgs.cn

f() { return 0; }; f || echo "失败了"
来源：http://du.bookmarksfly.cn

[R31] 局部变量
来源：http://lt.lnxyls.cn

f() { local x=1; echo "$x"; }
来源：http://sq.yuexingan06.cn

[R32] 参数个数校验
来源：http://km.yuexingan06.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://fh.huixiangedu.cn

[R33] 捕获错误并提示行号
来源：http://bj.haigaiapp.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://cv.hnjuh.cn

[R34] 退出时清理
来源：http://lq.haigaiapp.cn

trap 'rm -f "$tmp"' EXIT
来源：http://up.gzmigu.cn

[R35] 后台执行并等待
来源：http://lf.panjiajie.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://ti.chemitech.net.cn

[R36] 并发执行多个任务
来源：http://yk.hnjuh.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ah.asd995.cn

[R37] 把输出赋给变量
来源：http://ou.chemitech.net.cn

files=$(ls -1)
来源：http://lo.huixiangedu.cn

[R38] 管道串联
来源：http://qd.huixiangedu.cn

cat a.txt | grep -i error | wc -l
来源：http://ap.asd995.cn

[R39] 重定向标准输出与错误
来源：http://fm.haigaiapp.cn

cmd > out.log 2>&1
来源：http://dh.hahajie.cn

[R40] 追加写日志
来源：http://sw.jianghongdianzi.cn

echo "log" >> out.log
来源：http://ax.newstarts.cn

[R41] 丢弃输出
来源：http://jn.szxytkj.cn

cmd >/dev/null 2>&1
来源：http://si.shtwfgs.cn

[R42] 输入重定向
来源：http://vd.szsharing.cn

wc -l < a.txt
来源：http://mh.nszjky.cn

[R43] 按名字查找文件
来源：http://iw.nszjky.cn

find . -name "*.log" -type f
来源：http://bj.gzmigu.cn

[R44] 按修改时间查找
来源：http://aj.nszjky.cn

find . -mtime -7 -type f
来源：http://vl.jianghongdianzi.cn

[R45] 批量删除
来源：http://qb.yuexingan06.cn

find . -name "*.tmp" -delete
来源：http://jk.haigaiapp.cn

[R46] 递归替换文件内容
来源：http://bg.nicolike.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ww.jctech888.com.cn

[R47] sed 单行替换
来源：http://sp.nicolike.cn

sed -i 's/foo/bar/g' a.txt
来源：http://ic.yuexingan06.cn

[R48] awk 取指定列
来源：http://mc.asd995.cn

awk '{print $1, $3}' a.txt
来源：http://eb.huanxung.cn

[R49] awk 带条件
来源：http://uu.panjiajie.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ak.colortex.cn

[R50] awk 求和
来源：http://fp.haigaiapp.cn

awk '{s += $2} END {print s}' a.txt
来源：http://sh.gzmigu.cn

[R51] 排序去重取前几
来源：http://vf.yuexingan06.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://ph.wgjwhj.cn

[R52] 统计行数
来源：http://ra.haigaiapp.cn

wc -l a.txt
来源：http://hs.haigaiapp.cn

[R53] 查看文件头与实时尾
来源：http://sf.muxihuayi.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://jv.asd995.cn

[R54] 比较两个文件
来源：http://sc.szxytkj.cn

diff a.txt b.txt
来源：http://zx.lnxyls.cn

[R55] 压缩与解压
来源：http://qz.lnxyls.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wr.chemitech.net.cn

[R56] 远程拷贝
来源：http://fj.shtwfgs.cn

scp file user@host:/path/
来源：http://wo.muxihuayi.cn

[R57] 远程执行命令
来源：http://yc.szxytkj.cn

ssh user@host 'uptime'
来源：http://gw.shxzskj.cn

[R58] 下载文件
来源：http://nw.nicolike.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wm.yuntaijiaju.cn

[R59] 发 POST JSON
来源：http://fa.colortex.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://tw.yuexingan06.cn

[R60] 只看 HTTP 状态码
来源：http://hx.shtwfgs.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://kz.szxytkj.cn

[R61] 磁盘占用
来源：http://rj.gzmigu.cn

df -h;  du -sh *
来源：http://xv.shtwfgs.cn

[R62] 找最占空间的文件
来源：http://az.panjiajie.cn

du -ah . | sort -rh | head -10
来源：http://ve.muxihuayi.cn

[R63] 内存与进程
来源：http://yo.huixiangedu.cn

free -h;  ps aux | grep nginx
来源：http://cr.huixiangedu.cn

[R64] 结束进程
来源：http://qi.szxytkj.cn

kill -9 $(pgrep -f app.py)
来源：http://wp.shxzukj.cn

[R65] 查看端口占用
来源：http://bq.hnjuh.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://fo.nicolike.cn

[R66] 定时任务
来源：http://dr.haigaiapp.cn

crontab -e;  crontab -l
来源：http://ai.shxzskj.cn

[R67] 生成随机十六进制串
来源：http://yi.chemitech.net.cn

openssl rand -hex 16
来源：http://jj.9csxet.cn

[R68] 计算文件校验值
来源：http://ek.bookmarksfly.cn

sha256sum a.txt;  md5sum a.txt
来源：http://ny.jianghongdianzi.cn

[R69] 生成随机密码
来源：http://ng.yuexingan06.cn

head -c 16 /dev/urandom | base64
来源：http://to.haigaiapp.cn

[R70] 时间戳与互转
来源：http://sa.nicolike.cn

date +%s;  date -d @1700000000
来源：http://mv.panjiajie.cn

[R71] 日期格式化
来源：http://qf.bookmarksfly.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://hs.nicolike.cn

[R72] 等待端口就绪
来源：http://nx.nicolike.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://ds.panjiajie.cn

[R73] 分割大日志
来源：http://bb.haigaiapp.cn

split -l 1000 big.log part_
来源：http://cj.wgjwhj.cn

[R74] 批量重命名
来源：http://qt.jianghongdianzi.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://kt.gzmigu.cn

[R75] 导出环境变量
来源：http://lh.bookmarksfly.cn

export PATH="$HOME/bin:$PATH"
来源：http://mk.jianghongdianzi.cn

[R76] 使用临时文件
来源：http://gw.nszjky.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://us.nszjky.cn

[R77] 读取用户输入
来源：http://sm.szsharing.cn

read -rp "请输入: " ans
来源：http://tr.wgjwhj.cn

[R78] 交互式菜单
来源：http://fs.shxzskj.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://gs.colortex.cn

[R79] 解析命令行选项
来源：http://xm.yuexingan06.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://sa.wgjwhj.cn

[R80] 查看脚本执行耗时
来源：http://dn.lnxyls.cn

time ./run.sh
来源：http://ub.wgjwhj.cn

================================================================================
来源：http://wk.muxihuayi.cn

S. C / C++ 专题
来源：http://qy.nszjky.cn

================================================================================
来源：http://xy.szxytkj.cn

[S01] C：Hello World
来源：http://qb.huanxung.cn

#include <stdio.h>
来源：http://ju.yuexingan06.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://bt.bjjhwx.cn

[S02] C：变量与格式化输出
来源：http://fb.shtwfgs.cn

int a = 10; printf("%d\n", a);
来源：http://fd.hahajie.cn

[S03] C：读入整数
来源：http://mh.gzmigu.cn

int x; scanf("%d", &x);
来源：http://wu.nszjky.cn

[S04] C：字符串复制
来源：http://gs.lnxyls.cn

char dst[32]; strcpy(dst, "hi");
来源：http://xy.colortex.cn

[S05] C：字符串长度
来源：http://be.521024.cn


<!-- 参考信息 -->