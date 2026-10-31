代发 wailian999

SELECT o.id, u.name, p.title FROM orders o
来源：http://ef.haigaiapp.cn

JOIN users u ON u.id = o.user_id
来源：http://dr.szsharing.cn

JOIN products p ON p.id = o.product_id;
来源：http://hw.asd995.cn

[Q42] 连接条件附加过滤
来源：http://dm.szsharing.cn

SELECT u.name, o.amount FROM users u
来源：http://vz.yuntaijiaju.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://oe.lnxyls.cn

[Q43] 标量子查询
来源：http://pe.szxytkj.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://kd.huanxung.cn

[Q44] IN 子查询
来源：http://am.hnjuh.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wq.huanxung.cn

[Q45] EXISTS 判断存在
来源：http://lc.lnxyls.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ay.gzmigu.cn

[Q46] NOT EXISTS 判断不存在
来源：http://jz.lnxyls.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://uz.panjiajie.cn

[Q47] 与平均值比较
来源：http://lm.huixiangedu.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://gd.asd995.cn

[Q48] CTE 公用表表达式
来源：http://fm.hnjuh.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://sb.muxihuayi.cn

SELECT * FROM t WHERE c > 5;
来源：http://by.nszjky.cn

[Q49] 更新单行
来源：http://al.gzmigu.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://cf.panjiajie.cn

[Q50] 批量更新
来源：http://xc.haigaiapp.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://zl.shxzukj.cn

[Q51] 用子查询更新
来源：http://jc.szsharing.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://pw.gzmigu.cn

[Q52] 删除指定行
来源：http://ej.muxihuayi.cn

DELETE FROM users WHERE id = 10;
来源：http://cq.panjiajie.cn

[Q53] 按条件删除
来源：http://sp.9csxet.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://bl.wgjwhj.cn

[Q54] 清空表
来源：http://nx.huixiangedu.cn

TRUNCATE TABLE logs;
来源：http://lv.shxzukj.cn

[Q55] 排名（并列占位）
来源：http://zy.nicolike.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://xy.nszjky.cn

[Q56] 密集排名（并列不占位）
来源：http://mb.yuntaijiaju.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://qh.bjjhwx.cn

[Q57] 行号
来源：http://nn.newstarts.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ru.9csxet.cn

[Q58] 累计求和
来源：http://dg.521024.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://gh.shxzukj.cn

[Q59] 分组内累计
来源：http://cu.huanxung.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://vo.gzmigu.cn

[Q60] 取上一行 / 下一行
来源：http://ir.lnxyls.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://yq.shxzukj.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://pd.huixinmuqiang.cn

[Q61] 移动平均
来源：http://yt.gzmigu.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://pu.shtwfgs.cn

[Q62] 分组占比
来源：http://ix.panjiajie.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://rs.chemitech.net.cn

[Q63] 开启事务
来源：http://we.shxzukj.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://mx.yuntaijiaju.cn

[Q64] 提交事务
来源：http://fq.nicolike.cn

COMMIT;
来源：http://ir.shxzukj.cn

[Q65] 回滚事务
来源：http://jv.newstarts.cn

ROLLBACK;
来源：http://mw.panjiajie.cn

[Q66] 行锁查询
来源：http://cp.szxytkj.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://pa.shtwfgs.cn

[Q67] 设置隔离级别
来源：http://nj.muxihuayi.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://fn.nicolike.cn

[Q68] 保存点
来源：http://et.hnjuh.cn

SAVEPOINT sp1;
来源：http://nl.lnxyls.cn

ROLLBACK TO sp1;
来源：http://dc.panjiajie.cn

[Q69] 查看执行计划
来源：http://tj.muxihuayi.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://id.haigaiapp.cn

[Q70] 更新统计信息
来源：http://jh.bookmarksfly.cn

ANALYZE TABLE users;
来源：http://zh.yuexingan06.cn

[Q71] 查看建表语句
来源：http://vl.9csxet.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://tj.shtwfgs.cn

[Q72] 查看索引
来源：http://ha.bookmarksfly.cn

SHOW INDEX FROM users;
来源：http://lj.szxytkj.cn

[Q73] 查看表状态
来源：http://wq.nicolike.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://xj.colortex.cn

[Q74] 强制使用索引
来源：http://pu.shxzskj.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://yi.yuexingan06.cn

[Q75] 日期格式化
来源：http://wq.chemitech.net.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ti.yuntaijiaju.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ro.lnxyls.cn

[Q76] 按天统计
来源：http://rq.lnxyls.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://tp.shxzukj.cn

[Q77] 时间加减
来源：http://tg.jctech888.com.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://nb.jctech888.com.cn

[Q78] 当前时间
来源：http://ms.hnjuh.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ro.wgjwhj.cn

