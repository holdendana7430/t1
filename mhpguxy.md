代发 wailian999

[Q36] 左连接
来源：http://qr.gzmigu.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ea.jianghongdianzi.cn

[Q37] 右连接
来源：http://ch.colortex.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://on.gzmigu.cn

[Q38] 全外连接（PostgreSQL）
来源：http://gf.9csxet.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://rj.nicolike.cn

[Q39] 自连接（查上下级）
来源：http://bk.newstarts.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://vh.szxytkj.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://lg.haigaiapp.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://cj.colortex.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://xr.bjjhwx.cn

[Q41] 多表连接
来源：http://xt.szxytkj.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://vx.nszjky.cn

JOIN users u ON u.id = o.user_id
来源：http://lm.bjjhwx.cn

JOIN products p ON p.id = o.product_id;
来源：http://wv.hahajie.cn

[Q42] 连接条件附加过滤
来源：http://km.muxihuayi.cn

SELECT u.name, o.amount FROM users u
来源：http://ze.colortex.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ba.shxzukj.cn

[Q43] 标量子查询
来源：http://pc.colortex.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://io.bjjhwx.cn

[Q44] IN 子查询
来源：http://td.szsharing.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ca.shxzukj.cn

[Q45] EXISTS 判断存在
来源：http://um.shxzukj.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ot.colortex.cn

[Q46] NOT EXISTS 判断不存在
来源：http://wm.szsharing.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://vb.nszjky.cn

[Q47] 与平均值比较
来源：http://qv.lnxyls.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mo.newstarts.cn

[Q48] CTE 公用表表达式
来源：http://yw.hnjuh.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://up.huanxung.cn

SELECT * FROM t WHERE c > 5;
来源：http://sa.lnxyls.cn

[Q49] 更新单行
来源：http://pt.bjjhwx.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://iy.lnxyls.cn

[Q50] 批量更新
来源：http://ku.wgjwhj.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://xw.nszjky.cn

[Q51] 用子查询更新
来源：http://ua.bookmarksfly.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://gw.chemitech.net.cn

[Q52] 删除指定行
来源：http://wc.shtwfgs.cn

DELETE FROM users WHERE id = 10;
来源：http://dv.colortex.cn

[Q53] 按条件删除
来源：http://wx.wgjwhj.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://xz.bjjhwx.cn

[Q54] 清空表
来源：http://gl.shtwfgs.cn

TRUNCATE TABLE logs;
来源：http://sx.szxytkj.cn

[Q55] 排名（并列占位）
来源：http://mx.newstarts.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hf.wgjwhj.cn

[Q56] 密集排名（并列不占位）
来源：http://rt.szsharing.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://nk.hnjuh.cn

[Q57] 行号
来源：http://ca.huanxung.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://bs.shtwfgs.cn

[Q58] 累计求和
来源：http://nr.huixiangedu.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://jz.bookmarksfly.cn

[Q59] 分组内累计
来源：http://fs.haigaiapp.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ae.asd995.cn

[Q60] 取上一行 / 下一行
来源：http://yf.shxzskj.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ar.shtwfgs.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://sk.jctech888.com.cn

[Q61] 移动平均
来源：http://dx.lnxyls.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ph.huixiangedu.cn

[Q62] 分组占比
来源：http://pu.yuexingan06.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://as.nszjky.cn

[Q63] 开启事务
来源：http://jm.shxzskj.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://uq.521024.cn

[Q64] 提交事务
来源：http://ha.gzmigu.cn

COMMIT;
来源：http://xu.panjiajie.cn

[Q65] 回滚事务
来源：http://nu.huixiangedu.cn

ROLLBACK;
来源：http://ws.nszjky.cn

[Q66] 行锁查询
来源：http://nh.huanxung.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://tj.huixinmuqiang.cn

[Q67] 设置隔离级别
来源：http://qb.hnjuh.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://an.shxzukj.cn

[Q68] 保存点
来源：http://tn.shtwfgs.cn

SAVEPOINT sp1;
来源：http://fr.chemitech.net.cn

ROLLBACK TO sp1;
来源：http://nt.lnxyls.cn

[Q69] 查看执行计划
来源：http://ld.jianghongdianzi.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://vm.shxzskj.cn

[Q70] 更新统计信息
来源：http://wt.bookmarksfly.cn

ANALYZE TABLE users;
来源：http://mv.huixiangedu.cn

[Q71] 查看建表语句
来源：http://aq.yuntaijiaju.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ot.szsharing.cn

[Q72] 查看索引
来源：http://hl.yuexingan06.cn

SHOW INDEX FROM users;
来源：http://sb.bookmarksfly.cn

