代发 wailian999

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hk.huixiangedu.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://es.jctech888.com.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://rw.9csxet.cn

[Q41] 多表连接
来源：http://fc.haigaiapp.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://nx.shxzukj.cn

JOIN users u ON u.id = o.user_id
来源：http://vz.gzmigu.cn

JOIN products p ON p.id = o.product_id;
来源：http://xb.hnjuh.cn

[Q42] 连接条件附加过滤
来源：http://fe.lnxyls.cn

SELECT u.name, o.amount FROM users u
来源：http://xp.bookmarksfly.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ca.wgjwhj.cn

[Q43] 标量子查询
来源：http://kl.szsharing.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://zu.9csxet.cn

[Q44] IN 子查询
来源：http://ec.nicolike.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ou.shxzukj.cn

[Q45] EXISTS 判断存在
来源：http://ma.9csxet.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://lh.hnjuh.cn

[Q46] NOT EXISTS 判断不存在
来源：http://vt.hnjuh.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://lh.jianghongdianzi.cn

[Q47] 与平均值比较
来源：http://lq.colortex.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://gj.yuexingan06.cn

[Q48] CTE 公用表表达式
来源：http://ok.bookmarksfly.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://bh.lnxyls.cn

SELECT * FROM t WHERE c > 5;
来源：http://ow.bjjhwx.cn

[Q49] 更新单行
来源：http://yp.colortex.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://vy.huanxung.cn

[Q50] 批量更新
来源：http://hh.jianghongdianzi.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://dc.haigaiapp.cn

[Q51] 用子查询更新
来源：http://wn.gzmigu.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://gy.huanxung.cn

[Q52] 删除指定行
来源：http://gc.shxzskj.cn

DELETE FROM users WHERE id = 10;
来源：http://ni.panjiajie.cn

[Q53] 按条件删除
来源：http://ar.jctech888.com.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://qu.hnjuh.cn

[Q54] 清空表
来源：http://ap.lnxyls.cn

TRUNCATE TABLE logs;
来源：http://ky.jctech888.com.cn

[Q55] 排名（并列占位）
来源：http://md.huixinmuqiang.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://rr.hahajie.cn

[Q56] 密集排名（并列不占位）
来源：http://oz.huanxung.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://va.huanxung.cn

[Q57] 行号
来源：http://gz.wgjwhj.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://td.yuntaijiaju.cn

[Q58] 累计求和
来源：http://de.nszjky.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ch.szxytkj.cn

[Q59] 分组内累计
来源：http://lq.9csxet.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://uj.nicolike.cn

[Q60] 取上一行 / 下一行
来源：http://kv.hnjuh.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://vu.colortex.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://bg.bjjhwx.cn

[Q61] 移动平均
来源：http://do.bjjhwx.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://im.chemitech.net.cn

[Q62] 分组占比
来源：http://gk.shtwfgs.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://tk.lnxyls.cn

[Q63] 开启事务
来源：http://nm.shxzukj.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://ef.wgjwhj.cn

[Q64] 提交事务
来源：http://iz.newstarts.cn

COMMIT;
来源：http://lq.szxytkj.cn

[Q65] 回滚事务
来源：http://yl.huanxung.cn

ROLLBACK;
来源：http://ox.521024.cn

[Q66] 行锁查询
来源：http://cr.haigaiapp.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mb.haigaiapp.cn

[Q67] 设置隔离级别
来源：http://jq.huanxung.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://cr.yuexingan06.cn

[Q68] 保存点
来源：http://xv.colortex.cn

SAVEPOINT sp1;
来源：http://xb.lnxyls.cn

ROLLBACK TO sp1;
来源：http://yr.jianghongdianzi.cn

[Q69] 查看执行计划
来源：http://gt.yuexingan06.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://kx.haigaiapp.cn

[Q70] 更新统计信息
来源：http://fj.huixinmuqiang.cn

ANALYZE TABLE users;
来源：http://xe.wgjwhj.cn

[Q71] 查看建表语句
来源：http://do.bookmarksfly.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ie.yuexingan06.cn

[Q72] 查看索引
来源：http://ez.shxzukj.cn

SHOW INDEX FROM users;
来源：http://bi.muxihuayi.cn

[Q73] 查看表状态
来源：http://it.bookmarksfly.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://qo.haigaiapp.cn

[Q74] 强制使用索引
来源：http://mq.yuexingan06.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://pa.huanxung.cn

[Q75] 日期格式化
来源：http://za.panjiajie.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hp.colortex.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wy.jianghongdianzi.cn

[Q76] 按天统计
来源：http://pl.newstarts.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ux.huixiangedu.cn

