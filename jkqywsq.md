代发 wailian999

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://rf.bjjhwx.cn

[Q32] 分组拼接字符串
来源：http://cp.shtwfgs.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://uo.asd995.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://iq.521024.cn

[Q33] 多列分组
来源：http://ko.bjjhwx.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wf.521024.cn

[Q34] 每组取第一条
来源：http://zg.szsharing.cn

SELECT * FROM (
来源：http://td.huixinmuqiang.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://eq.muxihuayi.cn

) t WHERE rn = 1;
来源：http://lf.lnxyls.cn

[Q35] 内连接
来源：http://ly.521024.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://cq.521024.cn

[Q36] 左连接
来源：http://ml.gzmigu.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mt.9csxet.cn

[Q37] 右连接
来源：http://ba.wgjwhj.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://dj.haigaiapp.cn

[Q38] 全外连接（PostgreSQL）
来源：http://zy.wgjwhj.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://sl.jctech888.com.cn

[Q39] 自连接（查上下级）
来源：http://fl.nicolike.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://mq.szxytkj.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://og.yuexingan06.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://tt.haigaiapp.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://fw.shxzukj.cn

[Q41] 多表连接
来源：http://xc.panjiajie.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://fo.jianghongdianzi.cn

JOIN users u ON u.id = o.user_id
来源：http://hh.hahajie.cn

JOIN products p ON p.id = o.product_id;
来源：http://tt.lnxyls.cn

[Q42] 连接条件附加过滤
来源：http://nu.hnjuh.cn

SELECT u.name, o.amount FROM users u
来源：http://qj.haigaiapp.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mx.shtwfgs.cn

[Q43] 标量子查询
来源：http://xn.bookmarksfly.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://lv.huanxung.cn

[Q44] IN 子查询
来源：http://jb.colortex.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://xf.muxihuayi.cn

[Q45] EXISTS 判断存在
来源：http://ax.haigaiapp.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://xc.nicolike.cn

[Q46] NOT EXISTS 判断不存在
来源：http://ad.asd995.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://sg.hahajie.cn

[Q47] 与平均值比较
来源：http://hn.shtwfgs.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://pu.wgjwhj.cn

[Q48] CTE 公用表表达式
来源：http://nd.bjjhwx.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://lm.shtwfgs.cn

SELECT * FROM t WHERE c > 5;
来源：http://sl.shxzukj.cn

[Q49] 更新单行
来源：http://es.szxytkj.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://qc.wgjwhj.cn

[Q50] 批量更新
来源：http://dt.jianghongdianzi.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://sb.shtwfgs.cn

[Q51] 用子查询更新
来源：http://bp.huanxung.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://zo.9csxet.cn

[Q52] 删除指定行
来源：http://sy.bookmarksfly.cn

DELETE FROM users WHERE id = 10;
来源：http://so.bjjhwx.cn

[Q53] 按条件删除
来源：http://fb.521024.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wf.newstarts.cn

[Q54] 清空表
来源：http://wg.gzmigu.cn

TRUNCATE TABLE logs;
来源：http://cz.shtwfgs.cn

[Q55] 排名（并列占位）
来源：http://iw.521024.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://gy.gzmigu.cn

[Q56] 密集排名（并列不占位）
来源：http://vi.shxzskj.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ea.huanxung.cn

[Q57] 行号
来源：http://fz.colortex.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ym.colortex.cn

[Q58] 累计求和
来源：http://lz.shtwfgs.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://tw.hahajie.cn

[Q59] 分组内累计
来源：http://ui.hnjuh.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://as.szxytkj.cn

[Q60] 取上一行 / 下一行
来源：http://vx.chemitech.net.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://eu.panjiajie.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hv.huixiangedu.cn

[Q61] 移动平均
来源：http://iu.nszjky.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://xn.szxytkj.cn

[Q62] 分组占比
来源：http://ky.wgjwhj.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://qp.panjiajie.cn

[Q63] 开启事务
来源：http://rs.gzmigu.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://cd.asd995.cn

[Q64] 提交事务
来源：http://nu.shxzskj.cn

COMMIT;
来源：http://ax.yuexingan06.cn

[Q65] 回滚事务
来源：http://qz.huixinmuqiang.cn

ROLLBACK;
来源：http://eu.haigaiapp.cn

[Q66] 行锁查询
来源：http://kj.yuexingan06.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://iu.shxzukj.cn

[Q67] 设置隔离级别
来源：http://mw.wgjwhj.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://xr.nicolike.cn

[Q68] 保存点
来源：http://kn.shtwfgs.cn

