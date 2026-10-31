代发 wailian999

SELECT o.id, u.name, p.title FROM orders o
来源：http://ei.521024.cn

JOIN users u ON u.id = o.user_id
来源：http://qm.nicolike.cn

JOIN products p ON p.id = o.product_id;
来源：http://dp.szsharing.cn

[Q42] 连接条件附加过滤
来源：http://by.szxytkj.cn

SELECT u.name, o.amount FROM users u
来源：http://xd.huixinmuqiang.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hl.521024.cn

[Q43] 标量子查询
来源：http://kc.muxihuayi.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://om.jianghongdianzi.cn

[Q44] IN 子查询
来源：http://nw.shxzskj.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://zh.huixinmuqiang.cn

[Q45] EXISTS 判断存在
来源：http://oj.jianghongdianzi.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://tm.bjjhwx.cn

[Q46] NOT EXISTS 判断不存在
来源：http://px.jianghongdianzi.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hu.muxihuayi.cn

[Q47] 与平均值比较
来源：http://dd.shxzskj.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://at.9csxet.cn

[Q48] CTE 公用表表达式
来源：http://qc.yuntaijiaju.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hq.bjjhwx.cn

SELECT * FROM t WHERE c > 5;
来源：http://ox.asd995.cn

[Q49] 更新单行
来源：http://wy.nszjky.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://yo.yuexingan06.cn

[Q50] 批量更新
来源：http://fg.colortex.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://ex.huixiangedu.cn

[Q51] 用子查询更新
来源：http://sw.huanxung.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://fs.huixinmuqiang.cn

[Q52] 删除指定行
来源：http://dw.newstarts.cn

DELETE FROM users WHERE id = 10;
来源：http://cs.shxzskj.cn

[Q53] 按条件删除
来源：http://jr.panjiajie.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://yt.wgjwhj.cn

[Q54] 清空表
来源：http://ey.asd995.cn

TRUNCATE TABLE logs;
来源：http://ba.chemitech.net.cn

[Q55] 排名（并列占位）
来源：http://io.hnjuh.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://bt.colortex.cn

[Q56] 密集排名（并列不占位）
来源：http://bu.gzmigu.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://zp.muxihuayi.cn

[Q57] 行号
来源：http://wq.jctech888.com.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://cr.huixiangedu.cn

[Q58] 累计求和
来源：http://wd.nszjky.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ra.newstarts.cn

[Q59] 分组内累计
来源：http://sl.9csxet.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://uz.haigaiapp.cn

[Q60] 取上一行 / 下一行
来源：http://ei.jctech888.com.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://dg.panjiajie.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://eo.newstarts.cn

[Q61] 移动平均
来源：http://ig.shxzukj.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://vc.bjjhwx.cn

[Q62] 分组占比
来源：http://ag.lnxyls.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://dm.shxzukj.cn

[Q63] 开启事务
来源：http://fp.bjjhwx.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://yj.shxzskj.cn

[Q64] 提交事务
来源：http://sw.jctech888.com.cn

COMMIT;
来源：http://zs.haigaiapp.cn

[Q65] 回滚事务
来源：http://ra.jctech888.com.cn

ROLLBACK;
来源：http://sp.huixiangedu.cn

[Q66] 行锁查询
来源：http://tg.huanxung.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://lk.gzmigu.cn

[Q67] 设置隔离级别
来源：http://mw.shxzukj.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://li.nicolike.cn

[Q68] 保存点
来源：http://ok.bookmarksfly.cn

SAVEPOINT sp1;
来源：http://wf.nszjky.cn

ROLLBACK TO sp1;
来源：http://mn.huanxung.cn

[Q69] 查看执行计划
来源：http://cu.haigaiapp.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://cn.newstarts.cn

[Q70] 更新统计信息
来源：http://ln.nicolike.cn

ANALYZE TABLE users;
来源：http://pd.bookmarksfly.cn

[Q71] 查看建表语句
来源：http://ul.hahajie.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://jt.bjjhwx.cn

[Q72] 查看索引
来源：http://jv.lnxyls.cn

SHOW INDEX FROM users;
来源：http://zm.colortex.cn

[Q73] 查看表状态
来源：http://ce.hahajie.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://op.huanxung.cn

[Q74] 强制使用索引
来源：http://zs.yuexingan06.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://tl.muxihuayi.cn

[Q75] 日期格式化
来源：http://hb.szsharing.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://pk.haigaiapp.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://eh.shtwfgs.cn

[Q76] 按天统计
来源：http://si.huixiangedu.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ki.newstarts.cn

[Q77] 时间加减
来源：http://xn.szsharing.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://pa.lnxyls.cn