[Q77] 时间加减
来源：http://xa.9csxet.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hj.shxzskj.cn

[Q78] 当前时间
来源：http://ow.shtwfgs.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://tk.yuntaijiaju.cn

[Q79] 字符串拼接
来源：http://zh.shxzukj.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ck.nszjky.cn

[Q80] 字符串截取
来源：http://pn.bookmarksfly.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://cc.haigaiapp.cn

[Q81] 字符串替换
来源：http://cb.huixinmuqiang.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://dq.szxytkj.cn

[Q82] 字符长度与字节长度
来源：http://db.hnjuh.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ya.jctech888.com.cn

[Q83] 大小写转换
来源：http://kr.bjjhwx.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://tq.newstarts.cn

[Q84] 去除首尾空格
来源：http://qb.szsharing.cn

SELECT TRIM(name) FROM users;
来源：http://op.nszjky.cn

[Q85] 数值取整
来源：http://jt.colortex.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://sa.hnjuh.cn

[Q86] 读取 JSON 字段
来源：http://lt.hnjuh.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://uu.yuntaijiaju.cn

[Q87] JSON 字段做条件
来源：http://rl.muxihuayi.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://od.nszjky.cn

[Q88] 行转列（条件聚合）
来源：http://lu.jianghongdianzi.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wk.szxytkj.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ok.szxytkj.cn

[Q89] 判断表是否存在
来源：http://yc.bookmarksfly.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://og.wgjwhj.cn

[Q90] 生成序号列
来源：http://ab.haigaiapp.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://gb.hahajie.cn

================================================================================
来源：http://ej.asd995.cn

R. Bash 专题
来源：http://ug.shtwfgs.cn

================================================================================
来源：http://wj.szsharing.cn

[R01] shebang 与严格模式
来源：http://dh.chemitech.net.cn

#!/usr/bin/env bash
来源：http://sj.shxzukj.cn

set -euo pipefail
来源：http://fj.jianghongdianzi.cn

[R02] 变量赋值与使用
来源：http://qk.wgjwhj.cn

name="Tom"; echo "$name"
来源：http://rp.shxzskj.cn

[R03] 只读变量
来源：http://hr.panjiajie.cn

readonly PI=3.14
来源：http://ab.huixiangedu.cn

[R04] 位置参数
来源：http://nd.shxzukj.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://da.yuexingan06.cn

[R05] 参数默认值
来源：http://jw.jctech888.com.cn

name="${1:-default}"
来源：http://vb.huixinmuqiang.cn

[R06] 判断命令是否存在
来源：http://pq.yuntaijiaju.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://cd.yuntaijiaju.cn

[R07] if 判断文件
来源：http://ji.shtwfgs.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ez.jctech888.com.cn

[R08] 数值比较
来源：http://xr.yuexingan06.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://hm.hahajie.cn

[R09] 字符串比较
来源：http://bs.chemitech.net.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ol.bookmarksfly.cn

[R10] 正则匹配
来源：http://zh.shtwfgs.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hn.521024.cn

[R11] case 多分支
来源：http://ct.newstarts.cn

case "$1" in
来源：http://kp.huanxung.cn

start) echo "启动" ;;
来源：http://xb.muxihuayi.cn

stop)  echo "停止" ;;
来源：http://vc.nicolike.cn

*)     echo "未知命令" ;;
来源：http://gj.521024.cn

esac
来源：http://ns.shxzskj.cn

[R12] for 遍历文件
来源：http://pr.yuexingan06.cn

for f in *.txt; do echo "$f"; done
来源：http://nq.muxihuayi.cn

[R13] for 计数循环
来源：http://ng.nicolike.cn

for i in {1..10}; do echo "$i"; done
来源：http://uq.nszjky.cn

[R14] C 风格 for
来源：http://xt.jctech888.com.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://cp.huanxung.cn

[R15] while 逐行读文件
来源：http://bf.9csxet.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://cn.shxzskj.cn

[R16] until 等待条件
来源：http://au.521024.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ml.muxihuayi.cn

[R17] 数组定义与取值
来源：http://sa.szsharing.cn

arr=(a b c); echo "${arr[0]}"
来源：http://ej.bookmarksfly.cn

[R18] 遍历数组
来源：http://kl.jianghongdianzi.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://lu.panjiajie.cn

[R19] 数组长度
来源：http://co.bjjhwx.cn

echo "${#arr[@]}"
来源：http://xw.nszjky.cn

[R20] 关联数组（字典）
来源：http://tw.huixinmuqiang.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ek.bookmarksfly.cn

[R21] 字符串长度
来源：http://lo.panjiajie.cn

echo "${#s}"
来源：http://ot.hahajie.cn