[Q73] 查看表状态
来源：http://ru.panjiajie.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://ka.521024.cn

[Q74] 强制使用索引
来源：http://uu.huanxung.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://rf.shxzskj.cn

[Q75] 日期格式化
来源：http://sz.jianghongdianzi.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://gg.huixinmuqiang.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://nt.huixiangedu.cn

[Q76] 按天统计
来源：http://ke.shxzskj.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://gb.jctech888.com.cn

[Q77] 时间加减
来源：http://vh.panjiajie.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://uw.asd995.cn

[Q78] 当前时间
来源：http://db.huixinmuqiang.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ug.huixiangedu.cn

[Q79] 字符串拼接
来源：http://qb.szxytkj.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://sn.wgjwhj.cn

[Q80] 字符串截取
来源：http://cw.szsharing.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://cq.nicolike.cn

[Q81] 字符串替换
来源：http://ab.521024.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hi.huanxung.cn

[Q82] 字符长度与字节长度
来源：http://oi.hahajie.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ug.shxzskj.cn

[Q83] 大小写转换
来源：http://eh.yuexingan06.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hy.asd995.cn

[Q84] 去除首尾空格
来源：http://vn.muxihuayi.cn

SELECT TRIM(name) FROM users;
来源：http://pa.chemitech.net.cn

[Q85] 数值取整
来源：http://gn.huixiangedu.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://cy.yuntaijiaju.cn

[Q86] 读取 JSON 字段
来源：http://lv.shxzskj.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ms.hahajie.cn

[Q87] JSON 字段做条件
来源：http://zd.huanxung.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ni.asd995.cn

[Q88] 行转列（条件聚合）
来源：http://is.hahajie.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ns.muxihuayi.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://iq.bookmarksfly.cn

[Q89] 判断表是否存在
来源：http://tv.hnjuh.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://uo.huanxung.cn

[Q90] 生成序号列
来源：http://pv.yuexingan06.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://rs.nszjky.cn

================================================================================
来源：http://ek.colortex.cn

R. Bash 专题
来源：http://xg.521024.cn

================================================================================
来源：http://kr.huixinmuqiang.cn

[R01] shebang 与严格模式
来源：http://fp.jctech888.com.cn

#!/usr/bin/env bash
来源：http://vx.shtwfgs.cn

set -euo pipefail
来源：http://ln.bookmarksfly.cn

[R02] 变量赋值与使用
来源：http://jp.jctech888.com.cn

name="Tom"; echo "$name"
来源：http://jj.nicolike.cn

[R03] 只读变量
来源：http://vc.haigaiapp.cn

readonly PI=3.14
来源：http://dv.newstarts.cn

[R04] 位置参数
来源：http://em.muxihuayi.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://xh.9csxet.cn

[R05] 参数默认值
来源：http://ke.shtwfgs.cn

name="${1:-default}"
来源：http://nh.yuntaijiaju.cn

[R06] 判断命令是否存在
来源：http://sf.9csxet.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://pd.bjjhwx.cn

[R07] if 判断文件
来源：http://la.yuexingan06.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://zd.nszjky.cn

[R08] 数值比较
来源：http://hq.yuntaijiaju.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://av.bookmarksfly.cn

[R09] 字符串比较
来源：http://xz.521024.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://gr.huixinmuqiang.cn

[R10] 正则匹配
来源：http://hl.jianghongdianzi.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://cb.nicolike.cn

[R11] case 多分支
来源：http://nr.szsharing.cn

case "$1" in
来源：http://da.shxzskj.cn

start) echo "启动" ;;
来源：http://rf.yuntaijiaju.cn

stop)  echo "停止" ;;
来源：http://uk.bjjhwx.cn

*)     echo "未知命令" ;;
来源：http://hc.hnjuh.cn

esac
来源：http://nm.bookmarksfly.cn

[R12] for 遍历文件
来源：http://ry.9csxet.cn

for f in *.txt; do echo "$f"; done
来源：http://lw.haigaiapp.cn

[R13] for 计数循环
来源：http://sv.bookmarksfly.cn

for i in {1..10}; do echo "$i"; done
来源：http://ec.yuntaijiaju.cn

[R14] C 风格 for
来源：http://tr.bjjhwx.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hs.shxzskj.cn

[R15] while 逐行读文件
来源：http://sb.shxzukj.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://sr.huixiangedu.cn

[R16] until 等待条件
来源：http://vu.huixinmuqiang.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ev.gzmigu.cn

[R17] 数组定义与取值
来源：http://il.hnjuh.cn

arr=(a b c); echo "${arr[0]}"
来源：http://ty.9csxet.cn