[Q78] 当前时间
来源：http://te.colortex.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://lq.chemitech.net.cn

[Q79] 字符串拼接
来源：http://tm.yuexingan06.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://gj.shtwfgs.cn

[Q80] 字符串截取
来源：http://gb.nicolike.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://zg.9csxet.cn

[Q81] 字符串替换
来源：http://by.gzmigu.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://pp.szsharing.cn

[Q82] 字符长度与字节长度
来源：http://qu.szxytkj.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://fo.huanxung.cn

[Q83] 大小写转换
来源：http://wt.panjiajie.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://xm.wgjwhj.cn

[Q84] 去除首尾空格
来源：http://yp.szsharing.cn

SELECT TRIM(name) FROM users;
来源：http://dq.bookmarksfly.cn

[Q85] 数值取整
来源：http://gj.521024.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hh.wgjwhj.cn

[Q86] 读取 JSON 字段
来源：http://lg.szxytkj.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://cj.lnxyls.cn

[Q87] JSON 字段做条件
来源：http://gj.shxzskj.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://yz.yuntaijiaju.cn

[Q88] 行转列（条件聚合）
来源：http://yi.bjjhwx.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://li.hahajie.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ow.521024.cn

[Q89] 判断表是否存在
来源：http://yj.newstarts.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://kr.haigaiapp.cn

[Q90] 生成序号列
来源：http://mw.huixiangedu.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://pz.muxihuayi.cn

================================================================================
来源：http://fc.bookmarksfly.cn

R. Bash 专题
来源：http://kl.shtwfgs.cn

================================================================================
来源：http://vw.haigaiapp.cn

[R01] shebang 与严格模式
来源：http://jb.shxzskj.cn

#!/usr/bin/env bash
来源：http://aw.hahajie.cn

set -euo pipefail
来源：http://aq.9csxet.cn

[R02] 变量赋值与使用
来源：http://mo.szxytkj.cn

name="Tom"; echo "$name"
来源：http://tw.muxihuayi.cn

[R03] 只读变量
来源：http://pv.lnxyls.cn

readonly PI=3.14
来源：http://wm.jctech888.com.cn

[R04] 位置参数
来源：http://zb.hahajie.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://lv.hahajie.cn

[R05] 参数默认值
来源：http://zy.huixinmuqiang.cn

name="${1:-default}"
来源：http://nk.9csxet.cn

[R06] 判断命令是否存在
来源：http://wk.jianghongdianzi.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://fq.bjjhwx.cn

[R07] if 判断文件
来源：http://qj.newstarts.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://pf.jianghongdianzi.cn

[R08] 数值比较
来源：http://xv.jianghongdianzi.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://jo.huanxung.cn

[R09] 字符串比较
来源：http://mv.nszjky.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mt.wgjwhj.cn

[R10] 正则匹配
来源：http://ow.huixiangedu.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://vq.muxihuayi.cn

[R11] case 多分支
来源：http://gz.haigaiapp.cn

case "$1" in
来源：http://fn.szsharing.cn

start) echo "启动" ;;
来源：http://zw.hahajie.cn

stop)  echo "停止" ;;
来源：http://jn.nszjky.cn

*)     echo "未知命令" ;;
来源：http://bx.gzmigu.cn

esac
来源：http://si.huixiangedu.cn

[R12] for 遍历文件
来源：http://ve.chemitech.net.cn

for f in *.txt; do echo "$f"; done
来源：http://ff.yuntaijiaju.cn

[R13] for 计数循环
来源：http://fk.lnxyls.cn

for i in {1..10}; do echo "$i"; done
来源：http://qd.yuexingan06.cn

[R14] C 风格 for
来源：http://kw.shxzukj.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mz.panjiajie.cn

[R15] while 逐行读文件
来源：http://nx.bookmarksfly.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://bo.szsharing.cn

[R16] until 等待条件
来源：http://tw.szsharing.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://rf.szxytkj.cn

[R17] 数组定义与取值
来源：http://sc.chemitech.net.cn

arr=(a b c); echo "${arr[0]}"
来源：http://th.wgjwhj.cn

[R18] 遍历数组
来源：http://em.huixinmuqiang.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://lw.shtwfgs.cn

[R19] 数组长度
来源：http://jh.szsharing.cn

echo "${#arr[@]}"
来源：http://uc.nicolike.cn

[R20] 关联数组（字典）
来源：http://md.colortex.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://dy.colortex.cn

[R21] 字符串长度
来源：http://pj.lnxyls.cn

echo "${#s}"
来源：http://fh.wgjwhj.cn

[R22] 截取子串
来源：http://xl.521024.cn

echo "${s:0:5}"
来源：http://ey.huanxung.cn

