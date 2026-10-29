代发 wailian999

[Q46] NOT EXISTS 判断不存在
来源：http://3g.zdbjq.cn/Article/details/gpwqimvyu.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.fehbvm.com/Article/details/gknoaxkfz.sHtML

[Q47] 与平均值比较
来源：http://3g.fehbvm.com/Article/details/gjafwvync.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wap.fehbvm.com/Article/details/gjroofonx.sHtML

[Q48] CTE 公用表表达式
来源：http://www.share.fehbvm.com/Article/details/ggrwuxpmv.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://read.share.fehbvm.com/Article/details/gnkfgrben.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://baike.zdbjq.cn/Article/details/gecsvyotr.sHtML

[Q49] 更新单行
来源：http://read.share.hesvh.cn/Article/details/gmrxjogaq.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://3g.fehbvm.com/Article/details/gypobjjgr.sHtML

[Q50] 批量更新
来源：http://m.share.fehbvm.com/Article/details/geggbjsdd.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.m.share.zdbjq.cn/Article/details/gusbegisf.sHtML

[Q51] 用子查询更新
来源：http://3g.hesvh.cn/Article/details/gidgohwvv.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.share.hesvh.cn/Article/details/ggnyjbemv.sHtML

[Q52] 删除指定行
来源：http://www.m.share.hesvh.cn/Article/details/gedvirnfi.sHtML

DELETE FROM users WHERE id = 10;
来源：http://baike.hesvh.cn/Article/details/gmxahpanx.sHtML

[Q53] 按条件删除
来源：http://mobile.hesvh.cn/Article/details/gpohvgmvg.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.fehbvm.com/Article/details/gpsshxloe.sHtML

[Q54] 清空表
来源：http://baike.hesvh.cn/Article/details/gcsifwpcy.sHtML

TRUNCATE TABLE logs;
来源：http://www.share.zdbjq.cn/Article/details/gdgncnxrn.sHtML

[Q55] 排名（并列占位）
来源：http://www.blog.zdbjq.cn/Article/details/gdjmjhcet.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://m.share.hesvh.cn/Article/details/gbutgzgzd.sHtML

[Q56] 密集排名（并列不占位）
来源：http://mobile.zdbjq.cn/Article/details/gkqktaila.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://read.share.hesvh.cn/Article/details/gwglftflm.sHtML

[Q57] 行号
来源：http://wap.hesvh.cn/Article/details/gmltxoglm.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/ggmykeums.sHtML

[Q58] 累计求和
来源：http://mobile.hesvh.cn/Article/details/grezjnoys.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/gbsyjmdtj.sHtML

[Q59] 分组内累计
来源：http://m.share.hesvh.cn/Article/details/gmmwgkoru.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/gwurxxcqz.sHtML

[Q60] 取上一行 / 下一行
来源：http://read.share.hesvh.cn/Article/details/gbtjvxdyy.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.hesvh.cn/Article/details/gaptsuabt.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/gzhuoedbt.sHtML

[Q61] 移动平均
来源：http://m.share.zdbjq.cn/Article/details/gpixxenpg.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://3g.zdbjq.cn/Article/details/gewpfxyiv.sHtML

[Q62] 分组占比
来源：http://read.share.hesvh.cn/Article/details/gqjzrxede.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://baike.hesvh.cn/Article/details/gpsyympjq.sHtML

[Q63] 开启事务
来源：http://blog.fehbvm.com/Article/details/guobomqzc.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.zdbjq.cn/Article/details/gdywbvyfk.sHtML

[Q64] 提交事务
来源：http://baike.zdbjq.cn/Article/details/gfklsfbdi.sHtML

COMMIT;
来源：http://www.m.share.hesvh.cn/Article/details/gdwzepwnm.sHtML

[Q65] 回滚事务
来源：http://read.share.hesvh.cn/Article/details/gbbaxwurj.sHtML

ROLLBACK;
来源：http://baike.fehbvm.com/Article/details/gwbtgntmz.sHtML