SAVEPOINT sp1;
来源：http://lt.huixinmuqiang.cn

ROLLBACK TO sp1;
来源：http://rh.bookmarksfly.cn

[Q69] 查看执行计划
来源：http://au.jianghongdianzi.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://it.jctech888.com.cn

[Q70] 更新统计信息
来源：http://rz.yuexingan06.cn

ANALYZE TABLE users;
来源：http://fw.newstarts.cn

[Q71] 查看建表语句
来源：http://nf.asd995.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://eb.hnjuh.cn

[Q72] 查看索引
来源：http://sj.szsharing.cn

SHOW INDEX FROM users;
来源：http://np.haigaiapp.cn

[Q73] 查看表状态
来源：http://pz.hahajie.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://kb.wgjwhj.cn

[Q74] 强制使用索引
来源：http://sa.nicolike.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://fw.bjjhwx.cn

[Q75] 日期格式化
来源：http://zy.muxihuayi.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://qs.521024.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://xc.jctech888.com.cn

[Q76] 按天统计
来源：http://dl.asd995.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://pd.muxihuayi.cn

[Q77] 时间加减
来源：http://tk.bjjhwx.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hh.newstarts.cn

[Q78] 当前时间
来源：http://vj.9csxet.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hc.wgjwhj.cn

[Q79] 字符串拼接
来源：http://fa.yuexingan06.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://xa.yuntaijiaju.cn

[Q80] 字符串截取
来源：http://ec.shxzskj.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://vo.panjiajie.cn

[Q81] 字符串替换
来源：http://yk.hnjuh.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://aj.yuntaijiaju.cn

[Q82] 字符长度与字节长度
来源：http://ul.521024.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://uy.bjjhwx.cn

[Q83] 大小写转换
来源：http://gu.wgjwhj.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://sa.yuntaijiaju.cn

[Q84] 去除首尾空格
来源：http://qy.nicolike.cn

SELECT TRIM(name) FROM users;
来源：http://tz.bjjhwx.cn

[Q85] 数值取整
来源：http://rq.jianghongdianzi.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://sv.bjjhwx.cn

[Q86] 读取 JSON 字段
来源：http://ci.shxzukj.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://be.huixiangedu.cn

[Q87] JSON 字段做条件
来源：http://ov.9csxet.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://dm.521024.cn

[Q88] 行转列（条件聚合）
来源：http://eq.shtwfgs.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://lg.huixinmuqiang.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://no.nicolike.cn

[Q89] 判断表是否存在
来源：http://vu.wgjwhj.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://vc.521024.cn

[Q90] 生成序号列
来源：http://en.nicolike.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://pf.colortex.cn

================================================================================
来源：http://yx.panjiajie.cn

R. Bash 专题
来源：http://bb.newstarts.cn

================================================================================
来源：http://ew.haigaiapp.cn

[R01] shebang 与严格模式
来源：http://aq.huixiangedu.cn

#!/usr/bin/env bash
来源：http://oa.yuexingan06.cn

set -euo pipefail
来源：http://lk.bookmarksfly.cn

[R02] 变量赋值与使用
来源：http://ib.yuexingan06.cn

name="Tom"; echo "$name"
来源：http://op.huixinmuqiang.cn

[R03] 只读变量
来源：http://ua.huixinmuqiang.cn

readonly PI=3.14
来源：http://kp.wgjwhj.cn

[R04] 位置参数
来源：http://mh.shxzskj.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ow.yuntaijiaju.cn

[R05] 参数默认值
来源：http://on.gzmigu.cn

name="${1:-default}"
来源：http://yw.shxzukj.cn

[R06] 判断命令是否存在
来源：http://lr.szsharing.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://cb.gzmigu.cn

[R07] if 判断文件
来源：http://az.haigaiapp.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ew.wgjwhj.cn

[R08] 数值比较
来源：http://rf.lnxyls.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://yx.lnxyls.cn

[R09] 字符串比较
来源：http://og.panjiajie.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://nn.shxzskj.cn

[R10] 正则匹配
来源：http://yq.gzmigu.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://lv.bjjhwx.cn

[R11] case 多分支
来源：http://tn.yuntaijiaju.cn

case "$1" in
来源：http://zl.jianghongdianzi.cn

start) echo "启动" ;;
来源：http://qu.yuexingan06.cn

stop)  echo "停止" ;;
来源：http://it.bjjhwx.cn

*)     echo "未知命令" ;;
来源：http://ld.521024.cn

esac
来源：http://st.yuntaijiaju.cn

[R12] for 遍历文件
来源：http://yd.jianghongdianzi.cn

for f in *.txt; do echo "$f"; done
来源：http://vw.gzmigu.cn