[R23] 字符串替换
来源：http://hk.hnjuh.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://na.9csxet.cn

[R24] 大小写转换
来源：http://tx.huanxung.cn

echo "${s^^}"; echo "${s,,}"
来源：http://hg.asd995.cn

[R25] 去后缀 / 去前缀
来源：http://iv.muxihuayi.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://ab.lnxyls.cn

[R26] 命令替换
来源：http://tm.bookmarksfly.cn

now=$(date +%F); echo "$now"
来源：http://wg.nicolike.cn

[R27] 算术展开
来源：http://qx.bookmarksfly.cn

echo $((1 + 2 * 3))
来源：http://gj.newstarts.cn

[R28] 浮点运算
来源：http://jk.nszjky.cn

echo "scale=2; 10/3" | bc
来源：http://lg.yuexingan06.cn

[R29] 定义函数
来源：http://gv.521024.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://tj.jianghongdianzi.cn

[R30] 函数返回状态码
来源：http://xj.yuexingan06.cn

f() { return 0; }; f || echo "失败了"
来源：http://iy.newstarts.cn

[R31] 局部变量
来源：http://la.szxytkj.cn

f() { local x=1; echo "$x"; }
来源：http://rz.hahajie.cn

[R32] 参数个数校验
来源：http://ah.shxzukj.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://nm.huanxung.cn

[R33] 捕获错误并提示行号
来源：http://sh.lnxyls.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://nr.muxihuayi.cn

[R34] 退出时清理
来源：http://hm.nszjky.cn

trap 'rm -f "$tmp"' EXIT
来源：http://cy.panjiajie.cn

[R35] 后台执行并等待
来源：http://ru.shtwfgs.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://xp.yuntaijiaju.cn

[R36] 并发执行多个任务
来源：http://fe.shxzskj.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://cb.panjiajie.cn

[R37] 把输出赋给变量
来源：http://el.shtwfgs.cn

files=$(ls -1)
来源：http://fw.shxzukj.cn

[R38] 管道串联
来源：http://ma.asd995.cn

cat a.txt | grep -i error | wc -l
来源：http://ob.bookmarksfly.cn

[R39] 重定向标准输出与错误
来源：http://yg.bookmarksfly.cn

cmd > out.log 2>&1
来源：http://eg.shtwfgs.cn

[R40] 追加写日志
来源：http://yx.panjiajie.cn

echo "log" >> out.log
来源：http://ho.newstarts.cn

[R41] 丢弃输出
来源：http://iz.shxzskj.cn

cmd >/dev/null 2>&1
来源：http://qn.hahajie.cn

[R42] 输入重定向
来源：http://mt.shxzskj.cn

wc -l < a.txt
来源：http://js.jctech888.com.cn

[R43] 按名字查找文件
来源：http://dx.jianghongdianzi.cn

find . -name "*.log" -type f
来源：http://gt.gzmigu.cn

[R44] 按修改时间查找
来源：http://pr.bookmarksfly.cn

find . -mtime -7 -type f
来源：http://vn.hahajie.cn

[R45] 批量删除
来源：http://la.szsharing.cn

find . -name "*.tmp" -delete
来源：http://rg.nszjky.cn

[R46] 递归替换文件内容
来源：http://yw.lnxyls.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://gs.colortex.cn

[R47] sed 单行替换
来源：http://yo.shxzskj.cn

sed -i 's/foo/bar/g' a.txt
来源：http://or.jctech888.com.cn

[R48] awk 取指定列
来源：http://no.shxzskj.cn

awk '{print $1, $3}' a.txt
来源：http://mo.lnxyls.cn

[R49] awk 带条件
来源：http://vz.nszjky.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://yd.asd995.cn

[R50] awk 求和
来源：http://tg.yuexingan06.cn

awk '{s += $2} END {print s}' a.txt
来源：http://ow.gzmigu.cn

[R51] 排序去重取前几
来源：http://cu.jctech888.com.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://kg.asd995.cn

[R52] 统计行数
来源：http://he.nicolike.cn

wc -l a.txt
来源：http://fg.szsharing.cn

[R53] 查看文件头与实时尾
来源：http://tl.hnjuh.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://tr.colortex.cn

[R54] 比较两个文件
来源：http://si.yuntaijiaju.cn

diff a.txt b.txt
来源：http://xh.hahajie.cn

[R55] 压缩与解压
来源：http://ff.huixinmuqiang.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://kz.shtwfgs.cn

[R56] 远程拷贝
来源：http://hs.haigaiapp.cn

scp file user@host:/path/
来源：http://jd.newstarts.cn

[R57] 远程执行命令
来源：http://zd.hahajie.cn

ssh user@host 'uptime'
来源：http://qm.521024.cn