[R22] 截取子串
来源：http://tt.nicolike.cn

echo "${s:0:5}"
来源：http://gh.chemitech.net.cn

[R23] 字符串替换
来源：http://gc.haigaiapp.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://io.szxytkj.cn

[R24] 大小写转换
来源：http://tg.jctech888.com.cn

echo "${s^^}"; echo "${s,,}"
来源：http://wm.szxytkj.cn

[R25] 去后缀 / 去前缀
来源：http://mv.asd995.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://ou.nszjky.cn

[R26] 命令替换
来源：http://bs.shxzukj.cn

now=$(date +%F); echo "$now"
来源：http://fi.521024.cn

[R27] 算术展开
来源：http://al.bookmarksfly.cn

echo $((1 + 2 * 3))
来源：http://ty.hnjuh.cn

[R28] 浮点运算
来源：http://rf.bjjhwx.cn

echo "scale=2; 10/3" | bc
来源：http://pp.nicolike.cn

[R29] 定义函数
来源：http://ya.nicolike.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://pe.jianghongdianzi.cn

[R30] 函数返回状态码
来源：http://yw.nszjky.cn

f() { return 0; }; f || echo "失败了"
来源：http://up.shtwfgs.cn

[R31] 局部变量
来源：http://fl.lnxyls.cn

f() { local x=1; echo "$x"; }
来源：http://vw.bookmarksfly.cn

[R32] 参数个数校验
来源：http://fd.haigaiapp.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ii.nicolike.cn

[R33] 捕获错误并提示行号
来源：http://gj.hahajie.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://qp.hahajie.cn

[R34] 退出时清理
来源：http://hh.panjiajie.cn

trap 'rm -f "$tmp"' EXIT
来源：http://bl.shxzukj.cn

[R35] 后台执行并等待
来源：http://tf.shtwfgs.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://bx.9csxet.cn

[R36] 并发执行多个任务
来源：http://vb.asd995.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://kp.newstarts.cn

[R37] 把输出赋给变量
来源：http://da.szxytkj.cn

files=$(ls -1)
来源：http://ye.asd995.cn

[R38] 管道串联
来源：http://yq.jctech888.com.cn

cat a.txt | grep -i error | wc -l
来源：http://nz.521024.cn

[R39] 重定向标准输出与错误
来源：http://ay.panjiajie.cn

cmd > out.log 2>&1
来源：http://wf.yuexingan06.cn

[R40] 追加写日志
来源：http://ei.colortex.cn

echo "log" >> out.log
来源：http://kn.chemitech.net.cn

[R41] 丢弃输出
来源：http://fk.hnjuh.cn

cmd >/dev/null 2>&1
来源：http://co.bjjhwx.cn

[R42] 输入重定向
来源：http://ed.nszjky.cn

wc -l < a.txt
来源：http://nf.shxzukj.cn

[R43] 按名字查找文件
来源：http://ht.chemitech.net.cn

find . -name "*.log" -type f
来源：http://uu.shxzukj.cn

[R44] 按修改时间查找
来源：http://ds.colortex.cn

find . -mtime -7 -type f
来源：http://ir.9csxet.cn

[R45] 批量删除
来源：http://ja.nicolike.cn

find . -name "*.tmp" -delete
来源：http://ih.lnxyls.cn

[R46] 递归替换文件内容
来源：http://xf.newstarts.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://gj.hnjuh.cn

[R47] sed 单行替换
来源：http://ng.newstarts.cn

sed -i 's/foo/bar/g' a.txt
来源：http://dc.muxihuayi.cn

[R48] awk 取指定列
来源：http://pi.panjiajie.cn

awk '{print $1, $3}' a.txt
来源：http://ad.shxzskj.cn

[R49] awk 带条件
来源：http://uq.lnxyls.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://zs.wgjwhj.cn

[R50] awk 求和
来源：http://nh.yuntaijiaju.cn

awk '{s += $2} END {print s}' a.txt
来源：http://nn.yuntaijiaju.cn

[R51] 排序去重取前几
来源：http://wg.newstarts.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://pd.newstarts.cn

[R52] 统计行数
来源：http://wv.huanxung.cn

wc -l a.txt
来源：http://yu.jctech888.com.cn

[R53] 查看文件头与实时尾
来源：http://fg.jctech888.com.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://oh.shxzskj.cn

[R54] 比较两个文件
来源：http://rr.bjjhwx.cn

diff a.txt b.txt
来源：http://fu.nicolike.cn

[R55] 压缩与解压
来源：http://fj.hnjuh.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://eg.asd995.cn

[R56] 远程拷贝
来源：http://gd.huixiangedu.cn

