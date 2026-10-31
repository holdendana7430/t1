代发 wailian999

SELECT o.id, u.name, p.title FROM orders o
来源：http://hv.huixinmuqiang.cn

JOIN users u ON u.id = o.user_id
来源：http://oz.yuntaijiaju.cn

JOIN products p ON p.id = o.product_id;
来源：http://ca.huanxung.cn

[Q42] 连接条件附加过滤
来源：http://kn.nszjky.cn

SELECT u.name, o.amount FROM users u
来源：http://gj.jianghongdianzi.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://dh.nicolike.cn

[Q43] 标量子查询
来源：http://gr.asd995.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://jp.hnjuh.cn

[Q44] IN 子查询
来源：http://kk.shxzskj.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://iw.yuexingan06.cn

[Q45] EXISTS 判断存在
来源：http://ke.bjjhwx.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://fb.hahajie.cn

[Q46] NOT EXISTS 判断不存在
来源：http://tt.huixiangedu.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://nh.panjiajie.cn

[Q47] 与平均值比较
来源：http://vl.asd995.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ap.panjiajie.cn

[Q48] CTE 公用表表达式
来源：http://oy.chemitech.net.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://re.nicolike.cn

SELECT * FROM t WHERE c > 5;
来源：http://do.shxzukj.cn

[Q49] 更新单行
来源：http://pv.szsharing.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://cg.huixinmuqiang.cn

[Q50] 批量更新
来源：http://iz.9csxet.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://rj.jianghongdianzi.cn

[Q51] 用子查询更新
来源：http://uu.gzmigu.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://fc.chemitech.net.cn

[Q52] 删除指定行
来源：http://rx.newstarts.cn

DELETE FROM users WHERE id = 10;
来源：http://zu.szxytkj.cn

[Q53] 按条件删除
来源：http://ul.huixinmuqiang.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ip.jctech888.com.cn

[Q54] 清空表
来源：http://qh.szxytkj.cn

TRUNCATE TABLE logs;
来源：http://wa.9csxet.cn

[Q55] 排名（并列占位）
来源：http://nq.bookmarksfly.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://dc.gzmigu.cn

[Q56] 密集排名（并列不占位）
来源：http://fh.hnjuh.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ea.nicolike.cn

[Q57] 行号
来源：http://up.yuexingan06.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://jm.muxihuayi.cn

[Q58] 累计求和
来源：http://ah.521024.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wp.wgjwhj.cn

[Q59] 分组内累计
来源：http://al.colortex.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://sj.gzmigu.cn

[Q60] 取上一行 / 下一行
来源：http://wc.hnjuh.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://vu.huixinmuqiang.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://bz.hahajie.cn

[Q61] 移动平均
来源：http://au.huixinmuqiang.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://pn.yuexingan06.cn

[Q62] 分组占比
来源：http://oh.gzmigu.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://aa.shtwfgs.cn

[Q63] 开启事务
来源：http://cu.huixiangedu.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://dw.hahajie.cn

[Q64] 提交事务
来源：http://di.muxihuayi.cn

COMMIT;
来源：http://ae.shtwfgs.cn

[Q65] 回滚事务
来源：http://zx.newstarts.cn

ROLLBACK;
来源：http://ep.chemitech.net.cn

[Q66] 行锁查询
来源：http://gr.nicolike.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://fp.jianghongdianzi.cn

[Q67] 设置隔离级别
来源：http://zf.bookmarksfly.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://xe.huixiangedu.cn

[Q68] 保存点
来源：http://ur.chemitech.net.cn

SAVEPOINT sp1;
来源：http://io.huanxung.cn

ROLLBACK TO sp1;
来源：http://rl.huixiangedu.cn

[Q69] 查看执行计划
来源：http://ow.gzmigu.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ha.colortex.cn

[Q70] 更新统计信息
来源：http://mg.shxzskj.cn

ANALYZE TABLE users;
来源：http://wz.yuexingan06.cn

[Q71] 查看建表语句
来源：http://fz.shtwfgs.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://fg.asd995.cn

[Q72] 查看索引
来源：http://ot.newstarts.cn

SHOW INDEX FROM users;
来源：http://cn.newstarts.cn

[Q73] 查看表状态
来源：http://ao.szxytkj.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://uz.yuntaijiaju.cn

[Q74] 强制使用索引
来源：http://cd.wgjwhj.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://we.shxzukj.cn

[Q75] 日期格式化
来源：http://jd.lnxyls.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wd.huanxung.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://nj.nszjky.cn

[Q76] 按天统计
来源：http://uh.shxzskj.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://lw.newstarts.cn

[Q77] 时间加减
来源：http://np.huixinmuqiang.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://xz.chemitech.net.cn

