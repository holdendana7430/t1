代发 wailian999

[Q38] 全外连接（PostgreSQL）
来源：http://ee.521024.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ip.muxihuayi.cn

[Q39] 自连接（查上下级）
来源：http://tb.yuntaijiaju.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://dw.nszjky.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://sx.huixiangedu.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://hj.521024.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://yf.haigaiapp.cn

[Q41] 多表连接
来源：http://gw.jianghongdianzi.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://fo.nszjky.cn

JOIN users u ON u.id = o.user_id
来源：http://mu.newstarts.cn

JOIN products p ON p.id = o.product_id;
来源：http://zx.lnxyls.cn

[Q42] 连接条件附加过滤
来源：http://fg.shxzukj.cn

SELECT u.name, o.amount FROM users u
来源：http://om.wgjwhj.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ms.bookmarksfly.cn

[Q43] 标量子查询
来源：http://qv.huanxung.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://bs.bookmarksfly.cn

[Q44] IN 子查询
来源：http://tb.521024.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hk.gzmigu.cn

[Q45] EXISTS 判断存在
来源：http://hh.521024.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://zt.gzmigu.cn

[Q46] NOT EXISTS 判断不存在
来源：http://uv.haigaiapp.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mh.newstarts.cn

[Q47] 与平均值比较
来源：http://la.shxzskj.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://et.colortex.cn

[Q48] CTE 公用表表达式
来源：http://mq.jianghongdianzi.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://tw.chemitech.net.cn

SELECT * FROM t WHERE c > 5;
来源：http://em.muxihuayi.cn

[Q49] 更新单行
来源：http://hn.jctech888.com.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mo.nicolike.cn

[Q50] 批量更新
来源：http://fx.jctech888.com.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://na.wgjwhj.cn

[Q51] 用子查询更新
来源：http://no.521024.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://dl.jianghongdianzi.cn

[Q52] 删除指定行
来源：http://wm.bjjhwx.cn

DELETE FROM users WHERE id = 10;
来源：http://dr.hahajie.cn

[Q53] 按条件删除
来源：http://un.lnxyls.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://na.gzmigu.cn

[Q54] 清空表
来源：http://ma.nicolike.cn

TRUNCATE TABLE logs;
来源：http://lr.szsharing.cn

[Q55] 排名（并列占位）
来源：http://vi.chemitech.net.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://xs.colortex.cn

[Q56] 密集排名（并列不占位）
来源：http://ux.asd995.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://pw.jianghongdianzi.cn

[Q57] 行号
来源：http://wa.shxzukj.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://pq.newstarts.cn

[Q58] 累计求和
来源：http://mo.shxzukj.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://yj.muxihuayi.cn

[Q59] 分组内累计
来源：http://mp.9csxet.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://qa.muxihuayi.cn

[Q60] 取上一行 / 下一行
来源：http://mp.9csxet.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://eb.9csxet.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://rf.huanxung.cn

[Q61] 移动平均
来源：http://da.newstarts.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://lf.asd995.cn

[Q62] 分组占比
来源：http://ya.huixinmuqiang.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://te.jctech888.com.cn

[Q63] 开启事务
来源：http://ei.muxihuayi.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://ap.newstarts.cn

[Q64] 提交事务
来源：http://vi.jianghongdianzi.cn

COMMIT;
来源：http://ru.asd995.cn

[Q65] 回滚事务
来源：http://mw.panjiajie.cn

ROLLBACK;
来源：http://ot.panjiajie.cn

[Q66] 行锁查询
来源：http://yr.hnjuh.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mv.jianghongdianzi.cn

[Q67] 设置隔离级别
来源：http://fq.bjjhwx.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://tx.asd995.cn

[Q68] 保存点
来源：http://sw.huanxung.cn

SAVEPOINT sp1;
来源：http://bp.panjiajie.cn

ROLLBACK TO sp1;
来源：http://re.yuntaijiaju.cn

[Q69] 查看执行计划
来源：http://bi.hahajie.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ko.nicolike.cn

[Q70] 更新统计信息
来源：http://ik.lnxyls.cn

ANALYZE TABLE users;
来源：http://np.nszjky.cn

[Q71] 查看建表语句
来源：http://pw.9csxet.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ug.haigaiapp.cn

[Q72] 查看索引
来源：http://ir.jianghongdianzi.cn

SHOW INDEX FROM users;
来源：http://oa.huanxung.cn

[Q73] 查看表状态
来源：http://sw.gzmigu.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://ca.szsharing.cn

[Q74] 强制使用索引
来源：http://jl.jianghongdianzi.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://dk.panjiajie.cn