[Q66] 行锁查询
来源：http://www.share.zdbjq.cn/Article/details/guygxyqtx.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mobile.zdbjq.cn/Article/details/gbaustgcn.sHtML

[Q67] 设置隔离级别
来源：http://www.m.share.zdbjq.cn/Article/details/gifcutuzg.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.hesvh.cn/Article/details/gfimlosbi.sHtML

[Q68] 保存点
来源：http://m.share.hesvh.cn/Article/details/gleryiiqk.sHtML

SAVEPOINT sp1;
来源：http://www.share.hesvh.cn/Article/details/gzztbbkmp.sHtML

ROLLBACK TO sp1;
来源：http://baike.fehbvm.com/Article/details/gciqryhiy.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.hesvh.cn/Article/details/gzhdfahtf.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://m.share.zdbjq.cn/Article/details/gjrdtjjsh.sHtML

[Q70] 更新统计信息
来源：http://wap.zdbjq.cn/Article/details/govpqdkgw.sHtML

ANALYZE TABLE users;
来源：http://blog.fehbvm.com/Article/details/garothgzy.sHtML

[Q71] 查看建表语句
来源：http://3g.fehbvm.com/Article/details/gxjwempxr.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.hesvh.cn/Article/details/gmalzutot.sHtML

[Q72] 查看索引
来源：http://www.m.share.zdbjq.cn/Article/details/gfxwdyyjm.sHtML

SHOW INDEX FROM users;
来源：http://m.share.hesvh.cn/Article/details/gomygkskt.sHtML

[Q73] 查看表状态
来源：http://blog.hesvh.cn/Article/details/gsnrjfrok.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.fehbvm.com/Article/details/gvhayyimu.sHtML

[Q74] 强制使用索引
来源：http://wap.hesvh.cn/Article/details/gikmqgybl.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.hesvh.cn/Article/details/gseytoyuq.sHtML

[Q75] 日期格式化
来源：http://read.share.hesvh.cn/Article/details/gnecahptv.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/gzjhvwnfd.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.fehbvm.com/Article/details/gngdjnbdh.sHtML

[Q76] 按天统计
来源：http://m.share.fehbvm.com/Article/details/gituvvnni.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.fehbvm.com/Article/details/gmjnrtamp.sHtML

[Q77] 时间加减
来源：http://www.blog.zdbjq.cn/Article/details/geptectyz.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.zdbjq.cn/Article/details/gunzezzup.sHtML

[Q78] 当前时间
来源：http://wap.zdbjq.cn/Article/details/gxnofzwld.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.hesvh.cn/Article/details/grkcfpdix.sHtML

[Q79] 字符串拼接
来源：http://read.share.zdbjq.cn/Article/details/goqdncejo.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.hesvh.cn/Article/details/grqlzmueg.sHtML

[Q80] 字符串截取
来源：http://mobile.zdbjq.cn/Article/details/grshvwfnl.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mobile.hesvh.cn/Article/details/gqeoorlyh.sHtML

[Q81] 字符串替换
来源：http://www.blog.zdbjq.cn/Article/details/gpdtkwydw.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.fehbvm.com/Article/details/gtsfxjwue.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.fehbvm.com/Article/details/ggpgktevl.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gnliykine.sHtML

[Q83] 大小写转换
来源：http://www.m.share.fehbvm.com/Article/details/gishwlurf.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.zdbjq.cn/Article/details/gmdfzhpfi.sHtML

[Q84] 去除首尾空格
来源：http://m.share.zdbjq.cn/Article/details/gkqrjjrpv.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.zdbjq.cn/Article/details/gflyzphyh.sHtML

[Q85] 数值取整
来源：http://mobile.hesvh.cn/Article/details/ghkqfdpba.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.hesvh.cn/Article/details/gfqhazbme.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.fehbvm.com/Article/details/gnvifnumk.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.zdbjq.cn/Article/details/gyqlzzlva.sHtML