[R18] 遍历数组
来源：http://up.wgjwhj.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ez.huixiangedu.cn

[R19] 数组长度
来源：http://ea.huixiangedu.cn

echo "${#arr[@]}"
来源：http://dx.haigaiapp.cn

[R20] 关联数组（字典）
来源：http://gu.521024.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://jt.panjiajie.cn

[R21] 字符串长度
来源：http://jn.jctech888.com.cn

echo "${#s}"
来源：http://pd.huanxung.cn

[R22] 截取子串
来源：http://qs.muxihuayi.cn

echo "${s:0:5}"
来源：http://up.yuexingan06.cn

[R23] 字符串替换
来源：http://tb.shxzukj.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ti.huanxung.cn

[R24] 大小写转换
来源：http://gp.huixiangedu.cn

echo "${s^^}"; echo "${s,,}"
来源：http://zn.jctech888.com.cn

[R25] 去后缀 / 去前缀
来源：http://nc.bookmarksfly.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://ci.huanxung.cn

[R26] 命令替换
来源：http://yc.muxihuayi.cn

now=$(date +%F); echo "$now"
来源：http://mk.521024.cn

[R27] 算术展开
来源：http://pk.colortex.cn

echo $((1 + 2 * 3))
来源：http://zs.shtwfgs.cn

[R28] 浮点运算
来源：http://ul.lnxyls.cn

echo "scale=2; 10/3" | bc
来源：http://kr.muxihuayi.cn

[R29] 定义函数
来源：http://rw.nicolike.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wg.huixiangedu.cn

[R30] 函数返回状态码
来源：http://ph.yuntaijiaju.cn

f() { return 0; }; f || echo "失败了"
来源：http://ok.gzmigu.cn

[R31] 局部变量
来源：http://bi.bookmarksfly.cn

f() { local x=1; echo "$x"; }
来源：http://fb.bjjhwx.cn

[R32] 参数个数校验
来源：http://kg.wgjwhj.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ob.shxzukj.cn

[R33] 捕获错误并提示行号
来源：http://eh.asd995.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://sc.shxzukj.cn

[R34] 退出时清理
来源：http://nu.jianghongdianzi.cn

trap 'rm -f "$tmp"' EXIT
来源：http://tf.lnxyls.cn

[R35] 后台执行并等待
来源：http://yo.gzmigu.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://qu.jianghongdianzi.cn

[R36] 并发执行多个任务
来源：http://ew.shtwfgs.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mq.shtwfgs.cn

[R37] 把输出赋给变量
来源：http://ub.wgjwhj.cn

files=$(ls -1)
来源：http://gn.haigaiapp.cn

[R38] 管道串联
来源：http://bw.jctech888.com.cn

cat a.txt | grep -i error | wc -l
来源：http://zt.asd995.cn

[R39] 重定向标准输出与错误
来源：http://xl.wgjwhj.cn

cmd > out.log 2>&1
来源：http://zo.shxzukj.cn

[R40] 追加写日志
来源：http://pn.nicolike.cn

echo "log" >> out.log
来源：http://it.huixiangedu.cn

[R41] 丢弃输出
来源：http://sx.shxzukj.cn

cmd >/dev/null 2>&1
来源：http://cd.shxzukj.cn

[R42] 输入重定向
来源：http://zb.lnxyls.cn

wc -l < a.txt
来源：http://lx.huixiangedu.cn

[R43] 按名字查找文件
来源：http://ab.colortex.cn

find . -name "*.log" -type f
来源：http://rl.521024.cn

[R44] 按修改时间查找
来源：http://vg.haigaiapp.cn

find . -mtime -7 -type f
来源：http://fr.chemitech.net.cn

[R45] 批量删除
来源：http://qc.shxzukj.cn

find . -name "*.tmp" -delete
来源：http://jb.newstarts.cn

[R46] 递归替换文件内容
来源：http://oi.muxihuayi.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://dk.gzmigu.cn

[R47] sed 单行替换
来源：http://yg.jctech888.com.cn

sed -i 's/foo/bar/g' a.txt
来源：http://kz.muxihuayi.cn

[R48] awk 取指定列
来源：http://va.jianghongdianzi.cn

awk '{print $1, $3}' a.txt
来源：http://jv.9csxet.cn

[R49] awk 带条件
来源：http://bk.lnxyls.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ve.521024.cn

[R50] awk 求和
来源：http://sr.wgjwhj.cn

awk '{s += $2} END {print s}' a.txt
来源：http://sd.bookmarksfly.cn

[R51] 排序去重取前几
来源：http://aw.colortex.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://gi.szsharing.cn

[R52] 统计行数
来源：http://qp.hnjuh.cn