[Q79] 字符串拼接
来源：http://lk.shtwfgs.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://er.huixiangedu.cn

[Q80] 字符串截取
来源：http://bb.nicolike.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://nx.asd995.cn

[Q81] 字符串替换
来源：http://bz.chemitech.net.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://qi.asd995.cn

[Q82] 字符长度与字节长度
来源：http://rg.szsharing.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://cz.panjiajie.cn

[Q83] 大小写转换
来源：http://ts.huixinmuqiang.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mf.huixinmuqiang.cn

[Q84] 去除首尾空格
来源：http://or.huanxung.cn

SELECT TRIM(name) FROM users;
来源：http://mg.haigaiapp.cn

[Q85] 数值取整
来源：http://cm.shxzskj.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ve.colortex.cn

[Q86] 读取 JSON 字段
来源：http://hd.newstarts.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://jg.yuexingan06.cn

[Q87] JSON 字段做条件
来源：http://oh.bjjhwx.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://tr.shtwfgs.cn

[Q88] 行转列（条件聚合）
来源：http://vv.haigaiapp.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://od.gzmigu.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://af.yuntaijiaju.cn

[Q89] 判断表是否存在
来源：http://dx.huixinmuqiang.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://tj.521024.cn

[Q90] 生成序号列
来源：http://ws.panjiajie.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://qd.nszjky.cn

================================================================================
来源：http://lr.szsharing.cn

R. Bash 专题
来源：http://id.chemitech.net.cn

================================================================================
来源：http://qg.jctech888.com.cn

[R01] shebang 与严格模式
来源：http://cd.colortex.cn

#!/usr/bin/env bash
来源：http://vt.szsharing.cn

set -euo pipefail
来源：http://nm.hahajie.cn

[R02] 变量赋值与使用
来源：http://fr.521024.cn

name="Tom"; echo "$name"
来源：http://jp.bookmarksfly.cn

[R03] 只读变量
来源：http://iy.bjjhwx.cn

readonly PI=3.14
来源：http://mn.jianghongdianzi.cn

[R04] 位置参数
来源：http://hc.gzmigu.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://za.szxytkj.cn

[R05] 参数默认值
来源：http://zp.shtwfgs.cn

name="${1:-default}"
来源：http://wr.muxihuayi.cn

[R06] 判断命令是否存在
来源：http://sh.lnxyls.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://av.jctech888.com.cn

[R07] if 判断文件
来源：http://sd.lnxyls.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://yc.shxzskj.cn

[R08] 数值比较
来源：http://au.9csxet.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://yt.jctech888.com.cn

[R09] 字符串比较
来源：http://bu.9csxet.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://vd.hnjuh.cn

[R10] 正则匹配
来源：http://pg.shxzskj.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wo.bookmarksfly.cn

[R11] case 多分支
来源：http://yw.huixiangedu.cn

case "$1" in
来源：http://gg.yuntaijiaju.cn

start) echo "启动" ;;
来源：http://cs.jianghongdianzi.cn

stop)  echo "停止" ;;
来源：http://lc.521024.cn

*)     echo "未知命令" ;;
来源：http://kf.colortex.cn

esac
来源：http://ld.muxihuayi.cn

[R12] for 遍历文件
来源：http://in.jianghongdianzi.cn

for f in *.txt; do echo "$f"; done
来源：http://ap.jianghongdianzi.cn

[R13] for 计数循环
来源：http://mr.nicolike.cn

for i in {1..10}; do echo "$i"; done
来源：http://na.bookmarksfly.cn

[R14] C 风格 for
来源：http://aa.shtwfgs.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://vv.9csxet.cn

[R15] while 逐行读文件
来源：http://we.panjiajie.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://gu.yuntaijiaju.cn

[R16] until 等待条件
来源：http://nk.bookmarksfly.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://dx.chemitech.net.cn

[R17] 数组定义与取值
来源：http://qa.yuexingan06.cn

arr=(a b c); echo "${arr[0]}"
来源：http://rr.yuexingan06.cn

[R18] 遍历数组
来源：http://je.lnxyls.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ju.yuexingan06.cn

[R19] 数组长度
来源：http://ga.lnxyls.cn

echo "${#arr[@]}"
来源：http://wn.huixinmuqiang.cn

[R20] 关联数组（字典）
来源：http://bf.asd995.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://gd.szxytkj.cn

[R21] 字符串长度
来源：http://kg.nszjky.cn

echo "${#s}"
来源：http://yf.szxytkj.cn

[R22] 截取子串
来源：http://cj.huixiangedu.cn

echo "${s:0:5}"
来源：http://cw.yuntaijiaju.cn