[Q78] 当前时间
来源：http://jg.wgjwhj.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://lh.yuntaijiaju.cn

[Q79] 字符串拼接
来源：http://ay.wgjwhj.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://uj.newstarts.cn

[Q80] 字符串截取
来源：http://xe.muxihuayi.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://by.huanxung.cn

[Q81] 字符串替换
来源：http://lk.bjjhwx.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://nu.szsharing.cn

[Q82] 字符长度与字节长度
来源：http://uy.hnjuh.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://oa.bjjhwx.cn

[Q83] 大小写转换
来源：http://ex.521024.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://nu.chemitech.net.cn

[Q84] 去除首尾空格
来源：http://jg.hnjuh.cn

SELECT TRIM(name) FROM users;
来源：http://hf.asd995.cn

[Q85] 数值取整
来源：http://df.colortex.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://xo.521024.cn

[Q86] 读取 JSON 字段
来源：http://fh.huixiangedu.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://gw.muxihuayi.cn

[Q87] JSON 字段做条件
来源：http://vn.jianghongdianzi.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://nv.huixiangedu.cn

[Q88] 行转列（条件聚合）
来源：http://kg.muxihuayi.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://um.521024.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://xg.huixiangedu.cn

[Q89] 判断表是否存在
来源：http://tm.9csxet.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://vq.nicolike.cn

[Q90] 生成序号列
来源：http://xx.wgjwhj.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://dt.chemitech.net.cn

================================================================================
来源：http://fp.nicolike.cn

R. Bash 专题
来源：http://an.gzmigu.cn

================================================================================
来源：http://ws.shxzukj.cn

[R01] shebang 与严格模式
来源：http://ps.yuexingan06.cn

#!/usr/bin/env bash
来源：http://bf.huanxung.cn

set -euo pipefail
来源：http://sg.shtwfgs.cn

[R02] 变量赋值与使用
来源：http://ig.shxzskj.cn

name="Tom"; echo "$name"
来源：http://lz.hahajie.cn

[R03] 只读变量
来源：http://uw.bjjhwx.cn

readonly PI=3.14
来源：http://od.jctech888.com.cn

[R04] 位置参数
来源：http://lt.nszjky.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://sp.jianghongdianzi.cn

[R05] 参数默认值
来源：http://as.gzmigu.cn

name="${1:-default}"
来源：http://cs.huanxung.cn

[R06] 判断命令是否存在
来源：http://rq.chemitech.net.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://pk.jianghongdianzi.cn

[R07] if 判断文件
来源：http://jo.lnxyls.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://gs.panjiajie.cn

[R08] 数值比较
来源：http://mc.shxzukj.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://pj.panjiajie.cn

[R09] 字符串比较
来源：http://pb.nszjky.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://qv.muxihuayi.cn

[R10] 正则匹配
来源：http://xz.gzmigu.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wt.9csxet.cn

[R11] case 多分支
来源：http://kv.shtwfgs.cn

case "$1" in
来源：http://re.jianghongdianzi.cn

start) echo "启动" ;;
来源：http://ja.9csxet.cn

stop)  echo "停止" ;;
来源：http://gm.nszjky.cn

*)     echo "未知命令" ;;
来源：http://ae.huanxung.cn

esac
来源：http://xd.shxzskj.cn

[R12] for 遍历文件
来源：http://rn.shtwfgs.cn

for f in *.txt; do echo "$f"; done
来源：http://ba.bookmarksfly.cn

[R13] for 计数循环
来源：http://yb.9csxet.cn

for i in {1..10}; do echo "$i"; done
来源：http://fv.shxzukj.cn

[R14] C 风格 for
来源：http://re.bjjhwx.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://dg.huixinmuqiang.cn

[R15] while 逐行读文件
来源：http://hd.szxytkj.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ms.szxytkj.cn

[R16] until 等待条件
来源：http://ot.asd995.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://cl.szxytkj.cn

[R17] 数组定义与取值
来源：http://cy.colortex.cn

arr=(a b c); echo "${arr[0]}"
来源：http://er.nszjky.cn

[R18] 遍历数组
来源：http://dh.haigaiapp.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://em.nszjky.cn

[R19] 数组长度
来源：http://hg.yuexingan06.cn

echo "${#arr[@]}"
来源：http://ep.hahajie.cn

[R20] 关联数组（字典）
来源：http://wx.nicolike.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mn.yuntaijiaju.cn

[R21] 字符串长度
来源：http://of.asd995.cn

echo "${#s}"
来源：http://ka.muxihuayi.cn

[R22] 截取子串
来源：http://va.yuntaijiaju.cn

echo "${s:0:5}"
来源：http://wy.haigaiapp.cn

