代发 wailian999

[Q36] 左连接
来源：http://lk.colortex.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://kp.wgjwhj.cn

[Q37] 右连接
来源：http://bw.shxzskj.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://lx.bjjhwx.cn

[Q38] 全外连接（PostgreSQL）
来源：http://dp.huanxung.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://nx.huixinmuqiang.cn

[Q39] 自连接（查上下级）
来源：http://ze.newstarts.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://el.hahajie.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://nc.chemitech.net.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://in.huixinmuqiang.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://uz.lnxyls.cn

[Q41] 多表连接
来源：http://qt.szxytkj.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://jr.shxzskj.cn

JOIN users u ON u.id = o.user_id
来源：http://pl.hnjuh.cn

JOIN products p ON p.id = o.product_id;
来源：http://af.shxzskj.cn

[Q42] 连接条件附加过滤
来源：http://jp.bookmarksfly.cn

SELECT u.name, o.amount FROM users u
来源：http://id.panjiajie.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://gi.muxihuayi.cn

[Q43] 标量子查询
来源：http://nn.colortex.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://en.wgjwhj.cn

[Q44] IN 子查询
来源：http://jr.jctech888.com.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://eu.shtwfgs.cn

[Q45] EXISTS 判断存在
来源：http://id.newstarts.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://kd.gzmigu.cn

[Q46] NOT EXISTS 判断不存在
来源：http://uj.9csxet.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://qt.yuexingan06.cn

[Q47] 与平均值比较
来源：http://ji.shxzukj.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://xy.colortex.cn

[Q48] CTE 公用表表达式
来源：http://za.jctech888.com.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hq.shtwfgs.cn

SELECT * FROM t WHERE c > 5;
来源：http://os.yuntaijiaju.cn

[Q49] 更新单行
来源：http://jb.shtwfgs.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ny.wgjwhj.cn

[Q50] 批量更新
来源：http://bd.asd995.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://dk.huanxung.cn

[Q51] 用子查询更新
来源：http://yh.panjiajie.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://dg.yuexingan06.cn

[Q52] 删除指定行
来源：http://gj.huixiangedu.cn

DELETE FROM users WHERE id = 10;
来源：http://hw.hnjuh.cn

[Q53] 按条件删除
来源：http://fg.nszjky.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ww.huixinmuqiang.cn

[Q54] 清空表
来源：http://ta.wgjwhj.cn

TRUNCATE TABLE logs;
来源：http://qy.yuexingan06.cn

[Q55] 排名（并列占位）
来源：http://of.asd995.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://dy.nicolike.cn

[Q56] 密集排名（并列不占位）
来源：http://fq.gzmigu.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://uq.hnjuh.cn

[Q57] 行号
来源：http://xt.shxzukj.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ar.shxzukj.cn

[Q58] 累计求和
来源：http://kl.nicolike.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://xg.wgjwhj.cn

[Q59] 分组内累计
来源：http://lj.huixiangedu.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://vy.huanxung.cn

[Q60] 取上一行 / 下一行
来源：http://wa.nszjky.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://to.yuexingan06.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://bt.nszjky.cn

[Q61] 移动平均
来源：http://nf.yuexingan06.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://sw.hahajie.cn

[Q62] 分组占比
来源：http://ju.shxzukj.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://fi.newstarts.cn

[Q63] 开启事务
来源：http://at.yuexingan06.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://gy.wgjwhj.cn

[Q64] 提交事务
来源：http://il.shxzukj.cn

COMMIT;
来源：http://kq.huanxung.cn

[Q65] 回滚事务
来源：http://xk.huixinmuqiang.cn

ROLLBACK;
来源：http://vq.hnjuh.cn

[Q66] 行锁查询
来源：http://xk.huixinmuqiang.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://yb.huixinmuqiang.cn

[Q67] 设置隔离级别
来源：http://zm.newstarts.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wr.hahajie.cn

[Q68] 保存点
来源：http://fa.521024.cn

SAVEPOINT sp1;
来源：http://th.gzmigu.cn

ROLLBACK TO sp1;
来源：http://iz.9csxet.cn

[Q69] 查看执行计划
来源：http://lh.9csxet.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wy.yuexingan06.cn

[Q70] 更新统计信息
来源：http://rj.jctech888.com.cn

ANALYZE TABLE users;
来源：http://vk.lnxyls.cn

[Q71] 查看建表语句
来源：http://od.szsharing.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://xe.shxzukj.cn

[Q72] 查看索引
来源：http://zm.lnxyls.cn

SHOW INDEX FROM users;
来源：http://cf.hahajie.cn