[Q87] JSON 字段做条件
来源：http://blog.zdbjq.cn/Article/details/ghgcigfiv.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.hesvh.cn/Article/details/giadsqaqf.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.hesvh.cn/Article/details/gmuaahhxv.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.fehbvm.com/Article/details/gfhkzlybx.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gsaburzmy.sHtML

[Q89] 判断表是否存在
来源：http://wap.zdbjq.cn/Article/details/gwtzjylqk.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.zdbjq.cn/Article/details/gpwaybbzr.sHtML

[Q90] 生成序号列
来源：http://blog.hesvh.cn/Article/details/gqwiuiiis.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.fehbvm.com/Article/details/ggswgxrmo.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gquuuhjfj.sHtML

R. Bash 专题
来源：http://mobile.zdbjq.cn/Article/details/gfzuuiapu.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gzakcjrxf.sHtML

[R01] shebang 与严格模式
来源：http://www.blog.hesvh.cn/Article/details/gruhdjcja.sHtML

#!/usr/bin/env bash
来源：http://3g.fehbvm.com/Article/details/ghsoopemu.sHtML

set -euo pipefail
来源：http://3g.hesvh.cn/Article/details/gsfvhlddy.sHtML

[R02] 变量赋值与使用
来源：http://read.share.hesvh.cn/Article/details/gpwacwtkr.sHtML

name="Tom"; echo "$name"
来源：http://www.share.fehbvm.com/Article/details/gtkewjsag.sHtML

[R03] 只读变量
来源：http://wap.fehbvm.com/Article/details/gnyllskud.sHtML

readonly PI=3.14
来源：http://blog.fehbvm.com/Article/details/gqzgntvwu.sHtML

[R04] 位置参数
来源：http://www.share.zdbjq.cn/Article/details/gurtpqupz.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.fehbvm.com/Article/details/guflescbn.sHtML

[R05] 参数默认值
来源：http://baike.zdbjq.cn/Article/details/gedrxzkaj.sHtML

name="${1:-default}"
来源：http://www.share.zdbjq.cn/Article/details/gezjipgkj.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.zdbjq.cn/Article/details/gcnshcpat.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.zdbjq.cn/Article/details/gluslmukt.sHtML

[R07] if 判断文件
来源：http://www.share.fehbvm.com/Article/details/gjmgktfxz.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.fehbvm.com/Article/details/gdfxtmgpm.sHtML

[R08] 数值比较
来源：http://www.blog.zdbjq.cn/Article/details/gjetkgsmj.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.zdbjq.cn/Article/details/glpklqqqd.sHtML

[R09] 字符串比较
来源：http://www.blog.fehbvm.com/Article/details/gkfnrjdtj.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.zdbjq.cn/Article/details/giozgwvlp.sHtML

[R10] 正则匹配
来源：http://read.share.zdbjq.cn/Article/details/gonrhrvrp.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.hesvh.cn/Article/details/gihfdthlo.sHtML

[R11] case 多分支
来源：http://www.share.zdbjq.cn/Article/details/gogjxalck.sHtML

case "$1" in
来源：http://m.share.zdbjq.cn/Article/details/ghyocvqaw.sHtML

start) echo "启动" ;;
来源：http://3g.zdbjq.cn/Article/details/gmvktxjls.sHtML

stop)  echo "停止" ;;
来源：http://baike.hesvh.cn/Article/details/giqoslhyy.sHtML

*)     echo "未知命令" ;;
来源：http://baike.fehbvm.com/Article/details/ghpxobuvc.sHtML

esac
来源：http://blog.hesvh.cn/Article/details/gnbeownsp.sHtML

[R12] for 遍历文件
来源：http://baike.fehbvm.com/Article/details/gcgtrptdh.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.fehbvm.com/Article/details/gnmrwuznp.sHtML

[R13] for 计数循环
来源：http://3g.zdbjq.cn/Article/details/gyzmkayvn.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.fehbvm.com/Article/details/ggchaiuko.sHtML