[Q75] 日期格式化
来源：http://ty.chemitech.net.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://oe.nicolike.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://qg.nszjky.cn

[Q76] 按天统计
来源：http://yu.shxzskj.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ti.hahajie.cn

[Q77] 时间加减
来源：http://ud.shxzskj.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://kt.haigaiapp.cn

[Q78] 当前时间
来源：http://ko.muxihuayi.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://lb.colortex.cn

[Q79] 字符串拼接
来源：http://xh.lnxyls.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://pu.jctech888.com.cn

[Q80] 字符串截取
来源：http://wm.colortex.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://gz.521024.cn

[Q81] 字符串替换
来源：http://om.yuntaijiaju.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://rn.haigaiapp.cn

[Q82] 字符长度与字节长度
来源：http://oh.9csxet.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://tx.521024.cn

[Q83] 大小写转换
来源：http://oa.szsharing.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://en.9csxet.cn

[Q84] 去除首尾空格
来源：http://du.521024.cn

SELECT TRIM(name) FROM users;
来源：http://yy.newstarts.cn

[Q85] 数值取整
来源：http://ig.nszjky.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mn.chemitech.net.cn

[Q86] 读取 JSON 字段
来源：http://sp.bookmarksfly.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ft.szsharing.cn

[Q87] JSON 字段做条件
来源：http://wo.gzmigu.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mr.newstarts.cn

[Q88] 行转列（条件聚合）
来源：http://lu.gzmigu.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ws.yuexingan06.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://gb.nszjky.cn

[Q89] 判断表是否存在
来源：http://nh.asd995.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://gb.haigaiapp.cn

[Q90] 生成序号列
来源：http://aq.panjiajie.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://sd.huanxung.cn

================================================================================
来源：http://yj.hahajie.cn

R. Bash 专题
来源：http://mg.nszjky.cn

================================================================================
来源：http://ls.9csxet.cn

[R01] shebang 与严格模式
来源：http://bx.nicolike.cn

#!/usr/bin/env bash
来源：http://iy.521024.cn

set -euo pipefail
来源：http://dk.muxihuayi.cn

[R02] 变量赋值与使用
来源：http://ls.colortex.cn

name="Tom"; echo "$name"
来源：http://jc.jianghongdianzi.cn

[R03] 只读变量
来源：http://vh.9csxet.cn

readonly PI=3.14
来源：http://xe.nszjky.cn

[R04] 位置参数
来源：http://bs.shxzukj.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ys.bookmarksfly.cn

[R05] 参数默认值
来源：http://qz.hahajie.cn

name="${1:-default}"
来源：http://cn.bjjhwx.cn

[R06] 判断命令是否存在
来源：http://hu.shtwfgs.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://fq.shtwfgs.cn

[R07] if 判断文件
来源：http://lf.newstarts.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://pi.panjiajie.cn

[R08] 数值比较
来源：http://tw.huixiangedu.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://uf.colortex.cn

[R09] 字符串比较
来源：http://fu.huixiangedu.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wi.huixinmuqiang.cn

[R10] 正则匹配
来源：http://pr.9csxet.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://gc.huixinmuqiang.cn

[R11] case 多分支
来源：http://kw.shxzukj.cn

case "$1" in
来源：http://ve.bookmarksfly.cn

start) echo "启动" ;;
来源：http://zp.shxzukj.cn

stop)  echo "停止" ;;
来源：http://jc.yuexingan06.cn

*)     echo "未知命令" ;;
来源：http://ip.newstarts.cn

esac
来源：http://rq.jianghongdianzi.cn

[R12] for 遍历文件
来源：http://js.colortex.cn

for f in *.txt; do echo "$f"; done
来源：http://go.panjiajie.cn

[R13] for 计数循环
来源：http://je.gzmigu.cn

for i in {1..10}; do echo "$i"; done
来源：http://kg.muxihuayi.cn

[R14] C 风格 for
来源：http://fs.szxytkj.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wv.nicolike.cn

[R15] while 逐行读文件
来源：http://yd.bookmarksfly.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://gp.wgjwhj.cn

[R16] until 等待条件
来源：http://zm.nszjky.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://tf.szsharing.cn

[R17] 数组定义与取值
来源：http://de.newstarts.cn

arr=(a b c); echo "${arr[0]}"
来源：http://nt.shtwfgs.cn

[R18] 遍历数组
来源：http://ob.szxytkj.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://gn.gzmigu.cn

[R19] 数组长度
来源：http://ys.shxzukj.cn

echo "${#arr[@]}"
来源：http://uj.haigaiapp.cn

[R20] 关联数组（字典）
来源：http://us.521024.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://rt.shxzskj.cn

