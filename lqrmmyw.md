代发 wailian999

[Q38] 全外连接（PostgreSQL）
来源：http://hv.asd995.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://tz.muxihuayi.cn

[Q39] 自连接（查上下级）
来源：http://hz.panjiajie.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://bg.yuntaijiaju.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://gh.huanxung.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://cy.muxihuayi.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://fe.yuntaijiaju.cn

[Q41] 多表连接
来源：http://mk.yuntaijiaju.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://du.shxzukj.cn

JOIN users u ON u.id = o.user_id
来源：http://tr.jianghongdianzi.cn

JOIN products p ON p.id = o.product_id;
来源：http://ak.jianghongdianzi.cn

[Q42] 连接条件附加过滤
来源：http://ep.shxzskj.cn

SELECT u.name, o.amount FROM users u
来源：http://bf.jianghongdianzi.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://pi.gzmigu.cn

[Q43] 标量子查询
来源：http://ky.szsharing.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://pa.521024.cn

[Q44] IN 子查询
来源：http://vw.yuntaijiaju.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://xk.shxzskj.cn

[Q45] EXISTS 判断存在
来源：http://xn.bjjhwx.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://xo.panjiajie.cn

[Q46] NOT EXISTS 判断不存在
来源：http://aw.lnxyls.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://dv.chemitech.net.cn

[Q47] 与平均值比较
来源：http://xm.wgjwhj.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mj.hahajie.cn

[Q48] CTE 公用表表达式
来源：http://ir.huixinmuqiang.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://uw.asd995.cn

SELECT * FROM t WHERE c > 5;
来源：http://nf.hnjuh.cn

[Q49] 更新单行
来源：http://nh.nicolike.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://qf.shxzskj.cn

[Q50] 批量更新
来源：http://kc.9csxet.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://lw.hahajie.cn

[Q51] 用子查询更新
来源：http://cn.szsharing.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://ny.muxihuayi.cn

[Q52] 删除指定行
来源：http://vb.newstarts.cn

DELETE FROM users WHERE id = 10;
来源：http://wv.jianghongdianzi.cn

[Q53] 按条件删除
来源：http://iy.newstarts.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hj.9csxet.cn

[Q54] 清空表
来源：http://cz.yuntaijiaju.cn

TRUNCATE TABLE logs;
来源：http://he.521024.cn

[Q55] 排名（并列占位）
来源：http://wo.chemitech.net.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://la.jctech888.com.cn

[Q56] 密集排名（并列不占位）
来源：http://gj.gzmigu.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://uo.huixinmuqiang.cn

[Q57] 行号
来源：http://ik.huanxung.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://nc.yuexingan06.cn

[Q58] 累计求和
来源：http://bl.szxytkj.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ip.huixinmuqiang.cn

[Q59] 分组内累计
来源：http://oo.521024.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hi.newstarts.cn

[Q60] 取上一行 / 下一行
来源：http://bd.yuntaijiaju.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://bw.szxytkj.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ne.bookmarksfly.cn

[Q61] 移动平均
来源：http://tt.jctech888.com.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://dx.shxzukj.cn

[Q62] 分组占比
来源：http://si.huanxung.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wg.panjiajie.cn

[Q63] 开启事务
来源：http://kp.yuntaijiaju.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://fu.gzmigu.cn

[Q64] 提交事务
来源：http://gb.jctech888.com.cn

COMMIT;
来源：http://vu.nicolike.cn

[Q65] 回滚事务
来源：http://ya.shxzskj.cn

ROLLBACK;
来源：http://zn.jianghongdianzi.cn

[Q66] 行锁查询
来源：http://ln.yuexingan06.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mh.asd995.cn

[Q67] 设置隔离级别
来源：http://wt.szxytkj.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://kl.nicolike.cn

[Q68] 保存点
来源：http://hd.huixiangedu.cn

SAVEPOINT sp1;
来源：http://si.shxzukj.cn

ROLLBACK TO sp1;
来源：http://gt.huixinmuqiang.cn

[Q69] 查看执行计划
来源：http://jj.huanxung.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://he.jctech888.com.cn

[Q70] 更新统计信息
来源：http://rc.bjjhwx.cn

ANALYZE TABLE users;
来源：http://so.yuexingan06.cn

[Q71] 查看建表语句
来源：http://fd.jctech888.com.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ab.muxihuayi.cn

[Q72] 查看索引
来源：http://sd.colortex.cn

SHOW INDEX FROM users;
来源：http://nk.9csxet.cn

[Q73] 查看表状态
来源：http://ef.wgjwhj.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://ty.hnjuh.cn

[Q74] 强制使用索引
来源：http://za.gzmigu.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://oa.lnxyls.cn