[R13] for 计数循环
来源：http://hc.jctech888.com.cn

for i in {1..10}; do echo "$i"; done
来源：http://gz.jctech888.com.cn

[R14] C 风格 for
来源：http://lv.huanxung.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ul.bookmarksfly.cn

[R15] while 逐行读文件
来源：http://va.bookmarksfly.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://zy.haigaiapp.cn

[R16] until 等待条件
来源：http://wy.hnjuh.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://uq.gzmigu.cn

[R17] 数组定义与取值
来源：http://bp.szxytkj.cn

arr=(a b c); echo "${arr[0]}"
来源：http://rt.szxytkj.cn

[R18] 遍历数组
来源：http://my.muxihuayi.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://xj.colortex.cn

[R19] 数组长度
来源：http://dx.nicolike.cn

echo "${#arr[@]}"
来源：http://vq.muxihuayi.cn

[R20] 关联数组（字典）
来源：http://fm.jianghongdianzi.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ol.shtwfgs.cn

[R21] 字符串长度
来源：http://st.hahajie.cn

echo "${#s}"
来源：http://tz.wgjwhj.cn

[R22] 截取子串
来源：http://zq.muxihuayi.cn

echo "${s:0:5}"
来源：http://zl.chemitech.net.cn

[R23] 字符串替换
来源：http://yr.shxzukj.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://bu.panjiajie.cn

[R24] 大小写转换
来源：http://ja.newstarts.cn

echo "${s^^}"; echo "${s,,}"
来源：http://fo.haigaiapp.cn

[R25] 去后缀 / 去前缀
来源：http://mn.shtwfgs.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://mm.huanxung.cn

[R26] 命令替换
来源：http://pb.lnxyls.cn

now=$(date +%F); echo "$now"
来源：http://pg.shxzskj.cn

[R27] 算术展开
来源：http://pw.huixinmuqiang.cn

echo $((1 + 2 * 3))
来源：http://sa.nszjky.cn

[R28] 浮点运算
来源：http://gq.gzmigu.cn

echo "scale=2; 10/3" | bc
来源：http://kt.nszjky.cn

[R29] 定义函数
来源：http://wd.huixinmuqiang.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ie.yuntaijiaju.cn

[R30] 函数返回状态码
来源：http://bh.bookmarksfly.cn

f() { return 0; }; f || echo "失败了"
来源：http://jw.huixiangedu.cn

[R31] 局部变量
来源：http://nb.wgjwhj.cn

f() { local x=1; echo "$x"; }
来源：http://jk.jianghongdianzi.cn

[R32] 参数个数校验
来源：http://ql.bjjhwx.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://dx.521024.cn

[R33] 捕获错误并提示行号
来源：http://fr.lnxyls.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://rh.jianghongdianzi.cn

[R34] 退出时清理
来源：http://mr.gzmigu.cn

trap 'rm -f "$tmp"' EXIT
来源：http://cb.gzmigu.cn

[R35] 后台执行并等待
来源：http://bj.huanxung.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://ci.asd995.cn

[R36] 并发执行多个任务
来源：http://ck.jianghongdianzi.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wz.muxihuayi.cn

[R37] 把输出赋给变量
来源：http://qw.haigaiapp.cn

files=$(ls -1)
来源：http://jd.huanxung.cn

[R38] 管道串联
来源：http://vh.gzmigu.cn

cat a.txt | grep -i error | wc -l
来源：http://fz.shtwfgs.cn

[R39] 重定向标准输出与错误
来源：http://ec.nszjky.cn

cmd > out.log 2>&1
来源：http://ks.9csxet.cn

[R40] 追加写日志
来源：http://id.colortex.cn

echo "log" >> out.log
来源：http://jg.huixiangedu.cn

[R41] 丢弃输出
来源：http://dh.huixinmuqiang.cn

cmd >/dev/null 2>&1
来源：http://ng.521024.cn

[R42] 输入重定向
来源：http://km.nszjky.cn

wc -l < a.txt
来源：http://ku.haigaiapp.cn

[R43] 按名字查找文件
来源：http://sj.521024.cn

find . -name "*.log" -type f
来源：http://vm.haigaiapp.cn

[R44] 按修改时间查找
来源：http://fe.asd995.cn

find . -mtime -7 -type f
来源：http://bb.shxzukj.cn

[R45] 批量删除
来源：http://hp.asd995.cn

find . -name "*.tmp" -delete
来源：http://hb.chemitech.net.cn

[R46] 递归替换文件内容
来源：http://ss.yuexingan06.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ib.521024.cn