[R21] 字符串长度
来源：http://ir.shxzukj.cn

echo "${#s}"
来源：http://cy.jctech888.com.cn

[R22] 截取子串
来源：http://ip.huixinmuqiang.cn

echo "${s:0:5}"
来源：http://pu.huanxung.cn

[R23] 字符串替换
来源：http://nl.bookmarksfly.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://uz.shtwfgs.cn

[R24] 大小写转换
来源：http://th.colortex.cn

echo "${s^^}"; echo "${s,,}"
来源：http://pf.asd995.cn

[R25] 去后缀 / 去前缀
来源：http://sw.nszjky.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://gz.521024.cn

[R26] 命令替换
来源：http://pu.wgjwhj.cn

now=$(date +%F); echo "$now"
来源：http://yn.nicolike.cn

[R27] 算术展开
来源：http://my.nszjky.cn

echo $((1 + 2 * 3))
来源：http://pc.shxzukj.cn

[R28] 浮点运算
来源：http://ge.shtwfgs.cn

echo "scale=2; 10/3" | bc
来源：http://hv.panjiajie.cn

[R29] 定义函数
来源：http://cf.yuntaijiaju.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ay.nszjky.cn

[R30] 函数返回状态码
来源：http://tj.hnjuh.cn

f() { return 0; }; f || echo "失败了"
来源：http://oc.panjiajie.cn

[R31] 局部变量
来源：http://bi.bookmarksfly.cn

f() { local x=1; echo "$x"; }
来源：http://if.lnxyls.cn

[R32] 参数个数校验
来源：http://va.huixiangedu.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.muxihuayi.cn

[R33] 捕获错误并提示行号
来源：http://pw.wgjwhj.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://nv.jctech888.com.cn

[R34] 退出时清理
来源：http://xn.szsharing.cn

trap 'rm -f "$tmp"' EXIT
来源：http://iu.nicolike.cn

[R35] 后台执行并等待
来源：http://lt.gzmigu.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://zm.haigaiapp.cn

[R36] 并发执行多个任务
来源：http://ht.yuntaijiaju.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://aq.huixiangedu.cn

[R37] 把输出赋给变量
来源：http://vl.9csxet.cn

files=$(ls -1)
来源：http://ca.shtwfgs.cn

[R38] 管道串联
来源：http://qw.bookmarksfly.cn

cat a.txt | grep -i error | wc -l
来源：http://xj.bjjhwx.cn

[R39] 重定向标准输出与错误
来源：http://ki.gzmigu.cn

cmd > out.log 2>&1
来源：http://aa.shxzukj.cn

[R40] 追加写日志
来源：http://ac.521024.cn

echo "log" >> out.log
来源：http://yu.muxihuayi.cn

[R41] 丢弃输出
来源：http://pn.shxzukj.cn

cmd >/dev/null 2>&1
来源：http://uz.shxzskj.cn

[R42] 输入重定向
来源：http://cv.lnxyls.cn

wc -l < a.txt
来源：http://jl.muxihuayi.cn

[R43] 按名字查找文件
来源：http://tn.hnjuh.cn

find . -name "*.log" -type f
来源：http://nq.wgjwhj.cn

[R44] 按修改时间查找
来源：http://vp.yuexingan06.cn

find . -mtime -7 -type f
来源：http://be.huixiangedu.cn

[R45] 批量删除
来源：http://lc.lnxyls.cn

find . -name "*.tmp" -delete
来源：http://kv.szxytkj.cn

[R46] 递归替换文件内容
来源：http://nt.jctech888.com.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://xn.bjjhwx.cn

[R47] sed 单行替换
来源：http://ep.huixiangedu.cn

sed -i 's/foo/bar/g' a.txt
来源：http://ul.muxihuayi.cn

[R48] awk 取指定列
来源：http://ft.asd995.cn

awk '{print $1, $3}' a.txt
来源：http://ui.wgjwhj.cn

[R49] awk 带条件
来源：http://oo.9csxet.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://vj.nszjky.cn

[R50] awk 求和
来源：http://js.jianghongdianzi.cn

awk '{s += $2} END {print s}' a.txt
来源：http://hw.bookmarksfly.cn

[R51] 排序去重取前几
来源：http://zx.huixiangedu.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://dh.muxihuayi.cn

[R52] 统计行数
来源：http://jr.wgjwhj.cn

wc -l a.txt
来源：http://bm.shxzskj.cn

[R53] 查看文件头与实时尾
来源：http://jr.szxytkj.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ju.huixiangedu.cn

[R54] 比较两个文件
来源：http://te.shtwfgs.cn

diff a.txt b.txt
来源：http://to.521024.cn

