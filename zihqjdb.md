代发 wailian999

[Q44] IN 子查询
来源：http://ms.panjiajie.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://yw.newstarts.cn

[Q45] EXISTS 判断存在
来源：http://ng.asd995.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hj.shxzskj.cn

[Q46] NOT EXISTS 判断不存在
来源：http://wr.bjjhwx.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://nk.colortex.cn

[Q47] 与平均值比较
来源：http://yn.shxzskj.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://qy.panjiajie.cn

[Q48] CTE 公用表表达式
来源：http://kt.shxzskj.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://co.newstarts.cn

SELECT * FROM t WHERE c > 5;
来源：http://gq.hnjuh.cn

[Q49] 更新单行
来源：http://ut.shxzskj.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://vk.shxzskj.cn

[Q50] 批量更新
来源：http://zz.jianghongdianzi.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://zm.nicolike.cn

[Q51] 用子查询更新
来源：http://vb.muxihuayi.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://fy.szxytkj.cn

[Q52] 删除指定行
来源：http://xn.szxytkj.cn

DELETE FROM users WHERE id = 10;
来源：http://hy.yuntaijiaju.cn

[Q53] 按条件删除
来源：http://dl.panjiajie.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hy.huixiangedu.cn

[Q54] 清空表
来源：http://by.asd995.cn

TRUNCATE TABLE logs;
来源：http://sm.jctech888.com.cn

[Q55] 排名（并列占位）
来源：http://zh.shxzukj.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://fz.huanxung.cn

[Q56] 密集排名（并列不占位）
来源：http://xe.9csxet.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://kc.gzmigu.cn

[Q57] 行号
来源：http://lz.huixinmuqiang.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://za.shxzskj.cn

[Q58] 累计求和
来源：http://tg.huanxung.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://fd.gzmigu.cn

[Q59] 分组内累计
来源：http://ex.bjjhwx.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://qx.shxzukj.cn

[Q60] 取上一行 / 下一行
来源：http://xi.jctech888.com.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://pf.wgjwhj.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://qb.521024.cn

[Q61] 移动平均
来源：http://cn.huixiangedu.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://cs.panjiajie.cn

[Q62] 分组占比
来源：http://ou.shxzukj.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://fu.9csxet.cn

[Q63] 开启事务
来源：http://ln.bookmarksfly.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://we.asd995.cn

[Q64] 提交事务
来源：http://ny.nszjky.cn

COMMIT;
来源：http://dh.hahajie.cn

[Q65] 回滚事务
来源：http://pf.panjiajie.cn

ROLLBACK;
来源：http://xx.shtwfgs.cn

[Q66] 行锁查询
来源：http://xe.hahajie.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://cv.haigaiapp.cn

[Q67] 设置隔离级别
来源：http://mt.wgjwhj.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hm.shxzskj.cn

[Q68] 保存点
来源：http://ph.yuntaijiaju.cn

SAVEPOINT sp1;
来源：http://wn.bjjhwx.cn

ROLLBACK TO sp1;
来源：http://rg.nszjky.cn

[Q69] 查看执行计划
来源：http://rk.nszjky.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://pd.yuntaijiaju.cn

[Q70] 更新统计信息
来源：http://ih.muxihuayi.cn

ANALYZE TABLE users;
来源：http://dg.panjiajie.cn

[Q71] 查看建表语句
来源：http://lv.nszjky.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://qs.colortex.cn

[Q72] 查看索引
来源：http://cd.jctech888.com.cn

SHOW INDEX FROM users;
来源：http://vh.chemitech.net.cn

[Q73] 查看表状态
来源：http://xm.nszjky.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://aa.asd995.cn

[Q74] 强制使用索引
来源：http://bd.bookmarksfly.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hh.haigaiapp.cn

[Q75] 日期格式化
来源：http://ts.asd995.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://gq.wgjwhj.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://he.asd995.cn

[Q76] 按天统计
来源：http://ry.huixiangedu.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://zg.huixinmuqiang.cn

[Q77] 时间加减
来源：http://vr.jctech888.com.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://un.9csxet.cn

[Q78] 当前时间
来源：http://sw.yuexingan06.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://qx.yuntaijiaju.cn

[Q79] 字符串拼接
来源：http://lq.wgjwhj.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://aj.jctech888.com.cn

[Q80] 字符串截取
来源：http://vm.lnxyls.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ld.szxytkj.cn

[Q81] 字符串替换
来源：http://gu.gzmigu.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://qx.colortex.cn

[Q82] 字符长度与字节长度
来源：http://fr.yuntaijiaju.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wi.shxzskj.cn

[Q83] 大小写转换
来源：http://jk.jctech888.com.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://le.newstarts.cn