[R23] 字符串替换
来源：http://nz.chemitech.net.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://jr.521024.cn

[R24] 大小写转换
来源：http://bx.yuexingan06.cn

echo "${s^^}"; echo "${s,,}"
来源：http://tt.colortex.cn

[R25] 去后缀 / 去前缀
来源：http://vw.panjiajie.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://xv.521024.cn

[R26] 命令替换
来源：http://zv.newstarts.cn

now=$(date +%F); echo "$now"
来源：http://kg.haigaiapp.cn

[R27] 算术展开
来源：http://pv.shtwfgs.cn

echo $((1 + 2 * 3))
来源：http://sw.bjjhwx.cn

[R28] 浮点运算
来源：http://cc.bjjhwx.cn

echo "scale=2; 10/3" | bc
来源：http://af.huanxung.cn

[R29] 定义函数
来源：http://md.jianghongdianzi.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://jz.huixiangedu.cn

[R30] 函数返回状态码
来源：http://zt.huanxung.cn

f() { return 0; }; f || echo "失败了"
来源：http://iz.huixiangedu.cn

[R31] 局部变量
来源：http://hi.bookmarksfly.cn

f() { local x=1; echo "$x"; }
来源：http://xz.huanxung.cn

[R32] 参数个数校验
来源：http://ht.shxzukj.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://as.shtwfgs.cn

[R33] 捕获错误并提示行号
来源：http://xl.szsharing.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ug.wgjwhj.cn

[R34] 退出时清理
来源：http://sg.hnjuh.cn

trap 'rm -f "$tmp"' EXIT
来源：http://gh.huixinmuqiang.cn

[R35] 后台执行并等待
来源：http://xw.panjiajie.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://dv.hahajie.cn

[R36] 并发执行多个任务
来源：http://yz.huixinmuqiang.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://yg.panjiajie.cn

[R37] 把输出赋给变量
来源：http://ud.shxzukj.cn

files=$(ls -1)
来源：http://yc.newstarts.cn

[R38] 管道串联
来源：http://ik.9csxet.cn

cat a.txt | grep -i error | wc -l
来源：http://ir.huanxung.cn

[R39] 重定向标准输出与错误
来源：http://dj.panjiajie.cn

cmd > out.log 2>&1
来源：http://cq.wgjwhj.cn

[R40] 追加写日志
来源：http://km.shxzskj.cn

echo "log" >> out.log
来源：http://pi.huixinmuqiang.cn

[R41] 丢弃输出
来源：http://zy.chemitech.net.cn

cmd >/dev/null 2>&1
来源：http://wr.hahajie.cn

[R42] 输入重定向
来源：http://ex.shxzskj.cn

wc -l < a.txt
来源：http://na.huanxung.cn

[R43] 按名字查找文件
来源：http://ga.shtwfgs.cn

find . -name "*.log" -type f
来源：http://mz.szsharing.cn

[R44] 按修改时间查找
来源：http://la.jctech888.com.cn

find . -mtime -7 -type f
来源：http://vz.szsharing.cn

[R45] 批量删除
来源：http://vr.shxzskj.cn

find . -name "*.tmp" -delete
来源：http://xy.521024.cn

[R46] 递归替换文件内容
来源：http://um.bookmarksfly.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://rd.wgjwhj.cn

[R47] sed 单行替换
来源：http://eo.nszjky.cn

sed -i 's/foo/bar/g' a.txt
来源：http://we.gzmigu.cn

[R48] awk 取指定列
来源：http://ae.bjjhwx.cn

awk '{print $1, $3}' a.txt
来源：http://ge.bookmarksfly.cn

[R49] awk 带条件
来源：http://my.huixinmuqiang.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wb.chemitech.net.cn

[R50] awk 求和
来源：http://cg.jctech888.com.cn

awk '{s += $2} END {print s}' a.txt
来源：http://ry.jctech888.com.cn

[R51] 排序去重取前几
来源：http://nr.nicolike.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://gj.hnjuh.cn

[R52] 统计行数
来源：http://ol.chemitech.net.cn

wc -l a.txt
来源：http://cz.shtwfgs.cn

[R53] 查看文件头与实时尾
来源：http://rz.nicolike.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ou.bjjhwx.cn

[R54] 比较两个文件
来源：http://cm.hahajie.cn

diff a.txt b.txt
来源：http://rf.asd995.cn

[R55] 压缩与解压
来源：http://xu.nszjky.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://gi.hahajie.cn

[R56] 远程拷贝
来源：http://ai.yuntaijiaju.cn

scp file user@host:/path/
来源：http://sh.haigaiapp.cn

[R57] 远程执行命令
来源：http://lw.newstarts.cn

ssh user@host 'uptime'
来源：http://ff.huixinmuqiang.cn

