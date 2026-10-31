代发 wailian999

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://en.asd995.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://gk.panjiajie.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://kl.gzmigu.cn

[Q41] 多表连接
来源：http://re.nszjky.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://sf.huixinmuqiang.cn

JOIN users u ON u.id = o.user_id
来源：http://uv.shtwfgs.cn

JOIN products p ON p.id = o.product_id;
来源：http://ft.hnjuh.cn

[Q42] 连接条件附加过滤
来源：http://ib.jctech888.com.cn

SELECT u.name, o.amount FROM users u
来源：http://qz.chemitech.net.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ig.bjjhwx.cn

[Q43] 标量子查询
来源：http://cb.nszjky.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://yu.shxzukj.cn

[Q44] IN 子查询
来源：http://ew.colortex.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://yk.huixinmuqiang.cn

[Q45] EXISTS 判断存在
来源：http://nv.hnjuh.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ve.bookmarksfly.cn

[Q46] NOT EXISTS 判断不存在
来源：http://vb.panjiajie.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://gd.wgjwhj.cn

[Q47] 与平均值比较
来源：http://yz.hnjuh.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://bt.huixiangedu.cn

[Q48] CTE 公用表表达式
来源：http://gt.haigaiapp.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ls.haigaiapp.cn

SELECT * FROM t WHERE c > 5;
来源：http://iw.yuexingan06.cn

[Q49] 更新单行
来源：http://gm.newstarts.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://up.lnxyls.cn

[Q50] 批量更新
来源：http://yj.colortex.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://sz.chemitech.net.cn

[Q51] 用子查询更新
来源：http://gl.huixinmuqiang.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://yh.hahajie.cn

[Q52] 删除指定行
来源：http://qs.panjiajie.cn

DELETE FROM users WHERE id = 10;
来源：http://dk.colortex.cn

[Q53] 按条件删除
来源：http://eb.jctech888.com.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ot.chemitech.net.cn

[Q54] 清空表
来源：http://oc.panjiajie.cn

TRUNCATE TABLE logs;
来源：http://dn.jctech888.com.cn

[Q55] 排名（并列占位）
来源：http://hz.huanxung.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://md.wgjwhj.cn

[Q56] 密集排名（并列不占位）
来源：http://tw.huanxung.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ot.asd995.cn

[Q57] 行号
来源：http://sx.haigaiapp.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://qm.jianghongdianzi.cn

[Q58] 累计求和
来源：http://gk.bjjhwx.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hf.shtwfgs.cn

[Q59] 分组内累计
来源：http://xw.chemitech.net.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://oh.szxytkj.cn

[Q60] 取上一行 / 下一行
来源：http://wx.bookmarksfly.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ln.shtwfgs.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://gg.huanxung.cn

[Q61] 移动平均
来源：http://ba.szxytkj.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://rb.gzmigu.cn

[Q62] 分组占比
来源：http://hq.yuexingan06.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hn.9csxet.cn

[Q63] 开启事务
来源：http://qw.huixiangedu.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://zu.asd995.cn

[Q64] 提交事务
来源：http://uk.muxihuayi.cn

COMMIT;
来源：http://nf.colortex.cn

[Q65] 回滚事务
来源：http://fn.huixinmuqiang.cn

ROLLBACK;
来源：http://kd.muxihuayi.cn

[Q66] 行锁查询
来源：http://wr.huixiangedu.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://st.shtwfgs.cn

[Q67] 设置隔离级别
来源：http://pw.521024.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://vo.521024.cn

[Q68] 保存点
来源：http://jn.bookmarksfly.cn

SAVEPOINT sp1;
来源：http://up.shtwfgs.cn

ROLLBACK TO sp1;
来源：http://kh.bjjhwx.cn

[Q69] 查看执行计划
来源：http://gl.chemitech.net.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://qb.shxzukj.cn

[Q70] 更新统计信息
来源：http://nj.shtwfgs.cn

ANALYZE TABLE users;
来源：http://vy.huixinmuqiang.cn

[Q71] 查看建表语句
来源：http://iz.lnxyls.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ev.bookmarksfly.cn

[Q72] 查看索引
来源：http://ju.colortex.cn

SHOW INDEX FROM users;
来源：http://xu.shtwfgs.cn

[Q73] 查看表状态
来源：http://vw.jctech888.com.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://cs.nicolike.cn

[Q74] 强制使用索引
来源：http://km.huixiangedu.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mz.shxzukj.cn

[Q75] 日期格式化
来源：http://px.szsharing.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ky.hnjuh.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://zz.jctech888.com.cn

[Q76] 按天统计
来源：http://qp.bjjhwx.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://yt.asd995.cn