[Q73] 查看表状态
来源：http://uh.newstarts.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://ia.huixiangedu.cn

[Q74] 强制使用索引
来源：http://ec.nszjky.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://fj.colortex.cn

[Q75] 日期格式化
来源：http://if.colortex.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ji.wgjwhj.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://oh.9csxet.cn

[Q76] 按天统计
来源：http://hj.jianghongdianzi.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://kb.szxytkj.cn

[Q77] 时间加减
来源：http://lk.panjiajie.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://um.nicolike.cn

[Q78] 当前时间
来源：http://pr.shtwfgs.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://oa.bjjhwx.cn

[Q79] 字符串拼接
来源：http://xt.huixiangedu.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://zw.shxzskj.cn

[Q80] 字符串截取
来源：http://zi.shxzukj.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://rn.huanxung.cn

[Q81] 字符串替换
来源：http://xx.szsharing.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://sl.shxzukj.cn

[Q82] 字符长度与字节长度
来源：http://wj.bjjhwx.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://pv.chemitech.net.cn

[Q83] 大小写转换
来源：http://ts.newstarts.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ly.shtwfgs.cn

[Q84] 去除首尾空格
来源：http://zb.yuexingan06.cn

SELECT TRIM(name) FROM users;
来源：http://ch.521024.cn

[Q85] 数值取整
来源：http://ef.gzmigu.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://kv.jctech888.com.cn

[Q86] 读取 JSON 字段
来源：http://dm.shtwfgs.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://sh.wgjwhj.cn

[Q87] JSON 字段做条件
来源：http://ki.hahajie.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ux.yuntaijiaju.cn

[Q88] 行转列（条件聚合）
来源：http://sa.gzmigu.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://kh.shxzskj.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://rr.bookmarksfly.cn

[Q89] 判断表是否存在
来源：http://nx.szxytkj.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ch.newstarts.cn

[Q90] 生成序号列
来源：http://zs.panjiajie.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://li.huixiangedu.cn

================================================================================
来源：http://ha.yuexingan06.cn

R. Bash 专题
来源：http://rv.chemitech.net.cn

================================================================================
来源：http://sn.yuexingan06.cn

[R01] shebang 与严格模式
来源：http://gp.newstarts.cn

#!/usr/bin/env bash
来源：http://vb.muxihuayi.cn

set -euo pipefail
来源：http://ts.lnxyls.cn

[R02] 变量赋值与使用
来源：http://dm.asd995.cn

name="Tom"; echo "$name"
来源：http://jd.chemitech.net.cn

[R03] 只读变量
来源：http://um.9csxet.cn

readonly PI=3.14
来源：http://ix.hnjuh.cn

[R04] 位置参数
来源：http://tl.jianghongdianzi.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://lg.haigaiapp.cn

[R05] 参数默认值
来源：http://um.wgjwhj.cn

name="${1:-default}"
来源：http://ys.huanxung.cn

[R06] 判断命令是否存在
来源：http://xs.huanxung.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://yp.chemitech.net.cn

[R07] if 判断文件
来源：http://mo.bjjhwx.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mo.szxytkj.cn

[R08] 数值比较
来源：http://hq.9csxet.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://hf.yuexingan06.cn

[R09] 字符串比较
来源：http://ml.panjiajie.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ro.shxzukj.cn

[R10] 正则匹配
来源：http://ug.huixinmuqiang.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://pf.bookmarksfly.cn

[R11] case 多分支
来源：http://an.bookmarksfly.cn

case "$1" in
来源：http://lf.bookmarksfly.cn

start) echo "启动" ;;
来源：http://qp.gzmigu.cn

stop)  echo "停止" ;;
来源：http://on.hahajie.cn

*)     echo "未知命令" ;;
来源：http://ud.chemitech.net.cn

esac
来源：http://xg.huixinmuqiang.cn

[R12] for 遍历文件
来源：http://hs.521024.cn

for f in *.txt; do echo "$f"; done
来源：http://zk.shxzukj.cn

[R13] for 计数循环
来源：http://ka.bookmarksfly.cn

for i in {1..10}; do echo "$i"; done
来源：http://nc.panjiajie.cn

[R14] C 风格 for
来源：http://db.asd995.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://pb.muxihuayi.cn

[R15] while 逐行读文件
来源：http://pt.521024.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://og.colortex.cn

[R16] until 等待条件
来源：http://fy.szxytkj.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://pi.yuntaijiaju.cn

[R17] 数组定义与取值
来源：http://xg.newstarts.cn

arr=(a b c); echo "${arr[0]}"
来源：http://vc.9csxet.cn

[R18] 遍历数组
来源：http://za.jctech888.com.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wz.huanxung.cn