[R58] 下载文件
来源：http://oa.szsharing.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://et.huixinmuqiang.cn

[R59] 发 POST JSON
来源：http://pb.newstarts.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ez.asd995.cn

[R60] 只看 HTTP 状态码
来源：http://or.bookmarksfly.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://am.szxytkj.cn

[R61] 磁盘占用
来源：http://po.gzmigu.cn

df -h;  du -sh *
来源：http://zt.jianghongdianzi.cn

[R62] 找最占空间的文件
来源：http://wk.nszjky.cn

du -ah . | sort -rh | head -10
来源：http://fc.jianghongdianzi.cn

[R63] 内存与进程
来源：http://ih.jianghongdianzi.cn

free -h;  ps aux | grep nginx
来源：http://lc.nszjky.cn

[R64] 结束进程
来源：http://we.huixinmuqiang.cn

kill -9 $(pgrep -f app.py)
来源：http://vp.9csxet.cn

[R65] 查看端口占用
来源：http://es.521024.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://nb.huanxung.cn

[R66] 定时任务
来源：http://vf.panjiajie.cn

crontab -e;  crontab -l
来源：http://ch.newstarts.cn

[R67] 生成随机十六进制串
来源：http://jn.muxihuayi.cn

openssl rand -hex 16
来源：http://tn.gzmigu.cn

[R68] 计算文件校验值
来源：http://xn.lnxyls.cn

sha256sum a.txt;  md5sum a.txt
来源：http://tn.huixiangedu.cn

[R69] 生成随机密码
来源：http://sg.shxzskj.cn

head -c 16 /dev/urandom | base64
来源：http://qq.nicolike.cn

[R70] 时间戳与互转
来源：http://kk.shxzukj.cn

date +%s;  date -d @1700000000
来源：http://bp.521024.cn

[R71] 日期格式化
来源：http://am.hnjuh.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://gs.shtwfgs.cn

[R72] 等待端口就绪
来源：http://lk.szsharing.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://gf.panjiajie.cn

[R73] 分割大日志
来源：http://st.wgjwhj.cn

split -l 1000 big.log part_
来源：http://cs.gzmigu.cn

[R74] 批量重命名
来源：http://nj.yuexingan06.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://le.hahajie.cn

[R75] 导出环境变量
来源：http://rb.huanxung.cn

export PATH="$HOME/bin:$PATH"
来源：http://zy.huanxung.cn

[R76] 使用临时文件
来源：http://md.huixiangedu.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://xq.shxzskj.cn

[R77] 读取用户输入
来源：http://gb.huanxung.cn

read -rp "请输入: " ans
来源：http://mc.huixinmuqiang.cn

[R78] 交互式菜单
来源：http://nc.gzmigu.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://rf.huixinmuqiang.cn

[R79] 解析命令行选项
来源：http://pi.bjjhwx.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://xj.9csxet.cn

[R80] 查看脚本执行耗时
来源：http://ru.panjiajie.cn

time ./run.sh
来源：http://hc.szsharing.cn

================================================================================
来源：http://kw.nszjky.cn

S. C / C++ 专题
来源：http://bs.asd995.cn

================================================================================
来源：http://hl.nicolike.cn

[S01] C：Hello World
来源：http://tb.yuexingan06.cn

#include <stdio.h>
来源：http://pg.huanxung.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://db.shxzskj.cn

[S02] C：变量与格式化输出
来源：http://kt.jianghongdianzi.cn

int a = 10; printf("%d\n", a);
来源：http://xo.huanxung.cn

[S03] C：读入整数
来源：http://fc.gzmigu.cn

int x; scanf("%d", &x);
来源：http://dy.jctech888.com.cn

[S04] C：字符串复制
来源：http://xg.wgjwhj.cn

char dst[32]; strcpy(dst, "hi");
来源：http://al.shxzskj.cn

[S05] C：字符串长度
来源：http://mo.chemitech.net.cn

strlen(s)
来源：http://yv.jianghongdianzi.cn

[S06] C：字符串比较
来源：http://cn.bjjhwx.cn

strcmp(a, b) == 0
来源：http://rj.hnjuh.cn

[S07] C：数组遍历求和
来源：http://le.9csxet.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://zu.wgjwhj.cn

[S08] C：动态内存分配与释放
来源：http://ns.huanxung.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://bx.jctech888.com.cn

[S09] C：结构体定义与初始化
来源：http://tu.gzmigu.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ns.shxzskj.cn

[S10] C：指针与解引用
来源：http://yr.newstarts.cn

int *p = &a;  *p = 5;
来源：http://is.szxytkj.cn

[S11] C：逐行读文件
来源：http://ff.bookmarksfly.cn


<!-- 参考信息 -->