[R14] C 风格 for
来源：http://wap.zdbjq.cn/Article/details/gqogmfbgc.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.hesvh.cn/Article/details/gkgykwbiv.sHtML

[R15] while 逐行读文件
来源：http://read.share.fehbvm.com/Article/details/gxmywhbqk.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.fehbvm.com/Article/details/gswogctqb.sHtML

[R16] until 等待条件
来源：http://www.share.zdbjq.cn/Article/details/gvqimjpga.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.fehbvm.com/Article/details/gvnxvpcon.sHtML

[R17] 数组定义与取值
来源：http://read.share.zdbjq.cn/Article/details/gsjluazhx.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.fehbvm.com/Article/details/gdiqsbaof.sHtML

[R18] 遍历数组
来源：http://www.blog.fehbvm.com/Article/details/gvtbbgkjl.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.zdbjq.cn/Article/details/gyljngife.sHtML

[R19] 数组长度
来源：http://blog.fehbvm.com/Article/details/gngjferhs.sHtML

echo "${#arr[@]}"
来源：http://wap.fehbvm.com/Article/details/glfoqhcln.sHtML

[R20] 关联数组（字典）
来源：http://mobile.zdbjq.cn/Article/details/geiaviinj.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.hesvh.cn/Article/details/gkxkwsgaq.sHtML

[R21] 字符串长度
来源：http://3g.zdbjq.cn/Article/details/gggpnyrkn.sHtML

echo "${#s}"
来源：http://baike.zdbjq.cn/Article/details/gbuyuydlz.sHtML

[R22] 截取子串
来源：http://read.share.fehbvm.com/Article/details/gzayhhzxo.sHtML

echo "${s:0:5}"
来源：http://wap.hesvh.cn/Article/details/gdexngmnv.sHtML

[R23] 字符串替换
来源：http://www.blog.fehbvm.com/Article/details/gevoevxky.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.zdbjq.cn/Article/details/gablulckc.sHtML

[R24] 大小写转换
来源：http://www.blog.fehbvm.com/Article/details/gsqdfrsjz.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.fehbvm.com/Article/details/gbrwjiaxm.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.zdbjq.cn/Article/details/ggkpnuhft.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.zdbjq.cn/Article/details/giuhyjtmw.sHtML

[R26] 命令替换
来源：http://www.share.hesvh.cn/Article/details/gtaeaaaza.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.zdbjq.cn/Article/details/gravvtjtg.sHtML

[R27] 算术展开
来源：http://wap.zdbjq.cn/Article/details/gsuiqvjci.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.fehbvm.com/Article/details/gnoajuwod.sHtML

[R28] 浮点运算
来源：http://baike.hesvh.cn/Article/details/gguqzgukn.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.hesvh.cn/Article/details/gfoxbbesm.sHtML

[R29] 定义函数
来源：http://m.share.hesvh.cn/Article/details/gluqphzsi.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.hesvh.cn/Article/details/gjlgayism.sHtML

[R30] 函数返回状态码
来源：http://3g.zdbjq.cn/Article/details/giedvvuup.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.fehbvm.com/Article/details/gvcohaswy.sHtML

[R31] 局部变量
来源：http://3g.zdbjq.cn/Article/details/ggbdxtoae.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.hesvh.cn/Article/details/gtfvtzwsx.sHtML

[R32] 参数个数校验
来源：http://m.share.hesvh.cn/Article/details/gfmtxmbqh.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.hesvh.cn/Article/details/gtqaykncf.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.zdbjq.cn/Article/details/gvcyzabdm.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.fehbvm.com/Article/details/gfsybkoip.sHtML

[R34] 退出时清理
来源：http://mobile.hesvh.cn/Article/details/gwpblpaau.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fehbvm.com/Article/details/ghtwnwmws.sHtML