[R19] 数组长度
来源：http://ds.nicolike.cn

echo "${#arr[@]}"
来源：http://aa.panjiajie.cn

[R20] 关联数组（字典）
来源：http://qt.szxytkj.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ef.9csxet.cn

[R21] 字符串长度
来源：http://ik.jctech888.com.cn

echo "${#s}"
来源：http://yt.521024.cn

[R22] 截取子串
来源：http://mq.szsharing.cn

echo "${s:0:5}"
来源：http://yz.bjjhwx.cn

[R23] 字符串替换
来源：http://nh.panjiajie.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://gd.hnjuh.cn

[R24] 大小写转换
来源：http://ai.huanxung.cn

echo "${s^^}"; echo "${s,,}"
来源：http://du.lnxyls.cn

[R25] 去后缀 / 去前缀
来源：http://th.bookmarksfly.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://qv.huixiangedu.cn

[R26] 命令替换
来源：http://jv.chemitech.net.cn

now=$(date +%F); echo "$now"
来源：http://ec.bjjhwx.cn

[R27] 算术展开
来源：http://nx.haigaiapp.cn

echo $((1 + 2 * 3))
来源：http://so.9csxet.cn

[R28] 浮点运算
来源：http://za.huixinmuqiang.cn

echo "scale=2; 10/3" | bc
来源：http://ue.szxytkj.cn

[R29] 定义函数
来源：http://mu.nszjky.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://pu.9csxet.cn

[R30] 函数返回状态码
来源：http://rc.huixiangedu.cn

f() { return 0; }; f || echo "失败了"
来源：http://pf.huixinmuqiang.cn

[R31] 局部变量
来源：http://nf.panjiajie.cn

f() { local x=1; echo "$x"; }
来源：http://kg.asd995.cn

[R32] 参数个数校验
来源：http://dt.wgjwhj.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://yz.jianghongdianzi.cn

[R33] 捕获错误并提示行号
来源：http://lg.yuntaijiaju.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://op.wgjwhj.cn

[R34] 退出时清理
来源：http://ha.szsharing.cn

trap 'rm -f "$tmp"' EXIT
来源：http://lf.bjjhwx.cn

[R35] 后台执行并等待
来源：http://jg.hahajie.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://xy.shtwfgs.cn

[R36] 并发执行多个任务
来源：http://ee.panjiajie.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://uj.9csxet.cn

[R37] 把输出赋给变量
来源：http://zp.panjiajie.cn

files=$(ls -1)
来源：http://ba.huixiangedu.cn

[R38] 管道串联
来源：http://tf.hnjuh.cn

cat a.txt | grep -i error | wc -l
来源：http://op.shxzskj.cn

[R39] 重定向标准输出与错误
来源：http://hp.hahajie.cn

cmd > out.log 2>&1
来源：http://om.chemitech.net.cn

[R40] 追加写日志
来源：http://jk.asd995.cn

echo "log" >> out.log
来源：http://eb.huanxung.cn

[R41] 丢弃输出
来源：http://nk.jctech888.com.cn

cmd >/dev/null 2>&1
来源：http://fj.9csxet.cn

[R42] 输入重定向
来源：http://ma.chemitech.net.cn

wc -l < a.txt
来源：http://qg.shtwfgs.cn

[R43] 按名字查找文件
来源：http://hb.panjiajie.cn

find . -name "*.log" -type f
来源：http://gb.yuexingan06.cn

[R44] 按修改时间查找
来源：http://xc.hahajie.cn

find . -mtime -7 -type f
来源：http://wf.hahajie.cn

[R45] 批量删除
来源：http://fh.lnxyls.cn

find . -name "*.tmp" -delete
来源：http://jq.9csxet.cn

[R46] 递归替换文件内容
来源：http://vn.jctech888.com.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://cr.haigaiapp.cn

[R47] sed 单行替换
来源：http://wa.colortex.cn

sed -i 's/foo/bar/g' a.txt
来源：http://nn.nszjky.cn

[R48] awk 取指定列
来源：http://pv.szsharing.cn

awk '{print $1, $3}' a.txt
来源：http://jv.yuexingan06.cn

[R49] awk 带条件
来源：http://ro.jctech888.com.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://pw.shxzskj.cn

[R50] awk 求和
来源：http://li.huanxung.cn

awk '{s += $2} END {print s}' a.txt
来源：http://uv.bookmarksfly.cn

[R51] 排序去重取前几
来源：http://ug.huixinmuqiang.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://zq.huixinmuqiang.cn

[R52] 统计行数
来源：http://zw.521024.cn

wc -l a.txt
来源：http://km.gzmigu.cn