[Q75] 日期格式化
来源：http://er.yuexingan06.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://lp.bookmarksfly.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hl.huixinmuqiang.cn

[Q76] 按天统计
来源：http://nl.szxytkj.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://fi.bjjhwx.cn

[Q77] 时间加减
来源：http://iz.bookmarksfly.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://gn.chemitech.net.cn

[Q78] 当前时间
来源：http://hi.shtwfgs.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://yp.colortex.cn

[Q79] 字符串拼接
来源：http://qk.yuexingan06.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://og.hahajie.cn

[Q80] 字符串截取
来源：http://bd.jianghongdianzi.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://te.hnjuh.cn

[Q81] 字符串替换
来源：http://xv.muxihuayi.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ui.muxihuayi.cn

[Q82] 字符长度与字节长度
来源：http://to.bjjhwx.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mz.szsharing.cn

[Q83] 大小写转换
来源：http://zx.shxzukj.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ac.wgjwhj.cn

[Q84] 去除首尾空格
来源：http://gf.wgjwhj.cn

SELECT TRIM(name) FROM users;
来源：http://ne.szsharing.cn

[Q85] 数值取整
来源：http://sn.haigaiapp.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://xt.muxihuayi.cn

[Q86] 读取 JSON 字段
来源：http://bc.haigaiapp.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://dc.szsharing.cn

[Q87] JSON 字段做条件
来源：http://sq.9csxet.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://kd.panjiajie.cn

[Q88] 行转列（条件聚合）
来源：http://cg.szxytkj.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://le.shtwfgs.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://lw.yuexingan06.cn

[Q89] 判断表是否存在
来源：http://qg.shxzukj.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://gb.nicolike.cn

[Q90] 生成序号列
来源：http://tq.hahajie.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ja.jctech888.com.cn

================================================================================
来源：http://nm.newstarts.cn

R. Bash 专题
来源：http://xp.jianghongdianzi.cn

================================================================================
来源：http://fi.haigaiapp.cn

[R01] shebang 与严格模式
来源：http://mu.gzmigu.cn

#!/usr/bin/env bash
来源：http://kk.nszjky.cn

set -euo pipefail
来源：http://os.bookmarksfly.cn

[R02] 变量赋值与使用
来源：http://zd.jctech888.com.cn

name="Tom"; echo "$name"
来源：http://ke.hnjuh.cn

[R03] 只读变量
来源：http://xq.asd995.cn

readonly PI=3.14
来源：http://hq.yuexingan06.cn

[R04] 位置参数
来源：http://sq.shtwfgs.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://sh.gzmigu.cn

[R05] 参数默认值
来源：http://lh.bjjhwx.cn

name="${1:-default}"
来源：http://kn.hnjuh.cn

[R06] 判断命令是否存在
来源：http://cn.bookmarksfly.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://dg.gzmigu.cn

[R07] if 判断文件
来源：http://rh.asd995.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://yv.wgjwhj.cn

[R08] 数值比较
来源：http://kx.521024.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://xa.szxytkj.cn

[R09] 字符串比较
来源：http://ci.huixinmuqiang.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://kp.bjjhwx.cn

[R10] 正则匹配
来源：http://ey.bookmarksfly.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://nz.huanxung.cn

[R11] case 多分支
来源：http://ms.panjiajie.cn

case "$1" in
来源：http://tq.asd995.cn

start) echo "启动" ;;
来源：http://ra.bjjhwx.cn

stop)  echo "停止" ;;
来源：http://pe.nszjky.cn

*)     echo "未知命令" ;;
来源：http://rd.huixinmuqiang.cn

esac
来源：http://px.shxzskj.cn

[R12] for 遍历文件
来源：http://ze.asd995.cn

for f in *.txt; do echo "$f"; done
来源：http://ai.jctech888.com.cn

[R13] for 计数循环
来源：http://bw.szsharing.cn

for i in {1..10}; do echo "$i"; done
来源：http://li.bjjhwx.cn

[R14] C 风格 for
来源：http://ln.bjjhwx.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://zg.huixinmuqiang.cn

[R15] while 逐行读文件
来源：http://mj.haigaiapp.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://uj.9csxet.cn

[R16] until 等待条件
来源：http://jd.shtwfgs.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://we.asd995.cn

[R17] 数组定义与取值
来源：http://rn.nszjky.cn

arr=(a b c); echo "${arr[0]}"
来源：http://sy.yuntaijiaju.cn

[R18] 遍历数组
来源：http://vc.chemitech.net.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://bi.muxihuayi.cn

[R19] 数组长度
来源：http://vs.shxzukj.cn

echo "${#arr[@]}"
来源：http://gi.hahajie.cn