[R47] sed 单行替换
来源：http://tr.nszjky.cn

sed -i 's/foo/bar/g' a.txt
来源：http://hj.nszjky.cn

[R48] awk 取指定列
来源：http://hc.nicolike.cn

awk '{print $1, $3}' a.txt
来源：http://bo.shxzskj.cn

[R49] awk 带条件
来源：http://gb.hahajie.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://xq.bjjhwx.cn

[R50] awk 求和
来源：http://rd.szsharing.cn

awk '{s += $2} END {print s}' a.txt
来源：http://ez.yuexingan06.cn

[R51] 排序去重取前几
来源：http://hp.gzmigu.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://oe.shxzukj.cn

[R52] 统计行数
来源：http://km.huixinmuqiang.cn

wc -l a.txt
来源：http://vg.szxytkj.cn

[R53] 查看文件头与实时尾
来源：http://fq.szxytkj.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://cj.9csxet.cn

[R54] 比较两个文件
来源：http://hx.yuexingan06.cn

diff a.txt b.txt
来源：http://me.chemitech.net.cn

[R55] 压缩与解压
来源：http://jb.haigaiapp.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://jx.bookmarksfly.cn

[R56] 远程拷贝
来源：http://vf.hnjuh.cn

scp file user@host:/path/
来源：http://uk.yuexingan06.cn

[R57] 远程执行命令
来源：http://cj.521024.cn

ssh user@host 'uptime'
来源：http://lo.shxzskj.cn

[R58] 下载文件
来源：http://zq.huixinmuqiang.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://pn.colortex.cn

[R59] 发 POST JSON
来源：http://ax.9csxet.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://sg.bookmarksfly.cn

[R60] 只看 HTTP 状态码
来源：http://gx.huanxung.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ri.jianghongdianzi.cn

[R61] 磁盘占用
来源：http://qs.shtwfgs.cn

df -h;  du -sh *
来源：http://bb.huanxung.cn

[R62] 找最占空间的文件
来源：http://ug.bjjhwx.cn

du -ah . | sort -rh | head -10
来源：http://hq.9csxet.cn

[R63] 内存与进程
来源：http://vz.nszjky.cn

free -h;  ps aux | grep nginx
来源：http://tw.szsharing.cn

[R64] 结束进程
来源：http://ds.newstarts.cn

kill -9 $(pgrep -f app.py)
来源：http://rk.huixinmuqiang.cn

[R65] 查看端口占用
来源：http://sv.huixinmuqiang.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://sh.nicolike.cn

[R66] 定时任务
来源：http://vn.huixiangedu.cn

crontab -e;  crontab -l
来源：http://ed.hnjuh.cn

[R67] 生成随机十六进制串
来源：http://fa.szxytkj.cn

openssl rand -hex 16
来源：http://ti.nszjky.cn

[R68] 计算文件校验值
来源：http://yi.9csxet.cn

sha256sum a.txt;  md5sum a.txt
来源：http://is.nicolike.cn

[R69] 生成随机密码
来源：http://xt.jctech888.com.cn

head -c 16 /dev/urandom | base64
来源：http://fi.hnjuh.cn

[R70] 时间戳与互转
来源：http://qg.huixiangedu.cn

date +%s;  date -d @1700000000
来源：http://gz.jctech888.com.cn

[R71] 日期格式化
来源：http://eg.shtwfgs.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://iv.huixinmuqiang.cn

[R72] 等待端口就绪
来源：http://uh.haigaiapp.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://on.shxzukj.cn

[R73] 分割大日志
来源：http://iv.wgjwhj.cn

split -l 1000 big.log part_
来源：http://fp.gzmigu.cn

[R74] 批量重命名
来源：http://cf.yuntaijiaju.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ci.wgjwhj.cn

[R75] 导出环境变量
来源：http://oq.newstarts.cn

export PATH="$HOME/bin:$PATH"
来源：http://bb.panjiajie.cn

[R76] 使用临时文件
来源：http://hs.newstarts.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://xi.nicolike.cn

[R77] 读取用户输入
来源：http://kz.shtwfgs.cn

read -rp "请输入: " ans
来源：http://rw.bjjhwx.cn

[R78] 交互式菜单
来源：http://wo.yuexingan06.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://hd.haigaiapp.cn

[R79] 解析命令行选项
来源：http://ho.huanxung.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wo.muxihuayi.cn

[R80] 查看脚本执行耗时
来源：http://br.gzmigu.cn

time ./run.sh
来源：http://nh.huixinmuqiang.cn

================================================================================
来源：http://me.huixinmuqiang.cn


<!-- 参考信息 -->