wc -l a.txt
来源：http://kh.bjjhwx.cn

[R53] 查看文件头与实时尾
来源：http://vr.yuntaijiaju.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://pb.521024.cn

[R54] 比较两个文件
来源：http://rr.newstarts.cn

diff a.txt b.txt
来源：http://ff.jianghongdianzi.cn

[R55] 压缩与解压
来源：http://xb.gzmigu.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://pr.huixiangedu.cn

[R56] 远程拷贝
来源：http://tf.9csxet.cn

scp file user@host:/path/
来源：http://db.shtwfgs.cn

[R57] 远程执行命令
来源：http://ys.lnxyls.cn

ssh user@host 'uptime'
来源：http://mv.szxytkj.cn

[R58] 下载文件
来源：http://nn.9csxet.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://em.szsharing.cn

[R59] 发 POST JSON
来源：http://nl.huanxung.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://pq.asd995.cn

[R60] 只看 HTTP 状态码
来源：http://fl.gzmigu.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://pl.shxzukj.cn

[R61] 磁盘占用
来源：http://rz.9csxet.cn

df -h;  du -sh *
来源：http://er.asd995.cn

[R62] 找最占空间的文件
来源：http://ih.haigaiapp.cn

du -ah . | sort -rh | head -10
来源：http://bj.chemitech.net.cn

[R63] 内存与进程
来源：http://fk.shxzskj.cn

free -h;  ps aux | grep nginx
来源：http://wa.hnjuh.cn

[R64] 结束进程
来源：http://vk.nicolike.cn

kill -9 $(pgrep -f app.py)
来源：http://hm.shtwfgs.cn

[R65] 查看端口占用
来源：http://zw.hahajie.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://pf.gzmigu.cn

[R66] 定时任务
来源：http://nl.nicolike.cn

crontab -e;  crontab -l
来源：http://fc.muxihuayi.cn

[R67] 生成随机十六进制串
来源：http://ah.newstarts.cn

openssl rand -hex 16
来源：http://ta.9csxet.cn

[R68] 计算文件校验值
来源：http://vi.muxihuayi.cn

sha256sum a.txt;  md5sum a.txt
来源：http://bm.asd995.cn

[R69] 生成随机密码
来源：http://hf.hnjuh.cn

head -c 16 /dev/urandom | base64
来源：http://sh.jctech888.com.cn

[R70] 时间戳与互转
来源：http://dp.muxihuayi.cn

date +%s;  date -d @1700000000
来源：http://qh.jianghongdianzi.cn

[R71] 日期格式化
来源：http://kv.haigaiapp.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://ss.hahajie.cn

[R72] 等待端口就绪
来源：http://ew.asd995.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://cl.huixiangedu.cn

[R73] 分割大日志
来源：http://gt.szxytkj.cn

split -l 1000 big.log part_
来源：http://bk.yuexingan06.cn

[R74] 批量重命名
来源：http://fv.nicolike.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://un.hnjuh.cn

[R75] 导出环境变量
来源：http://wu.jctech888.com.cn

export PATH="$HOME/bin:$PATH"
来源：http://cw.huixinmuqiang.cn

[R76] 使用临时文件
来源：http://hs.szsharing.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wr.gzmigu.cn

[R77] 读取用户输入
来源：http://ze.shtwfgs.cn

read -rp "请输入: " ans
来源：http://mn.shxzskj.cn

[R78] 交互式菜单
来源：http://oz.bjjhwx.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://ns.yuntaijiaju.cn

[R79] 解析命令行选项
来源：http://ki.huanxung.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://dk.szsharing.cn

[R80] 查看脚本执行耗时
来源：http://az.panjiajie.cn

time ./run.sh
来源：http://ak.bjjhwx.cn

================================================================================
来源：http://rq.hnjuh.cn

S. C / C++ 专题
来源：http://zr.huanxung.cn

================================================================================
来源：http://sx.gzmigu.cn

[S01] C：Hello World
来源：http://fr.colortex.cn

#include <stdio.h>
来源：http://qo.shxzukj.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://lw.huanxung.cn

[S02] C：变量与格式化输出
来源：http://xa.huanxung.cn

int a = 10; printf("%d\n", a);
来源：http://wk.nicolike.cn

[S03] C：读入整数
来源：http://gm.colortex.cn

int x; scanf("%d", &x);
来源：http://sn.521024.cn

[S04] C：字符串复制
来源：http://br.shxzskj.cn

char dst[32]; strcpy(dst, "hi");
来源：http://gj.szsharing.cn

[S05] C：字符串长度
来源：http://rs.szsharing.cn


<!-- 参考信息 -->