[R53] 查看文件头与实时尾
来源：http://rv.huanxung.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ho.9csxet.cn

[R54] 比较两个文件
来源：http://nu.gzmigu.cn

diff a.txt b.txt
来源：http://vu.nszjky.cn

[R55] 压缩与解压
来源：http://uk.haigaiapp.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://yf.colortex.cn

[R56] 远程拷贝
来源：http://wv.521024.cn

scp file user@host:/path/
来源：http://oi.hnjuh.cn

[R57] 远程执行命令
来源：http://nh.shxzukj.cn

ssh user@host 'uptime'
来源：http://bq.521024.cn

[R58] 下载文件
来源：http://zc.yuntaijiaju.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ia.nicolike.cn

[R59] 发 POST JSON
来源：http://ku.9csxet.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://qz.yuexingan06.cn

[R60] 只看 HTTP 状态码
来源：http://db.muxihuayi.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://xk.nszjky.cn

[R61] 磁盘占用
来源：http://db.szsharing.cn

df -h;  du -sh *
来源：http://dq.lnxyls.cn

[R62] 找最占空间的文件
来源：http://pl.shxzukj.cn

du -ah . | sort -rh | head -10
来源：http://zs.gzmigu.cn

[R63] 内存与进程
来源：http://oh.shtwfgs.cn

free -h;  ps aux | grep nginx
来源：http://na.hahajie.cn

[R64] 结束进程
来源：http://cl.huixiangedu.cn

kill -9 $(pgrep -f app.py)
来源：http://eh.yuntaijiaju.cn

[R65] 查看端口占用
来源：http://ip.shxzukj.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://tw.muxihuayi.cn

[R66] 定时任务
来源：http://it.colortex.cn

crontab -e;  crontab -l
来源：http://zs.wgjwhj.cn

[R67] 生成随机十六进制串
来源：http://pk.panjiajie.cn

openssl rand -hex 16
来源：http://se.shxzukj.cn

[R68] 计算文件校验值
来源：http://sz.chemitech.net.cn

sha256sum a.txt;  md5sum a.txt
来源：http://bd.jctech888.com.cn

[R69] 生成随机密码
来源：http://bp.panjiajie.cn

head -c 16 /dev/urandom | base64
来源：http://av.haigaiapp.cn

[R70] 时间戳与互转
来源：http://pz.jctech888.com.cn

date +%s;  date -d @1700000000
来源：http://lm.wgjwhj.cn

[R71] 日期格式化
来源：http://vi.huanxung.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://av.bjjhwx.cn

[R72] 等待端口就绪
来源：http://vk.jianghongdianzi.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://mx.shtwfgs.cn

[R73] 分割大日志
来源：http://kn.wgjwhj.cn

split -l 1000 big.log part_
来源：http://bw.hahajie.cn

[R74] 批量重命名
来源：http://ma.huixinmuqiang.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://if.huixinmuqiang.cn

[R75] 导出环境变量
来源：http://wd.jctech888.com.cn

export PATH="$HOME/bin:$PATH"
来源：http://ze.jianghongdianzi.cn

[R76] 使用临时文件
来源：http://kx.hnjuh.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://pf.shxzukj.cn

[R77] 读取用户输入
来源：http://fd.nszjky.cn

read -rp "请输入: " ans
来源：http://nf.nszjky.cn

[R78] 交互式菜单
来源：http://kq.jianghongdianzi.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://tl.huixiangedu.cn

[R79] 解析命令行选项
来源：http://mk.jianghongdianzi.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://nz.jctech888.com.cn

[R80] 查看脚本执行耗时
来源：http://bs.newstarts.cn

time ./run.sh
来源：http://co.yuntaijiaju.cn

================================================================================
来源：http://kl.jctech888.com.cn

S. C / C++ 专题
来源：http://dm.gzmigu.cn

================================================================================
来源：http://qk.muxihuayi.cn

[S01] C：Hello World
来源：http://zz.newstarts.cn

#include <stdio.h>
来源：http://lz.muxihuayi.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://il.bookmarksfly.cn

[S02] C：变量与格式化输出
来源：http://ny.hahajie.cn

int a = 10; printf("%d\n", a);
来源：http://kj.shxzskj.cn

[S03] C：读入整数
来源：http://rt.wgjwhj.cn

int x; scanf("%d", &x);
来源：http://ch.szsharing.cn

[S04] C：字符串复制
来源：http://xd.shxzukj.cn

char dst[32]; strcpy(dst, "hi");
来源：http://xx.huanxung.cn

[S05] C：字符串长度
来源：http://sg.jianghongdianzi.cn


<!-- 参考信息 -->