[R55] 压缩与解压
来源：http://mc.shtwfgs.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://eg.jctech888.com.cn

[R56] 远程拷贝
来源：http://xu.huanxung.cn

scp file user@host:/path/
来源：http://ki.wgjwhj.cn

[R57] 远程执行命令
来源：http://er.nicolike.cn

ssh user@host 'uptime'
来源：http://hy.huixiangedu.cn

[R58] 下载文件
来源：http://iz.shtwfgs.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://vv.szxytkj.cn

[R59] 发 POST JSON
来源：http://mw.bjjhwx.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://zw.szsharing.cn

[R60] 只看 HTTP 状态码
来源：http://wn.szsharing.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mi.nszjky.cn

[R61] 磁盘占用
来源：http://cz.jianghongdianzi.cn

df -h;  du -sh *
来源：http://qn.bookmarksfly.cn

[R62] 找最占空间的文件
来源：http://xh.shxzskj.cn

du -ah . | sort -rh | head -10
来源：http://fx.yuexingan06.cn

[R63] 内存与进程
来源：http://rn.hnjuh.cn

free -h;  ps aux | grep nginx
来源：http://iw.hnjuh.cn

[R64] 结束进程
来源：http://ok.bookmarksfly.cn

kill -9 $(pgrep -f app.py)
来源：http://my.yuexingan06.cn

[R65] 查看端口占用
来源：http://st.gzmigu.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mw.nszjky.cn

[R66] 定时任务
来源：http://ar.521024.cn

crontab -e;  crontab -l
来源：http://ky.bjjhwx.cn

[R67] 生成随机十六进制串
来源：http://al.shtwfgs.cn

openssl rand -hex 16
来源：http://sx.lnxyls.cn

[R68] 计算文件校验值
来源：http://zd.newstarts.cn

sha256sum a.txt;  md5sum a.txt
来源：http://xp.bookmarksfly.cn

[R69] 生成随机密码
来源：http://ng.gzmigu.cn

head -c 16 /dev/urandom | base64
来源：http://rs.muxihuayi.cn

[R70] 时间戳与互转
来源：http://us.bjjhwx.cn

date +%s;  date -d @1700000000
来源：http://ds.wgjwhj.cn

[R71] 日期格式化
来源：http://gp.shtwfgs.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://ed.shxzukj.cn

[R72] 等待端口就绪
来源：http://sb.szxytkj.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://ah.shtwfgs.cn

[R73] 分割大日志
来源：http://no.haigaiapp.cn

split -l 1000 big.log part_
来源：http://hu.chemitech.net.cn

[R74] 批量重命名
来源：http://dh.9csxet.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://dh.szxytkj.cn

[R75] 导出环境变量
来源：http://nf.jctech888.com.cn

export PATH="$HOME/bin:$PATH"
来源：http://sg.yuexingan06.cn

[R76] 使用临时文件
来源：http://oj.lnxyls.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://vi.521024.cn

[R77] 读取用户输入
来源：http://am.9csxet.cn

read -rp "请输入: " ans
来源：http://mh.szsharing.cn

[R78] 交互式菜单
来源：http://rt.panjiajie.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://ls.wgjwhj.cn

[R79] 解析命令行选项
来源：http://hc.chemitech.net.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hi.szsharing.cn

[R80] 查看脚本执行耗时
来源：http://eu.huixiangedu.cn

time ./run.sh
来源：http://hz.hnjuh.cn

================================================================================
来源：http://em.yuntaijiaju.cn

S. C / C++ 专题
来源：http://tr.wgjwhj.cn

================================================================================
来源：http://wu.hnjuh.cn

[S01] C：Hello World
来源：http://mo.chemitech.net.cn

#include <stdio.h>
来源：http://fs.huixinmuqiang.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://aq.huixiangedu.cn

[S02] C：变量与格式化输出
来源：http://cp.shtwfgs.cn

int a = 10; printf("%d\n", a);
来源：http://ox.shtwfgs.cn

[S03] C：读入整数
来源：http://fu.newstarts.cn

int x; scanf("%d", &x);
来源：http://bv.shxzukj.cn

[S04] C：字符串复制
来源：http://lh.shxzukj.cn

char dst[32]; strcpy(dst, "hi");
来源：http://wg.huixiangedu.cn

[S05] C：字符串长度
来源：http://fk.nicolike.cn

strlen(s)
来源：http://qy.asd995.cn

[S06] C：字符串比较
来源：http://yh.asd995.cn

strcmp(a, b) == 0
来源：http://ft.asd995.cn

[S07] C：数组遍历求和
来源：http://bh.gzmigu.cn


<!-- 参考信息 -->