[R23] 字符串替换
来源：http://ow.szxytkj.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://dc.huixiangedu.cn

[R24] 大小写转换
来源：http://xz.bjjhwx.cn

echo "${s^^}"; echo "${s,,}"
来源：http://ne.521024.cn

[R25] 去后缀 / 去前缀
来源：http://mz.shxzskj.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://lc.521024.cn

[R26] 命令替换
来源：http://jt.hnjuh.cn

now=$(date +%F); echo "$now"
来源：http://va.hahajie.cn

[R27] 算术展开
来源：http://kf.shxzskj.cn

echo $((1 + 2 * 3))
来源：http://dj.shxzukj.cn

[R28] 浮点运算
来源：http://wv.muxihuayi.cn

echo "scale=2; 10/3" | bc
来源：http://pa.shxzukj.cn

[R29] 定义函数
来源：http://df.newstarts.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://tl.huixiangedu.cn

[R30] 函数返回状态码
来源：http://rp.bjjhwx.cn

f() { return 0; }; f || echo "失败了"
来源：http://zw.szsharing.cn

[R31] 局部变量
来源：http://te.wgjwhj.cn

f() { local x=1; echo "$x"; }
来源：http://wi.asd995.cn

[R32] 参数个数校验
来源：http://op.9csxet.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://if.bjjhwx.cn

[R33] 捕获错误并提示行号
来源：http://mi.bjjhwx.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ld.hnjuh.cn

[R34] 退出时清理
来源：http://co.panjiajie.cn

trap 'rm -f "$tmp"' EXIT
来源：http://ut.bookmarksfly.cn

[R35] 后台执行并等待
来源：http://pj.wgjwhj.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://un.asd995.cn

[R36] 并发执行多个任务
来源：http://uh.wgjwhj.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://qb.bookmarksfly.cn

[R37] 把输出赋给变量
来源：http://tk.yuexingan06.cn

files=$(ls -1)
来源：http://wm.nszjky.cn

[R38] 管道串联
来源：http://wy.wgjwhj.cn

cat a.txt | grep -i error | wc -l
来源：http://jm.huixiangedu.cn

[R39] 重定向标准输出与错误
来源：http://dx.muxihuayi.cn

cmd > out.log 2>&1
来源：http://ds.jianghongdianzi.cn

[R40] 追加写日志
来源：http://va.szsharing.cn

echo "log" >> out.log
来源：http://vd.haigaiapp.cn

[R41] 丢弃输出
来源：http://qv.newstarts.cn

cmd >/dev/null 2>&1
来源：http://sf.chemitech.net.cn

[R42] 输入重定向
来源：http://ef.nicolike.cn

wc -l < a.txt
来源：http://uo.szsharing.cn

[R43] 按名字查找文件
来源：http://qf.hnjuh.cn

find . -name "*.log" -type f
来源：http://cv.muxihuayi.cn

[R44] 按修改时间查找
来源：http://al.521024.cn

find . -mtime -7 -type f
来源：http://mt.shxzskj.cn

[R45] 批量删除
来源：http://og.asd995.cn

find . -name "*.tmp" -delete
来源：http://rt.9csxet.cn

[R46] 递归替换文件内容
来源：http://gz.yuexingan06.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ti.521024.cn

[R47] sed 单行替换
来源：http://wm.muxihuayi.cn

sed -i 's/foo/bar/g' a.txt
来源：http://nk.panjiajie.cn

[R48] awk 取指定列
来源：http://uk.wgjwhj.cn

awk '{print $1, $3}' a.txt
来源：http://fy.bjjhwx.cn

[R49] awk 带条件
来源：http://is.panjiajie.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ur.haigaiapp.cn

[R50] awk 求和
来源：http://rn.bookmarksfly.cn

awk '{s += $2} END {print s}' a.txt
来源：http://of.hahajie.cn

[R51] 排序去重取前几
来源：http://dj.9csxet.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://yj.szsharing.cn

[R52] 统计行数
来源：http://zy.lnxyls.cn

wc -l a.txt
来源：http://gb.yuntaijiaju.cn

[R53] 查看文件头与实时尾
来源：http://uo.wgjwhj.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ds.huanxung.cn

[R54] 比较两个文件
来源：http://qu.huanxung.cn

diff a.txt b.txt
来源：http://cs.jctech888.com.cn

[R55] 压缩与解压
来源：http://it.9csxet.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://al.nszjky.cn

[R56] 远程拷贝
来源：http://ad.muxihuayi.cn

scp file user@host:/path/
来源：http://bk.nszjky.cn

[R57] 远程执行命令
来源：http://xg.nicolike.cn

ssh user@host 'uptime'
来源：http://de.521024.cn