[Q77] 时间加减
来源：http://pz.haigaiapp.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ev.9csxet.cn

[Q78] 当前时间
来源：http://kl.huixiangedu.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wd.gzmigu.cn

[Q79] 字符串拼接
来源：http://or.szsharing.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://os.muxihuayi.cn

[Q80] 字符串截取
来源：http://rz.szxytkj.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://yu.huixinmuqiang.cn

[Q81] 字符串替换
来源：http://wd.nicolike.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ni.huixiangedu.cn

[Q82] 字符长度与字节长度
来源：http://fr.haigaiapp.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://sx.yuntaijiaju.cn

[Q83] 大小写转换
来源：http://or.wgjwhj.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://gi.nicolike.cn

[Q84] 去除首尾空格
来源：http://th.nszjky.cn

SELECT TRIM(name) FROM users;
来源：http://dh.haigaiapp.cn

[Q85] 数值取整
来源：http://vn.szxytkj.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ad.9csxet.cn

[Q86] 读取 JSON 字段
来源：http://pf.newstarts.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://su.huixiangedu.cn

[Q87] JSON 字段做条件
来源：http://jq.521024.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://au.9csxet.cn

[Q88] 行转列（条件聚合）
来源：http://yn.szxytkj.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://vn.szsharing.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://nm.nicolike.cn

[Q89] 判断表是否存在
来源：http://vd.szxytkj.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://oa.nicolike.cn

[Q90] 生成序号列
来源：http://io.haigaiapp.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://kb.huanxung.cn

================================================================================
来源：http://lv.jctech888.com.cn

R. Bash 专题
来源：http://uu.lnxyls.cn

================================================================================
来源：http://ld.muxihuayi.cn

[R01] shebang 与严格模式
来源：http://uv.yuexingan06.cn

#!/usr/bin/env bash
来源：http://rw.9csxet.cn

set -euo pipefail
来源：http://or.haigaiapp.cn

[R02] 变量赋值与使用
来源：http://py.bookmarksfly.cn

name="Tom"; echo "$name"
来源：http://rd.nszjky.cn

[R03] 只读变量
来源：http://jf.newstarts.cn

readonly PI=3.14
来源：http://sq.chemitech.net.cn

[R04] 位置参数
来源：http://rz.szxytkj.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://sv.huixinmuqiang.cn

[R05] 参数默认值
来源：http://fz.szsharing.cn

name="${1:-default}"
来源：http://lw.bookmarksfly.cn

[R06] 判断命令是否存在
来源：http://kp.colortex.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ed.szxytkj.cn

[R07] if 判断文件
来源：http://jx.hahajie.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ly.hahajie.cn

[R08] 数值比较
来源：http://lq.yuntaijiaju.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://ex.huixinmuqiang.cn

[R09] 字符串比较
来源：http://qy.haigaiapp.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://by.chemitech.net.cn

[R10] 正则匹配
来源：http://ua.hnjuh.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://oe.newstarts.cn

[R11] case 多分支
来源：http://lk.hnjuh.cn

case "$1" in
来源：http://dr.bjjhwx.cn

start) echo "启动" ;;
来源：http://zt.nszjky.cn

stop)  echo "停止" ;;
来源：http://ne.hahajie.cn

*)     echo "未知命令" ;;
来源：http://mb.shxzukj.cn

esac
来源：http://qn.bjjhwx.cn

[R12] for 遍历文件
来源：http://ca.panjiajie.cn

for f in *.txt; do echo "$f"; done
来源：http://ds.haigaiapp.cn

[R13] for 计数循环
来源：http://ms.huixiangedu.cn

for i in {1..10}; do echo "$i"; done
来源：http://py.wgjwhj.cn

[R14] C 风格 for
来源：http://az.wgjwhj.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ur.bookmarksfly.cn

[R15] while 逐行读文件
来源：http://zc.wgjwhj.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ab.yuexingan06.cn

[R16] until 等待条件
来源：http://jr.newstarts.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hs.huanxung.cn

[R17] 数组定义与取值
来源：http://pt.hnjuh.cn

arr=(a b c); echo "${arr[0]}"
来源：http://jp.panjiajie.cn

[R18] 遍历数组
来源：http://pn.nszjky.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://fw.gzmigu.cn

[R19] 数组长度
来源：http://zu.newstarts.cn

echo "${#arr[@]}"
来源：http://oy.521024.cn

[R20] 关联数组（字典）
来源：http://im.huixinmuqiang.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://pc.yuexingan06.cn

[R21] 字符串长度
来源：http://la.9csxet.cn

echo "${#s}"
来源：http://le.chemitech.net.cn

[R22] 截取子串
来源：http://db.newstarts.cn