[R20] 关联数组（字典）
来源：http://vf.jctech888.com.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ey.lnxyls.cn

[R21] 字符串长度
来源：http://gh.newstarts.cn

echo "${#s}"
来源：http://jj.jctech888.com.cn

[R22] 截取子串
来源：http://dt.9csxet.cn

echo "${s:0:5}"
来源：http://ow.shtwfgs.cn

[R23] 字符串替换
来源：http://mu.huixinmuqiang.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://le.shxzukj.cn

[R24] 大小写转换
来源：http://nr.shxzskj.cn

echo "${s^^}"; echo "${s,,}"
来源：http://nv.shtwfgs.cn

[R25] 去后缀 / 去前缀
来源：http://qs.colortex.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://xv.9csxet.cn

[R26] 命令替换
来源：http://vs.huixinmuqiang.cn

now=$(date +%F); echo "$now"
来源：http://zk.asd995.cn

[R27] 算术展开
来源：http://bl.wgjwhj.cn

echo $((1 + 2 * 3))
来源：http://mx.asd995.cn

[R28] 浮点运算
来源：http://zd.hnjuh.cn

echo "scale=2; 10/3" | bc
来源：http://zo.yuexingan06.cn

[R29] 定义函数
来源：http://xs.wgjwhj.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://vx.huixiangedu.cn

[R30] 函数返回状态码
来源：http://an.asd995.cn

f() { return 0; }; f || echo "失败了"
来源：http://ss.lnxyls.cn

[R31] 局部变量
来源：http://pe.panjiajie.cn

f() { local x=1; echo "$x"; }
来源：http://bw.huixinmuqiang.cn

[R32] 参数个数校验
来源：http://ov.huixinmuqiang.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ft.newstarts.cn

[R33] 捕获错误并提示行号
来源：http://zt.muxihuayi.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.521024.cn

[R34] 退出时清理
来源：http://at.521024.cn

trap 'rm -f "$tmp"' EXIT
来源：http://rx.nicolike.cn

[R35] 后台执行并等待
来源：http://rd.bookmarksfly.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://ey.yuntaijiaju.cn

[R36] 并发执行多个任务
来源：http://in.bookmarksfly.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://oh.bjjhwx.cn

[R37] 把输出赋给变量
来源：http://xl.szsharing.cn

files=$(ls -1)
来源：http://qt.nszjky.cn

[R38] 管道串联
来源：http://kz.yuntaijiaju.cn

cat a.txt | grep -i error | wc -l
来源：http://dy.wgjwhj.cn

[R39] 重定向标准输出与错误
来源：http://ko.hnjuh.cn

cmd > out.log 2>&1
来源：http://io.521024.cn

[R40] 追加写日志
来源：http://bu.colortex.cn

echo "log" >> out.log
来源：http://av.lnxyls.cn

[R41] 丢弃输出
来源：http://nq.nicolike.cn

cmd >/dev/null 2>&1
来源：http://la.nicolike.cn

[R42] 输入重定向
来源：http://xq.newstarts.cn

wc -l < a.txt
来源：http://yz.bjjhwx.cn

[R43] 按名字查找文件
来源：http://cf.nicolike.cn

find . -name "*.log" -type f
来源：http://lm.wgjwhj.cn

[R44] 按修改时间查找
来源：http://zd.nicolike.cn

find . -mtime -7 -type f
来源：http://rj.huanxung.cn

[R45] 批量删除
来源：http://wc.9csxet.cn

find . -name "*.tmp" -delete
来源：http://ae.bjjhwx.cn

[R46] 递归替换文件内容
来源：http://rm.gzmigu.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://cq.szsharing.cn

[R47] sed 单行替换
来源：http://lh.szxytkj.cn

sed -i 's/foo/bar/g' a.txt
来源：http://pk.muxihuayi.cn

[R48] awk 取指定列
来源：http://pp.hahajie.cn

awk '{print $1, $3}' a.txt
来源：http://iw.yuntaijiaju.cn

[R49] awk 带条件
来源：http://pg.szxytkj.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://of.colortex.cn

[R50] awk 求和
来源：http://id.bookmarksfly.cn

awk '{s += $2} END {print s}' a.txt
来源：http://ec.bjjhwx.cn

[R51] 排序去重取前几
来源：http://vt.asd995.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://nt.shtwfgs.cn

[R52] 统计行数
来源：http://ev.huixinmuqiang.cn

wc -l a.txt
来源：http://er.wgjwhj.cn

[R53] 查看文件头与实时尾
来源：http://zm.panjiajie.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://po.yuntaijiaju.cn

[R54] 比较两个文件
来源：http://am.muxihuayi.cn