scp file user@host:/path/
来源：http://rg.shtwfgs.cn

[R57] 远程执行命令
来源：http://fy.jianghongdianzi.cn

ssh user@host 'uptime'
来源：http://rz.nszjky.cn

[R58] 下载文件
来源：http://my.jctech888.com.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ez.wgjwhj.cn

[R59] 发 POST JSON
来源：http://qg.yuntaijiaju.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://lx.jianghongdianzi.cn

[R60] 只看 HTTP 状态码
来源：http://jo.wgjwhj.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://vn.wgjwhj.cn

[R61] 磁盘占用
来源：http://yg.lnxyls.cn

df -h;  du -sh *
来源：http://ag.bjjhwx.cn

[R62] 找最占空间的文件
来源：http://dk.nszjky.cn

du -ah . | sort -rh | head -10
来源：http://hg.nicolike.cn

[R63] 内存与进程
来源：http://gf.bjjhwx.cn

free -h;  ps aux | grep nginx
来源：http://ju.lnxyls.cn

[R64] 结束进程
来源：http://mf.shxzskj.cn

kill -9 $(pgrep -f app.py)
来源：http://ez.521024.cn

[R65] 查看端口占用
来源：http://fq.jianghongdianzi.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://av.muxihuayi.cn

[R66] 定时任务
来源：http://of.bookmarksfly.cn

crontab -e;  crontab -l
来源：http://is.lnxyls.cn

[R67] 生成随机十六进制串
来源：http://jf.jctech888.com.cn

openssl rand -hex 16
来源：http://uq.colortex.cn

[R68] 计算文件校验值
来源：http://au.hahajie.cn

sha256sum a.txt;  md5sum a.txt
来源：http://ot.nszjky.cn

[R69] 生成随机密码
来源：http://ua.hnjuh.cn

head -c 16 /dev/urandom | base64
来源：http://ty.newstarts.cn

[R70] 时间戳与互转
来源：http://pm.asd995.cn

date +%s;  date -d @1700000000
来源：http://uy.szxytkj.cn

[R71] 日期格式化
来源：http://js.shxzskj.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://wp.muxihuayi.cn

[R72] 等待端口就绪
来源：http://aq.huixiangedu.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://de.hahajie.cn

[R73] 分割大日志
来源：http://mi.asd995.cn

split -l 1000 big.log part_
来源：http://re.szsharing.cn

[R74] 批量重命名
来源：http://pu.colortex.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://by.panjiajie.cn

[R75] 导出环境变量
来源：http://vv.shxzskj.cn

export PATH="$HOME/bin:$PATH"
来源：http://kc.huixinmuqiang.cn

[R76] 使用临时文件
来源：http://ef.szsharing.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://fn.nszjky.cn

[R77] 读取用户输入
来源：http://nk.jctech888.com.cn

read -rp "请输入: " ans
来源：http://wo.panjiajie.cn

[R78] 交互式菜单
来源：http://ss.asd995.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://gz.yuexingan06.cn

[R79] 解析命令行选项
来源：http://xn.lnxyls.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://yj.bjjhwx.cn

[R80] 查看脚本执行耗时
来源：http://vv.shxzukj.cn

time ./run.sh
来源：http://lj.wgjwhj.cn

================================================================================
来源：http://kg.shtwfgs.cn

S. C / C++ 专题
来源：http://ur.yuexingan06.cn

================================================================================
来源：http://cl.hnjuh.cn

[S01] C：Hello World
来源：http://xe.colortex.cn

#include <stdio.h>
来源：http://uv.bjjhwx.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://yi.szsharing.cn

[S02] C：变量与格式化输出
来源：http://bj.newstarts.cn

int a = 10; printf("%d\n", a);
来源：http://xr.yuntaijiaju.cn

[S03] C：读入整数
来源：http://vy.panjiajie.cn

int x; scanf("%d", &x);
来源：http://tr.huixiangedu.cn

[S04] C：字符串复制
来源：http://cj.nicolike.cn

char dst[32]; strcpy(dst, "hi");
来源：http://kt.nszjky.cn

[S05] C：字符串长度
来源：http://oo.hnjuh.cn

strlen(s)
来源：http://ql.hahajie.cn

[S06] C：字符串比较
来源：http://wi.panjiajie.cn

strcmp(a, b) == 0
来源：http://if.shxzskj.cn

[S07] C：数组遍历求和
来源：http://en.521024.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ts.jctech888.com.cn

[S08] C：动态内存分配与释放
来源：http://qt.muxihuayi.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://sw.szsharing.cn

[S09] C：结构体定义与初始化
来源：http://zp.shtwfgs.cn


<!-- 参考信息 -->