[R35] 后台执行并等待
来源：http://read.share.fehbvm.com/Article/details/gkizloozw.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.fehbvm.com/Article/details/gnzdotyuc.sHtML

[R36] 并发执行多个任务
来源：http://3g.hesvh.cn/Article/details/gqqniqgvb.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.zdbjq.cn/Article/details/gwfjzhgrl.sHtML

[R37] 把输出赋给变量
来源：http://www.share.zdbjq.cn/Article/details/gzpyugarc.sHtML

files=$(ls -1)
来源：http://mobile.hesvh.cn/Article/details/gsxrlwtgi.sHtML

[R38] 管道串联
来源：http://blog.fehbvm.com/Article/details/gmixetgjn.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.hesvh.cn/Article/details/gatxkpxxy.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.zdbjq.cn/Article/details/gfspoodvz.sHtML

cmd > out.log 2>&1
来源：http://baike.zdbjq.cn/Article/details/gpehwakwq.sHtML

[R40] 追加写日志
来源：http://www.share.zdbjq.cn/Article/details/goiigyfbe.sHtML

echo "log" >> out.log
来源：http://mobile.zdbjq.cn/Article/details/gzlqzoifb.sHtML

[R41] 丢弃输出
来源：http://read.share.hesvh.cn/Article/details/gzyvshlop.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.zdbjq.cn/Article/details/gvmnxqkhl.sHtML

[R42] 输入重定向
来源：http://mobile.hesvh.cn/Article/details/grjyynmyd.sHtML

wc -l < a.txt
来源：http://mobile.fehbvm.com/Article/details/giktdrpvq.sHtML

[R43] 按名字查找文件
来源：http://m.share.zdbjq.cn/Article/details/gyhwtceck.sHtML

find . -name "*.log" -type f
来源：http://mobile.fehbvm.com/Article/details/gyhqpdjzr.sHtML

[R44] 按修改时间查找
来源：http://wap.hesvh.cn/Article/details/gxvsvceau.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.zdbjq.cn/Article/details/gkwbqiwco.sHtML

[R45] 批量删除
来源：http://wap.fehbvm.com/Article/details/gnbocqrkz.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.zdbjq.cn/Article/details/gdlqjpbxs.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.fehbvm.com/Article/details/gkjfrygxg.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.fehbvm.com/Article/details/gzxzgffqh.sHtML

[R47] sed 单行替换
来源：http://baike.hesvh.cn/Article/details/gkxdhmmcb.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.zdbjq.cn/Article/details/glqthpmgt.sHtML

[R48] awk 取指定列
来源：http://www.m.share.fehbvm.com/Article/details/gvvkqgygp.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.hesvh.cn/Article/details/garzyfhzq.sHtML

[R49] awk 带条件
来源：http://baike.hesvh.cn/Article/details/gwsftutua.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.zdbjq.cn/Article/details/gzwppojpj.sHtML

[R50] awk 求和
来源：http://www.m.share.zdbjq.cn/Article/details/gmxcueaup.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.zdbjq.cn/Article/details/gssalswnf.sHtML

[R51] 排序去重取前几
来源：http://3g.hesvh.cn/Article/details/gpoqmglhp.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.hesvh.cn/Article/details/gkipcuacz.sHtML

[R52] 统计行数
来源：http://blog.hesvh.cn/Article/details/gfwfhyrgr.sHtML

wc -l a.txt
来源：http://3g.fehbvm.com/Article/details/gendnxjec.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.hesvh.cn/Article/details/gsbmvjjwx.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.hesvh.cn/Article/details/giypzrqbi.sHtML

[R54] 比较两个文件
来源：http://www.share.zdbjq.cn/Article/details/gmoknpjwn.sHtML

diff a.txt b.txt
来源：http://baike.hesvh.cn/Article/details/gxvdizgeq.sHtML

[R55] 压缩与解压
来源：http://3g.hesvh.cn/Article/details/gimfmdlkq.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.zdbjq.cn/Article/details/glpunbfqr.sHtML