[Q84] 去除首尾空格
来源：http://pe.gzmigu.cn

SELECT TRIM(name) FROM users;
来源：http://tu.521024.cn

[Q85] 数值取整
来源：http://wi.gzmigu.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://cv.9csxet.cn

[Q86] 读取 JSON 字段
来源：http://an.yuntaijiaju.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ru.colortex.cn

[Q87] JSON 字段做条件
来源：http://fn.yuexingan06.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ea.yuntaijiaju.cn

[Q88] 行转列（条件聚合）
来源：http://wu.muxihuayi.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://pz.huanxung.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hy.lnxyls.cn

[Q89] 判断表是否存在
来源：http://xa.szxytkj.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://el.newstarts.cn

[Q90] 生成序号列
来源：http://cf.hnjuh.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ho.nszjky.cn

================================================================================
来源：http://ui.yuexingan06.cn

R. Bash 专题
来源：http://td.shtwfgs.cn

================================================================================
来源：http://ny.chemitech.net.cn

[R01] shebang 与严格模式
来源：http://ku.haigaiapp.cn

#!/usr/bin/env bash
来源：http://ld.hnjuh.cn

set -euo pipefail
来源：http://hr.shtwfgs.cn

[R02] 变量赋值与使用
来源：http://be.wgjwhj.cn

name="Tom"; echo "$name"
来源：http://pv.gzmigu.cn

[R03] 只读变量
来源：http://ba.shtwfgs.cn

readonly PI=3.14
来源：http://nw.huanxung.cn

[R04] 位置参数
来源：http://dd.newstarts.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://cu.shxzukj.cn

[R05] 参数默认值
来源：http://sz.shtwfgs.cn

name="${1:-default}"
来源：http://zy.bookmarksfly.cn

[R06] 判断命令是否存在
来源：http://nb.jianghongdianzi.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ui.lnxyls.cn

[R07] if 判断文件
来源：http://qo.chemitech.net.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://up.newstarts.cn

[R08] 数值比较
来源：http://lh.jctech888.com.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://cq.haigaiapp.cn

[R09] 字符串比较
来源：http://ex.nicolike.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ta.jianghongdianzi.cn

[R10] 正则匹配
来源：http://ij.shxzskj.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://no.muxihuayi.cn

[R11] case 多分支
来源：http://ss.gzmigu.cn

case "$1" in
来源：http://rz.jianghongdianzi.cn

start) echo "启动" ;;
来源：http://sn.chemitech.net.cn

stop)  echo "停止" ;;
来源：http://ib.huixiangedu.cn

*)     echo "未知命令" ;;
来源：http://bv.yuntaijiaju.cn

esac
来源：http://vc.asd995.cn

[R12] for 遍历文件
来源：http://vb.jianghongdianzi.cn

for f in *.txt; do echo "$f"; done
来源：http://pt.chemitech.net.cn

[R13] for 计数循环
来源：http://ap.chemitech.net.cn

for i in {1..10}; do echo "$i"; done
来源：http://qf.chemitech.net.cn

[R14] C 风格 for
来源：http://eu.panjiajie.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://rx.9csxet.cn

[R15] while 逐行读文件
来源：http://zg.huixiangedu.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://yj.haigaiapp.cn

[R16] until 等待条件
来源：http://rx.jianghongdianzi.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ei.wgjwhj.cn

[R17] 数组定义与取值
来源：http://of.huixinmuqiang.cn

arr=(a b c); echo "${arr[0]}"
来源：http://ad.newstarts.cn

[R18] 遍历数组
来源：http://yu.lnxyls.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://bu.yuexingan06.cn

[R19] 数组长度
来源：http://uh.newstarts.cn

echo "${#arr[@]}"
来源：http://ut.yuntaijiaju.cn

[R20] 关联数组（字典）
来源：http://mk.haigaiapp.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://zk.jctech888.com.cn

[R21] 字符串长度
来源：http://fn.huixinmuqiang.cn

echo "${#s}"
来源：http://ax.521024.cn

[R22] 截取子串
来源：http://tu.hnjuh.cn

echo "${s:0:5}"
来源：http://xq.huanxung.cn

[R23] 字符串替换
来源：http://xv.asd995.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://dx.huixiangedu.cn

[R24] 大小写转换
来源：http://mb.huixiangedu.cn

echo "${s^^}"; echo "${s,,}"
来源：http://le.gzmigu.cn

[R25] 去后缀 / 去前缀
来源：http://pw.haigaiapp.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://sv.szxytkj.cn

[R26] 命令替换
来源：http://ud.shxzukj.cn

now=$(date +%F); echo "$now"
来源：http://ab.huixinmuqiang.cn

[R27] 算术展开
来源：http://oc.shxzskj.cn