diff a.txt b.txt
来源：http://gu.panjiajie.cn

[R55] 压缩与解压
来源：http://zc.9csxet.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://qx.chemitech.net.cn

[R56] 远程拷贝
来源：http://tm.jianghongdianzi.cn

scp file user@host:/path/
来源：http://aa.hahajie.cn

[R57] 远程执行命令
来源：http://nm.jctech888.com.cn

ssh user@host 'uptime'
来源：http://hd.asd995.cn

[R58] 下载文件
来源：http://is.asd995.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://sq.szxytkj.cn

[R59] 发 POST JSON
来源：http://wb.haigaiapp.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://gl.nicolike.cn

[R60] 只看 HTTP 状态码
来源：http://qr.9csxet.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://fd.huanxung.cn

[R61] 磁盘占用
来源：http://rg.panjiajie.cn

df -h;  du -sh *
来源：http://jb.jianghongdianzi.cn

[R62] 找最占空间的文件
来源：http://hq.newstarts.cn

du -ah . | sort -rh | head -10
来源：http://pi.shxzskj.cn

[R63] 内存与进程
来源：http://gs.haigaiapp.cn

free -h;  ps aux | grep nginx
来源：http://be.hnjuh.cn

[R64] 结束进程
来源：http://wn.bookmarksfly.cn

kill -9 $(pgrep -f app.py)
来源：http://zs.521024.cn

[R65] 查看端口占用
来源：http://ra.yuntaijiaju.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://qm.yuntaijiaju.cn

[R66] 定时任务
来源：http://si.bookmarksfly.cn

crontab -e;  crontab -l
来源：http://vh.newstarts.cn

[R67] 生成随机十六进制串
来源：http://zh.shxzukj.cn

openssl rand -hex 16
来源：http://xa.nszjky.cn

[R68] 计算文件校验值
来源：http://cb.wgjwhj.cn

sha256sum a.txt;  md5sum a.txt
来源：http://th.newstarts.cn

[R69] 生成随机密码
来源：http://zn.huanxung.cn

head -c 16 /dev/urandom | base64
来源：http://cj.newstarts.cn

[R70] 时间戳与互转
来源：http://pw.huanxung.cn

date +%s;  date -d @1700000000
来源：http://xc.panjiajie.cn

[R71] 日期格式化
来源：http://pi.9csxet.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://eh.panjiajie.cn

[R72] 等待端口就绪
来源：http://dr.szsharing.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://vl.muxihuayi.cn

[R73] 分割大日志
来源：http://pm.muxihuayi.cn

split -l 1000 big.log part_
来源：http://aq.huanxung.cn

[R74] 批量重命名
来源：http://sx.shtwfgs.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ek.asd995.cn

[R75] 导出环境变量
来源：http://jk.shxzukj.cn

export PATH="$HOME/bin:$PATH"
来源：http://ys.muxihuayi.cn

[R76] 使用临时文件
来源：http://rb.chemitech.net.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://va.wgjwhj.cn

[R77] 读取用户输入
来源：http://bk.bookmarksfly.cn

read -rp "请输入: " ans
来源：http://ks.nszjky.cn

[R78] 交互式菜单
来源：http://bq.shxzskj.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://vb.jianghongdianzi.cn

[R79] 解析命令行选项
来源：http://si.nicolike.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://sk.shxzukj.cn

[R80] 查看脚本执行耗时
来源：http://qz.hnjuh.cn

time ./run.sh
来源：http://cu.szsharing.cn

================================================================================
来源：http://hs.szsharing.cn

S. C / C++ 专题
来源：http://ox.nszjky.cn

================================================================================
来源：http://aj.newstarts.cn

[S01] C：Hello World
来源：http://om.szsharing.cn

#include <stdio.h>
来源：http://ed.bjjhwx.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://nj.lnxyls.cn

[S02] C：变量与格式化输出
来源：http://pg.yuntaijiaju.cn

int a = 10; printf("%d\n", a);
来源：http://js.yuntaijiaju.cn

[S03] C：读入整数
来源：http://nx.shxzskj.cn

int x; scanf("%d", &x);
来源：http://on.huanxung.cn

[S04] C：字符串复制
来源：http://zk.muxihuayi.cn

char dst[32]; strcpy(dst, "hi");
来源：http://kj.hahajie.cn

[S05] C：字符串长度
来源：http://mu.szxytkj.cn

strlen(s)
来源：http://av.chemitech.net.cn

[S06] C：字符串比较
来源：http://uf.shxzukj.cn

strcmp(a, b) == 0
来源：http://qi.hahajie.cn

[S07] C：数组遍历求和
来源：http://fj.huixinmuqiang.cn


<!-- 参考信息 -->