[R56] 远程拷贝
来源：http://m.share.zdbjq.cn/Article/details/gwoczjjak.sHtML

scp file user@host:/path/
来源：http://3g.zdbjq.cn/Article/details/gytlurdej.sHtML

[R57] 远程执行命令
来源：http://www.blog.fehbvm.com/Article/details/gjpnmocxp.sHtML

ssh user@host 'uptime'
来源：http://blog.hesvh.cn/Article/details/gnajfnwup.sHtML

[R58] 下载文件
来源：http://blog.zdbjq.cn/Article/details/grvchhgwo.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.hesvh.cn/Article/details/gealmxodp.sHtML

[R59] 发 POST JSON
来源：http://m.share.zdbjq.cn/Article/details/gmoprolfd.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.zdbjq.cn/Article/details/gxwsptwyn.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.zdbjq.cn/Article/details/gpewfkchj.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.fehbvm.com/Article/details/gltmrtqyr.sHtML

[R61] 磁盘占用
来源：http://mobile.hesvh.cn/Article/details/gukjnbbpt.sHtML

df -h;  du -sh *
来源：http://read.share.zdbjq.cn/Article/details/gmzsenlko.sHtML

[R62] 找最占空间的文件
来源：http://m.share.zdbjq.cn/Article/details/gclpwpqxd.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.zdbjq.cn/Article/details/gwvdtinxv.sHtML

[R63] 内存与进程
来源：http://m.share.hesvh.cn/Article/details/gfzowkstm.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.zdbjq.cn/Article/details/gbojkiglu.sHtML

[R64] 结束进程
来源：http://baike.fehbvm.com/Article/details/gjuohdsrl.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.zdbjq.cn/Article/details/gqyabqcxa.sHtML

[R65] 查看端口占用
来源：http://3g.hesvh.cn/Article/details/gqhjkqykf.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.hesvh.cn/Article/details/glkxlsiba.sHtML

[R66] 定时任务
来源：http://baike.zdbjq.cn/Article/details/gasjqxbim.sHtML

crontab -e;  crontab -l
来源：http://m.share.zdbjq.cn/Article/details/gyhhszpyc.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.fehbvm.com/Article/details/gvwiavmqi.sHtML

openssl rand -hex 16
来源：http://www.share.hesvh.cn/Article/details/grlqftokp.sHtML

[R68] 计算文件校验值
来源：http://baike.zdbjq.cn/Article/details/gqeezsmhv.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.hesvh.cn/Article/details/gqsxgilbs.sHtML

[R69] 生成随机密码
来源：http://3g.zdbjq.cn/Article/details/gihbrwxti.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.fehbvm.com/Article/details/gwkgzrnba.sHtML

[R70] 时间戳与互转
来源：http://wap.hesvh.cn/Article/details/gwslhidof.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.fehbvm.com/Article/details/gcbvclzlv.sHtML

[R71] 日期格式化
来源：http://blog.hesvh.cn/Article/details/gfbwdwgzu.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.hesvh.cn/Article/details/gfujjnjgy.sHtML

[R72] 等待端口就绪
来源：http://baike.hesvh.cn/Article/details/gmviyjezt.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.fehbvm.com/Article/details/gfzdbcrna.sHtML

[R73] 分割大日志
来源：http://www.m.share.zdbjq.cn/Article/details/gxnrwhnaq.sHtML

split -l 1000 big.log part_
来源：http://mobile.hesvh.cn/Article/details/gtmqxmdaw.sHtML

[R74] 批量重命名
来源：http://blog.fehbvm.com/Article/details/gcihdriuy.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.zdbjq.cn/Article/details/gfhifqnnn.sHtML

[R75] 导出环境变量
来源：http://www.blog.fehbvm.com/Article/details/ggyxallrs.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.fehbvm.com/Article/details/gwapyumwr.sHtML

[R76] 使用临时文件
来源：http://baike.hesvh.cn/Article/details/gpryeipxc.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.zdbjq.cn/Article/details/gsoizjxxo.sHtML