echo $((1 + 2 * 3))
来源：http://qm.panjiajie.cn

[R28] 浮点运算
来源：http://ez.colortex.cn

echo "scale=2; 10/3" | bc
来源：http://jk.chemitech.net.cn

[R29] 定义函数
来源：http://lx.yuntaijiaju.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://rf.szsharing.cn

[R30] 函数返回状态码
来源：http://ly.nszjky.cn

f() { return 0; }; f || echo "失败了"
来源：http://dx.jctech888.com.cn

[R31] 局部变量
来源：http://tn.colortex.cn

f() { local x=1; echo "$x"; }
来源：http://gh.szxytkj.cn

[R32] 参数个数校验
来源：http://dp.szxytkj.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://vi.huanxung.cn

[R33] 捕获错误并提示行号
来源：http://tv.bjjhwx.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://sb.newstarts.cn

[R34] 退出时清理
来源：http://gc.asd995.cn

trap 'rm -f "$tmp"' EXIT
来源：http://wf.shxzukj.cn

[R35] 后台执行并等待
来源：http://ma.wgjwhj.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://yv.hnjuh.cn

[R36] 并发执行多个任务
来源：http://ch.yuntaijiaju.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://vg.shtwfgs.cn

[R37] 把输出赋给变量
来源：http://jk.panjiajie.cn

files=$(ls -1)
来源：http://ew.huanxung.cn

[R38] 管道串联
来源：http://wi.shtwfgs.cn

cat a.txt | grep -i error | wc -l
来源：http://sg.wgjwhj.cn

[R39] 重定向标准输出与错误
来源：http://dx.hnjuh.cn

cmd > out.log 2>&1
来源：http://rz.hnjuh.cn

[R40] 追加写日志
来源：http://rl.nicolike.cn

echo "log" >> out.log
来源：http://wd.shxzskj.cn

[R41] 丢弃输出
来源：http://dw.chemitech.net.cn

cmd >/dev/null 2>&1
来源：http://tk.colortex.cn

[R42] 输入重定向
来源：http://qm.gzmigu.cn

wc -l < a.txt
来源：http://nl.jianghongdianzi.cn

[R43] 按名字查找文件
来源：http://im.yuexingan06.cn

find . -name "*.log" -type f
来源：http://iz.yuexingan06.cn

[R44] 按修改时间查找
来源：http://rc.nszjky.cn

find . -mtime -7 -type f
来源：http://mp.haigaiapp.cn

[R45] 批量删除
来源：http://hv.hnjuh.cn

find . -name "*.tmp" -delete
来源：http://kv.shxzskj.cn

[R46] 递归替换文件内容
来源：http://te.gzmigu.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://nq.muxihuayi.cn

[R47] sed 单行替换
来源：http://bz.muxihuayi.cn

sed -i 's/foo/bar/g' a.txt
来源：http://cj.wgjwhj.cn

[R48] awk 取指定列
来源：http://mh.bookmarksfly.cn

awk '{print $1, $3}' a.txt
来源：http://fx.panjiajie.cn

[R49] awk 带条件
来源：http://mv.yuntaijiaju.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://iu.chemitech.net.cn

[R50] awk 求和
来源：http://on.yuexingan06.cn

awk '{s += $2} END {print s}' a.txt
来源：http://bm.szsharing.cn

[R51] 排序去重取前几
来源：http://hs.jctech888.com.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://oo.hnjuh.cn

[R52] 统计行数
来源：http://kr.wgjwhj.cn

wc -l a.txt
来源：http://jd.muxihuayi.cn

[R53] 查看文件头与实时尾
来源：http://tf.hahajie.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://cj.shxzskj.cn

[R54] 比较两个文件
来源：http://ac.jianghongdianzi.cn

diff a.txt b.txt
来源：http://wi.huixiangedu.cn

[R55] 压缩与解压
来源：http://zd.yuexingan06.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://yy.lnxyls.cn

[R56] 远程拷贝
来源：http://xv.521024.cn

scp file user@host:/path/
来源：http://vc.jianghongdianzi.cn

[R57] 远程执行命令
来源：http://wf.shxzskj.cn

ssh user@host 'uptime'
来源：http://kf.yuexingan06.cn

[R58] 下载文件
来源：http://yp.jctech888.com.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://oe.bookmarksfly.cn

[R59] 发 POST JSON
来源：http://pv.gzmigu.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://zy.huanxung.cn

[R60] 只看 HTTP 状态码
来源：http://qk.szxytkj.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://se.bookmarksfly.cn

[R61] 磁盘占用
来源：http://jg.chemitech.net.cn

df -h;  du -sh *
来源：http://wm.jctech888.com.cn