echo "${s:0:5}"
来源：http://ym.nszjky.cn

[R23] 字符串替换
来源：http://vo.newstarts.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wl.bookmarksfly.cn

[R24] 大小写转换
来源：http://sy.yuntaijiaju.cn

echo "${s^^}"; echo "${s,,}"
来源：http://xx.muxihuayi.cn

[R25] 去后缀 / 去前缀
来源：http://wa.muxihuayi.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://nz.shxzukj.cn

[R26] 命令替换
来源：http://go.muxihuayi.cn

now=$(date +%F); echo "$now"
来源：http://pe.huanxung.cn

[R27] 算术展开
来源：http://bg.newstarts.cn

echo $((1 + 2 * 3))
来源：http://jq.haigaiapp.cn

[R28] 浮点运算
来源：http://uv.yuexingan06.cn

echo "scale=2; 10/3" | bc
来源：http://jf.asd995.cn

[R29] 定义函数
来源：http://vr.shtwfgs.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://pv.chemitech.net.cn

[R30] 函数返回状态码
来源：http://eb.shxzukj.cn

f() { return 0; }; f || echo "失败了"
来源：http://sg.huixiangedu.cn

[R31] 局部变量
来源：http://vu.newstarts.cn

f() { local x=1; echo "$x"; }
来源：http://vz.shxzukj.cn

[R32] 参数个数校验
来源：http://io.nicolike.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://su.nszjky.cn

[R33] 捕获错误并提示行号
来源：http://td.jctech888.com.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ft.szsharing.cn

[R34] 退出时清理
来源：http://hv.521024.cn

trap 'rm -f "$tmp"' EXIT
来源：http://yl.hnjuh.cn

[R35] 后台执行并等待
来源：http://nw.haigaiapp.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://oj.chemitech.net.cn

[R36] 并发执行多个任务
来源：http://ww.haigaiapp.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://uo.9csxet.cn

[R37] 把输出赋给变量
来源：http://ip.shtwfgs.cn

files=$(ls -1)
来源：http://ox.yuntaijiaju.cn

[R38] 管道串联
来源：http://od.jianghongdianzi.cn

cat a.txt | grep -i error | wc -l
来源：http://tn.shxzskj.cn

[R39] 重定向标准输出与错误
来源：http://lx.bjjhwx.cn

cmd > out.log 2>&1
来源：http://af.9csxet.cn

[R40] 追加写日志
来源：http://rs.jianghongdianzi.cn

echo "log" >> out.log
来源：http://zk.huixiangedu.cn

[R41] 丢弃输出
来源：http://ut.521024.cn

cmd >/dev/null 2>&1
来源：http://xa.huanxung.cn

[R42] 输入重定向
来源：http://hr.yuntaijiaju.cn

wc -l < a.txt
来源：http://wr.yuexingan06.cn

[R43] 按名字查找文件
来源：http://fx.yuntaijiaju.cn

find . -name "*.log" -type f
来源：http://jr.wgjwhj.cn

[R44] 按修改时间查找
来源：http://df.huixiangedu.cn

find . -mtime -7 -type f
来源：http://yr.bjjhwx.cn

[R45] 批量删除
来源：http://zl.huixinmuqiang.cn

find . -name "*.tmp" -delete
来源：http://ji.colortex.cn

[R46] 递归替换文件内容
来源：http://az.panjiajie.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://oj.hnjuh.cn

[R47] sed 单行替换
来源：http://tq.shtwfgs.cn

sed -i 's/foo/bar/g' a.txt
来源：http://tw.nicolike.cn

[R48] awk 取指定列
来源：http://cx.jctech888.com.cn

awk '{print $1, $3}' a.txt
来源：http://bk.huixiangedu.cn

[R49] awk 带条件
来源：http://jz.huixinmuqiang.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mh.huixinmuqiang.cn

[R50] awk 求和
来源：http://sb.huixinmuqiang.cn

awk '{s += $2} END {print s}' a.txt
来源：http://li.huixiangedu.cn

[R51] 排序去重取前几
来源：http://mt.haigaiapp.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://qm.hnjuh.cn

[R52] 统计行数
来源：http://uh.yuexingan06.cn

wc -l a.txt
来源：http://dd.yuexingan06.cn

[R53] 查看文件头与实时尾
来源：http://fp.gzmigu.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://qk.bookmarksfly.cn

[R54] 比较两个文件
来源：http://ws.huixiangedu.cn

diff a.txt b.txt
来源：http://xi.yuntaijiaju.cn

[R55] 压缩与解压
来源：http://yd.huixiangedu.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://fw.asd995.cn

[R56] 远程拷贝
来源：http://uy.huixiangedu.cn