[R77] 读取用户输入
来源：http://blog.fehbvm.com/Article/details/gtdvpsusk.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.hesvh.cn/Article/details/gtwfydceh.sHtML

[R78] 交互式菜单
来源：http://3g.zdbjq.cn/Article/details/ghbpgyesc.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.hesvh.cn/Article/details/gzyahyvly.sHtML

[R79] 解析命令行选项
来源：http://www.blog.zdbjq.cn/Article/details/gdeefxzzs.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.fehbvm.com/Article/details/gnichamew.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.zdbjq.cn/Article/details/grvwtikdo.sHtML

time ./run.sh
来源：http://m.share.fehbvm.com/Article/details/gbimfmefw.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/goobklyix.sHtML

S. C / C++ 专题
来源：http://read.share.fehbvm.com/Article/details/gjjrekazo.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gtbrbucjy.sHtML

[S01] C：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gsvlgremb.sHtML

#include <stdio.h>
来源：http://mobile.fehbvm.com/Article/details/giphjlsjz.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.fehbvm.com/Article/details/glucenlzw.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.hesvh.cn/Article/details/ghimtvzno.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.zdbjq.cn/Article/details/gmjklbjel.sHtML

[S03] C：读入整数
来源：http://wap.fehbvm.com/Article/details/gildbbrml.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.hesvh.cn/Article/details/gzxemrjgh.sHtML

[S04] C：字符串复制
来源：http://www.m.share.zdbjq.cn/Article/details/gulhqkyzl.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.hesvh.cn/Article/details/gsukgwumh.sHtML

[S05] C：字符串长度
来源：http://read.share.hesvh.cn/Article/details/grwzfdrhl.sHtML

strlen(s)
来源：http://blog.fehbvm.com/Article/details/gyhuhgpla.sHtML

[S06] C：字符串比较
来源：http://www.share.hesvh.cn/Article/details/gxebxxouz.sHtML

strcmp(a, b) == 0
来源：http://mobile.fehbvm.com/Article/details/ggbesqaxf.sHtML

[S07] C：数组遍历求和
来源：http://www.share.fehbvm.com/Article/details/ghzxhzwxl.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.hesvh.cn/Article/details/gobqueply.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.zdbjq.cn/Article/details/glhecmbry.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.hesvh.cn/Article/details/gnskzlnnv.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.fehbvm.com/Article/details/guedbueqm.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.hesvh.cn/Article/details/gijcpmhkg.sHtML

[S10] C：指针与解引用
来源：http://wap.fehbvm.com/Article/details/ggjblzasq.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.fehbvm.com/Article/details/gdfooejhl.sHtML

[S11] C：逐行读文件
来源：http://baike.hesvh.cn/Article/details/gzudsdjhh.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.zdbjq.cn/Article/details/gmhfqlzur.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.zdbjq.cn/Article/details/gerouhctg.sHtML

fclose(f);
来源：http://read.share.fehbvm.com/Article/details/grqlpflsy.sHtML

[S12] C：写文件
来源：http://www.m.share.hesvh.cn/Article/details/gyjauouas.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.hesvh.cn/Article/details/gmyhjvhki.sHtML

[S13] C：宏定义
来源：http://3g.zdbjq.cn/Article/details/gpuleedes.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.zdbjq.cn/Article/details/gkwfuvxpg.sHtML

[S14] C：枚举
来源：http://www.m.share.fehbvm.com/Article/details/giykdedlm.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.fehbvm.com/Article/details/gpqlsqnvy.sHtML

[S15] C：类型转换
来源：http://www.blog.hesvh.cn/Article/details/gsdvuucom.sHtML

(double) a / b
来源：http://3g.fehbvm.com/Article/details/gsvyrignr.sHtML

[S16] C：位操作置位
来源：http://mobile.hesvh.cn/Article/details/gazooqbhz.sHtML


<!-- 参考信息 -->