[R62] 找最占空间的文件
来源：http://kn.yuexingan06.cn

du -ah . | sort -rh | head -10
来源：http://sm.chemitech.net.cn

[R63] 内存与进程
来源：http://jf.gzmigu.cn

free -h;  ps aux | grep nginx
来源：http://ct.bookmarksfly.cn

[R64] 结束进程
来源：http://cf.asd995.cn

kill -9 $(pgrep -f app.py)
来源：http://of.wgjwhj.cn

[R65] 查看端口占用
来源：http://ji.haigaiapp.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://tn.bjjhwx.cn

[R66] 定时任务
来源：http://zv.wgjwhj.cn

crontab -e;  crontab -l
来源：http://pk.shxzskj.cn

[R67] 生成随机十六进制串
来源：http://vv.shtwfgs.cn

openssl rand -hex 16
来源：http://vy.yuntaijiaju.cn

[R68] 计算文件校验值
来源：http://nw.szxytkj.cn

sha256sum a.txt;  md5sum a.txt
来源：http://fm.hnjuh.cn

[R69] 生成随机密码
来源：http://jn.huixiangedu.cn

head -c 16 /dev/urandom | base64
来源：http://qa.nszjky.cn

[R70] 时间戳与互转
来源：http://ih.gzmigu.cn

date +%s;  date -d @1700000000
来源：http://dj.muxihuayi.cn

[R71] 日期格式化
来源：http://he.hahajie.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://cz.bjjhwx.cn

[R72] 等待端口就绪
来源：http://an.muxihuayi.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://vq.yuexingan06.cn

[R73] 分割大日志
来源：http://gw.bjjhwx.cn

split -l 1000 big.log part_
来源：http://tp.shxzukj.cn

[R74] 批量重命名
来源：http://wd.szxytkj.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://oe.nicolike.cn

[R75] 导出环境变量
来源：http://xm.hahajie.cn

export PATH="$HOME/bin:$PATH"
来源：http://zc.huanxung.cn

[R76] 使用临时文件
来源：http://pv.nszjky.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://fd.bjjhwx.cn

[R77] 读取用户输入
来源：http://sq.nszjky.cn

read -rp "请输入: " ans
来源：http://oq.huanxung.cn

[R78] 交互式菜单
来源：http://zt.shtwfgs.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://pq.newstarts.cn

[R79] 解析命令行选项
来源：http://uy.muxihuayi.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ea.521024.cn

[R80] 查看脚本执行耗时
来源：http://my.haigaiapp.cn

time ./run.sh
来源：http://ys.bjjhwx.cn

================================================================================
来源：http://iw.shxzskj.cn

S. C / C++ 专题
来源：http://dh.muxihuayi.cn

================================================================================
来源：http://yu.wgjwhj.cn

[S01] C：Hello World
来源：http://fh.jianghongdianzi.cn

#include <stdio.h>
来源：http://vn.shxzskj.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://ez.nicolike.cn

[S02] C：变量与格式化输出
来源：http://rn.hnjuh.cn

int a = 10; printf("%d\n", a);
来源：http://ce.bookmarksfly.cn

[S03] C：读入整数
来源：http://va.nicolike.cn

int x; scanf("%d", &x);
来源：http://fx.shtwfgs.cn

[S04] C：字符串复制
来源：http://so.hahajie.cn

char dst[32]; strcpy(dst, "hi");
来源：http://fz.hnjuh.cn

[S05] C：字符串长度
来源：http://ri.huanxung.cn

strlen(s)
来源：http://zg.shxzskj.cn

[S06] C：字符串比较
来源：http://sw.jianghongdianzi.cn

strcmp(a, b) == 0
来源：http://ur.bjjhwx.cn

[S07] C：数组遍历求和
来源：http://nn.colortex.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://xp.lnxyls.cn

[S08] C：动态内存分配与释放
来源：http://ae.jctech888.com.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://qz.huanxung.cn

[S09] C：结构体定义与初始化
来源：http://iv.yuexingan06.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ko.szsharing.cn

[S10] C：指针与解引用
来源：http://dp.shxzukj.cn

int *p = &a;  *p = 5;
来源：http://nq.yuexingan06.cn

[S11] C：逐行读文件
来源：http://ku.nicolike.cn

FILE *f = fopen("a.txt", "r");
来源：http://xc.szxytkj.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://sv.9csxet.cn

fclose(f);
来源：http://li.szxytkj.cn

[S12] C：写文件
来源：http://ny.hnjuh.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mj.jianghongdianzi.cn

[S13] C：宏定义
来源：http://ur.shxzskj.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wb.nszjky.cn

[S14] C：枚举
来源：http://la.hnjuh.cn


<!-- 参考信息 -->