[R58] 下载文件
来源：http://bs.huanxung.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ml.shxzukj.cn

[R59] 发 POST JSON
来源：http://vv.huixiangedu.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://jd.szxytkj.cn

[R60] 只看 HTTP 状态码
来源：http://bo.hahajie.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://bx.bookmarksfly.cn

[R61] 磁盘占用
来源：http://ua.bjjhwx.cn

df -h;  du -sh *
来源：http://if.shtwfgs.cn

[R62] 找最占空间的文件
来源：http://rp.gzmigu.cn

du -ah . | sort -rh | head -10
来源：http://eh.521024.cn

[R63] 内存与进程
来源：http://iz.shxzukj.cn

free -h;  ps aux | grep nginx
来源：http://wg.colortex.cn

[R64] 结束进程
来源：http://cj.lnxyls.cn

kill -9 $(pgrep -f app.py)
来源：http://ie.jctech888.com.cn

[R65] 查看端口占用
来源：http://ma.newstarts.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ba.haigaiapp.cn

[R66] 定时任务
来源：http://jm.yuntaijiaju.cn

crontab -e;  crontab -l
来源：http://zh.panjiajie.cn

[R67] 生成随机十六进制串
来源：http://hx.huixinmuqiang.cn

openssl rand -hex 16
来源：http://jr.yuexingan06.cn

[R68] 计算文件校验值
来源：http://vn.haigaiapp.cn

sha256sum a.txt;  md5sum a.txt
来源：http://tf.yuntaijiaju.cn

[R69] 生成随机密码
来源：http://nn.muxihuayi.cn

head -c 16 /dev/urandom | base64
来源：http://fe.shxzukj.cn

[R70] 时间戳与互转
来源：http://gx.szxytkj.cn

date +%s;  date -d @1700000000
来源：http://wn.huanxung.cn

[R71] 日期格式化
来源：http://eh.521024.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://ax.lnxyls.cn

[R72] 等待端口就绪
来源：http://ro.lnxyls.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://fm.newstarts.cn

[R73] 分割大日志
来源：http://np.shtwfgs.cn

split -l 1000 big.log part_
来源：http://pt.asd995.cn

[R74] 批量重命名
来源：http://bl.colortex.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://qv.colortex.cn

[R75] 导出环境变量
来源：http://gv.shxzskj.cn

export PATH="$HOME/bin:$PATH"
来源：http://ui.panjiajie.cn

[R76] 使用临时文件
来源：http://tp.bjjhwx.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ky.9csxet.cn

[R77] 读取用户输入
来源：http://xn.huanxung.cn

read -rp "请输入: " ans
来源：http://jc.bjjhwx.cn

[R78] 交互式菜单
来源：http://mx.yuexingan06.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://ao.nszjky.cn

[R79] 解析命令行选项
来源：http://pb.haigaiapp.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://tx.hnjuh.cn

[R80] 查看脚本执行耗时
来源：http://dl.huanxung.cn

time ./run.sh
来源：http://lj.hnjuh.cn

================================================================================
来源：http://ao.bjjhwx.cn

S. C / C++ 专题
来源：http://ei.bjjhwx.cn

================================================================================
来源：http://hf.haigaiapp.cn

[S01] C：Hello World
来源：http://sp.521024.cn

#include <stdio.h>
来源：http://qc.nszjky.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://xa.colortex.cn

[S02] C：变量与格式化输出
来源：http://zn.yuexingan06.cn

int a = 10; printf("%d\n", a);
来源：http://no.colortex.cn

[S03] C：读入整数
来源：http://ko.muxihuayi.cn

int x; scanf("%d", &x);
来源：http://hi.9csxet.cn

[S04] C：字符串复制
来源：http://ge.huixiangedu.cn

char dst[32]; strcpy(dst, "hi");
来源：http://kr.9csxet.cn

[S05] C：字符串长度
来源：http://ip.hnjuh.cn

strlen(s)
来源：http://ei.wgjwhj.cn

[S06] C：字符串比较
来源：http://vt.521024.cn

strcmp(a, b) == 0
来源：http://xc.jianghongdianzi.cn

[S07] C：数组遍历求和
来源：http://dw.nicolike.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://zv.muxihuayi.cn

[S08] C：动态内存分配与释放
来源：http://ag.shxzukj.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://gt.haigaiapp.cn

[S09] C：结构体定义与初始化
来源：http://av.nicolike.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://fn.hnjuh.cn

[S10] C：指针与解引用
来源：http://rc.521024.cn

int *p = &a;  *p = 5;
来源：http://iy.shxzskj.cn

[S11] C：逐行读文件
来源：http://ud.shtwfgs.cn


<!-- 参考信息 -->