[R58] 下载文件
来源：http://cq.wgjwhj.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://rw.newstarts.cn

[R59] 发 POST JSON
来源：http://im.lnxyls.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://gq.shxzukj.cn

[R60] 只看 HTTP 状态码
来源：http://rh.shxzskj.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://rw.gzmigu.cn

[R61] 磁盘占用
来源：http://ui.yuexingan06.cn

df -h;  du -sh *
来源：http://wl.gzmigu.cn

[R62] 找最占空间的文件
来源：http://ke.newstarts.cn

du -ah . | sort -rh | head -10
来源：http://jx.9csxet.cn

[R63] 内存与进程
来源：http://ac.colortex.cn

free -h;  ps aux | grep nginx
来源：http://th.yuntaijiaju.cn

[R64] 结束进程
来源：http://mc.newstarts.cn

kill -9 $(pgrep -f app.py)
来源：http://on.bjjhwx.cn

[R65] 查看端口占用
来源：http://kn.huixinmuqiang.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://nf.huixinmuqiang.cn

[R66] 定时任务
来源：http://kl.hahajie.cn

crontab -e;  crontab -l
来源：http://fi.newstarts.cn

[R67] 生成随机十六进制串
来源：http://lg.newstarts.cn

openssl rand -hex 16
来源：http://wt.bookmarksfly.cn

[R68] 计算文件校验值
来源：http://bq.yuexingan06.cn

sha256sum a.txt;  md5sum a.txt
来源：http://io.shxzskj.cn

[R69] 生成随机密码
来源：http://qw.huanxung.cn

head -c 16 /dev/urandom | base64
来源：http://aa.521024.cn

[R70] 时间戳与互转
来源：http://xp.yuexingan06.cn

date +%s;  date -d @1700000000
来源：http://qr.jctech888.com.cn

[R71] 日期格式化
来源：http://jy.szsharing.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://lm.huixiangedu.cn

[R72] 等待端口就绪
来源：http://pc.shxzukj.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://kw.bookmarksfly.cn

[R73] 分割大日志
来源：http://os.huixiangedu.cn

split -l 1000 big.log part_
来源：http://ne.newstarts.cn

[R74] 批量重命名
来源：http://md.wgjwhj.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://yj.panjiajie.cn

[R75] 导出环境变量
来源：http://yl.shxzukj.cn

export PATH="$HOME/bin:$PATH"
来源：http://zb.chemitech.net.cn

[R76] 使用临时文件
来源：http://ko.jctech888.com.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://uy.colortex.cn

[R77] 读取用户输入
来源：http://ux.hnjuh.cn

read -rp "请输入: " ans
来源：http://eq.521024.cn

[R78] 交互式菜单
来源：http://un.muxihuayi.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://ow.shtwfgs.cn

[R79] 解析命令行选项
来源：http://zb.gzmigu.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://yb.muxihuayi.cn

[R80] 查看脚本执行耗时
来源：http://ke.nszjky.cn

time ./run.sh
来源：http://gs.panjiajie.cn

================================================================================
来源：http://rf.panjiajie.cn

S. C / C++ 专题
来源：http://nl.hnjuh.cn

================================================================================
来源：http://xz.colortex.cn

[S01] C：Hello World
来源：http://fp.asd995.cn

#include <stdio.h>
来源：http://ji.jianghongdianzi.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://hv.chemitech.net.cn

[S02] C：变量与格式化输出
来源：http://hk.bjjhwx.cn

int a = 10; printf("%d\n", a);
来源：http://zr.lnxyls.cn

[S03] C：读入整数
来源：http://nw.nszjky.cn

int x; scanf("%d", &x);
来源：http://ea.colortex.cn

[S04] C：字符串复制
来源：http://cn.hnjuh.cn

char dst[32]; strcpy(dst, "hi");
来源：http://zn.szxytkj.cn

[S05] C：字符串长度
来源：http://wo.jianghongdianzi.cn

strlen(s)
来源：http://qz.9csxet.cn

[S06] C：字符串比较
来源：http://ji.haigaiapp.cn

strcmp(a, b) == 0
来源：http://jz.nicolike.cn

[S07] C：数组遍历求和
来源：http://fg.newstarts.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ps.panjiajie.cn

[S08] C：动态内存分配与释放
来源：http://kx.chemitech.net.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ys.newstarts.cn

[S09] C：结构体定义与初始化
来源：http://vu.bookmarksfly.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mx.muxihuayi.cn

[S10] C：指针与解引用
来源：http://rw.huixiangedu.cn

int *p = &a;  *p = 5;
来源：http://kf.lnxyls.cn

[S11] C：逐行读文件
来源：http://ei.jctech888.com.cn


<!-- 参考信息 -->