scp file user@host:/path/
来源：http://wq.muxihuayi.cn

[R57] 远程执行命令
来源：http://ay.jianghongdianzi.cn

ssh user@host 'uptime'
来源：http://jl.hnjuh.cn

[R58] 下载文件
来源：http://fz.gzmigu.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ca.chemitech.net.cn

[R59] 发 POST JSON
来源：http://uo.shxzukj.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://cm.hahajie.cn

[R60] 只看 HTTP 状态码
来源：http://dd.lnxyls.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ie.haigaiapp.cn

[R61] 磁盘占用
来源：http://cm.bookmarksfly.cn

df -h;  du -sh *
来源：http://fu.9csxet.cn

[R62] 找最占空间的文件
来源：http://lk.shtwfgs.cn

du -ah . | sort -rh | head -10
来源：http://ha.nszjky.cn

[R63] 内存与进程
来源：http://gs.shtwfgs.cn

free -h;  ps aux | grep nginx
来源：http://qa.nicolike.cn

[R64] 结束进程
来源：http://nu.asd995.cn

kill -9 $(pgrep -f app.py)
来源：http://py.nszjky.cn

[R65] 查看端口占用
来源：http://ax.shxzskj.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://pp.szsharing.cn

[R66] 定时任务
来源：http://lr.shxzukj.cn

crontab -e;  crontab -l
来源：http://qb.jianghongdianzi.cn

[R67] 生成随机十六进制串
来源：http://pq.gzmigu.cn

openssl rand -hex 16
来源：http://pi.yuexingan06.cn

[R68] 计算文件校验值
来源：http://ht.hahajie.cn

sha256sum a.txt;  md5sum a.txt
来源：http://vb.shxzukj.cn

[R69] 生成随机密码
来源：http://fb.hahajie.cn

head -c 16 /dev/urandom | base64
来源：http://sx.hnjuh.cn

[R70] 时间戳与互转
来源：http://mb.muxihuayi.cn

date +%s;  date -d @1700000000
来源：http://hc.gzmigu.cn

[R71] 日期格式化
来源：http://vh.nszjky.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://oe.colortex.cn

[R72] 等待端口就绪
来源：http://ic.huanxung.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://aa.huixiangedu.cn

[R73] 分割大日志
来源：http://bz.9csxet.cn

split -l 1000 big.log part_
来源：http://wj.asd995.cn

[R74] 批量重命名
来源：http://pn.szsharing.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://tb.nszjky.cn

[R75] 导出环境变量
来源：http://yj.lnxyls.cn

export PATH="$HOME/bin:$PATH"
来源：http://cc.shxzskj.cn

[R76] 使用临时文件
来源：http://pa.jctech888.com.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://uk.huixinmuqiang.cn

[R77] 读取用户输入
来源：http://gf.shtwfgs.cn

read -rp "请输入: " ans
来源：http://ou.bjjhwx.cn

[R78] 交互式菜单
来源：http://aj.bjjhwx.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://cl.newstarts.cn

[R79] 解析命令行选项
来源：http://qv.huixiangedu.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://cf.chemitech.net.cn

[R80] 查看脚本执行耗时
来源：http://ay.shtwfgs.cn

time ./run.sh
来源：http://vq.bjjhwx.cn

================================================================================
来源：http://jj.szsharing.cn

S. C / C++ 专题
来源：http://nc.szsharing.cn

================================================================================
来源：http://ao.panjiajie.cn

[S01] C：Hello World
来源：http://mx.bookmarksfly.cn

#include <stdio.h>
来源：http://wc.huixinmuqiang.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://wm.hnjuh.cn

[S02] C：变量与格式化输出
来源：http://wm.haigaiapp.cn

int a = 10; printf("%d\n", a);
来源：http://fd.wgjwhj.cn

[S03] C：读入整数
来源：http://ff.colortex.cn

int x; scanf("%d", &x);
来源：http://ca.bjjhwx.cn

[S04] C：字符串复制
来源：http://vk.szsharing.cn

char dst[32]; strcpy(dst, "hi");
来源：http://lx.huixiangedu.cn

[S05] C：字符串长度
来源：http://ea.bookmarksfly.cn

strlen(s)
来源：http://uj.huixiangedu.cn

[S06] C：字符串比较
来源：http://ji.shtwfgs.cn

strcmp(a, b) == 0
来源：http://ob.shtwfgs.cn

[S07] C：数组遍历求和
来源：http://ui.shtwfgs.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://vs.lnxyls.cn

[S08] C：动态内存分配与释放
来源：http://jo.hahajie.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ev.yuexingan06.cn

[S09] C：结构体定义与初始化
来源：http://el.nicolike.cn


<!-- 参考信息 -->