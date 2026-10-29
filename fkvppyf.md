代发 wailian999

SELECT u.name, o.amount FROM users u
来源：http://www.share.fehbvm.com/Article/details/gftvwybqv.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.zdbjq.cn/Article/details/garrfyxrp.sHtML

[Q43] 标量子查询
来源：http://www.blog.hesvh.cn/Article/details/gylhtpyhs.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://3g.hesvh.cn/Article/details/gjhrowerb.sHtML

[Q44] IN 子查询
来源：http://www.share.zdbjq.cn/Article/details/gwflllumd.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mobile.fehbvm.com/Article/details/glbigirwl.sHtML

[Q45] EXISTS 判断存在
来源：http://read.share.fehbvm.com/Article/details/gbsotspvn.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.zdbjq.cn/Article/details/gddkvpcbl.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.zdbjq.cn/Article/details/gksddpdwi.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.fehbvm.com/Article/details/ghmaxagwn.sHtML

[Q47] 与平均值比较
来源：http://www.share.fehbvm.com/Article/details/gpsmighpe.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wap.zdbjq.cn/Article/details/gbaumyjzo.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.hesvh.cn/Article/details/gmpbougvd.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://m.share.hesvh.cn/Article/details/gdhljjdcd.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.fehbvm.com/Article/details/gkzagexdm.sHtML

[Q49] 更新单行
来源：http://www.m.share.fehbvm.com/Article/details/gpqxrvcik.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://blog.hesvh.cn/Article/details/gmmzzcprl.sHtML

[Q50] 批量更新
来源：http://www.share.fehbvm.com/Article/details/gugvdzgmc.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.m.share.hesvh.cn/Article/details/gqiitxiwa.sHtML

[Q51] 用子查询更新
来源：http://3g.hesvh.cn/Article/details/gkcflmiif.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gcmfvvmjd.sHtML

[Q52] 删除指定行
来源：http://www.share.zdbjq.cn/Article/details/gzizhcysa.sHtML

DELETE FROM users WHERE id = 10;
来源：http://baike.zdbjq.cn/Article/details/gakljoyec.sHtML

[Q53] 按条件删除
来源：http://baike.fehbvm.com/Article/details/gfvnfkqrj.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.zdbjq.cn/Article/details/gyfaiapvz.sHtML

[Q54] 清空表
来源：http://read.share.fehbvm.com/Article/details/ggcspynlc.sHtML

TRUNCATE TABLE logs;
来源：http://www.blog.fehbvm.com/Article/details/guqerimga.sHtML

[Q55] 排名（并列占位）
来源：http://wap.hesvh.cn/Article/details/gnajtsukc.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.fehbvm.com/Article/details/gzxvbnjxy.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.m.share.zdbjq.cn/Article/details/gjrxkibud.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.fehbvm.com/Article/details/ggkfzlvdm.sHtML

[Q57] 行号
来源：http://read.share.zdbjq.cn/Article/details/gqnbixbge.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://read.share.hesvh.cn/Article/details/gudqjbggc.sHtML

[Q58] 累计求和
来源：http://wap.zdbjq.cn/Article/details/grvnfyufu.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/giplfwkhy.sHtML

[Q59] 分组内累计
来源：http://mobile.zdbjq.cn/Article/details/gbgxhxitv.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://m.share.fehbvm.com/Article/details/gxxoaiatv.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.blog.hesvh.cn/Article/details/gijpfvnyl.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://blog.fehbvm.com/Article/details/gbovxziil.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://blog.zdbjq.cn/Article/details/gzqkdjpse.sHtML

[Q61] 移动平均
来源：http://m.share.hesvh.cn/Article/details/grliwtjcf.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.fehbvm.com/Article/details/gxxowlisd.sHtML

[Q62] 分组占比
来源：http://wap.hesvh.cn/Article/details/ghhrlpofr.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.zdbjq.cn/Article/details/gyefaqoch.sHtML

[Q63] 开启事务
来源：http://m.share.zdbjq.cn/Article/details/gvzuvcemn.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.zdbjq.cn/Article/details/ghywxivcz.sHtML

[Q64] 提交事务
来源：http://baike.hesvh.cn/Article/details/grztyjrbe.sHtML

COMMIT;
来源：http://blog.zdbjq.cn/Article/details/gmbtodppi.sHtML

[Q65] 回滚事务
来源：http://baike.zdbjq.cn/Article/details/gtotgmaxs.sHtML

ROLLBACK;
来源：http://wap.fehbvm.com/Article/details/gpnidftul.sHtML

[Q66] 行锁查询
来源：http://mobile.fehbvm.com/Article/details/gpjumldxg.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.fehbvm.com/Article/details/gditjknnc.sHtML

[Q67] 设置隔离级别
来源：http://3g.hesvh.cn/Article/details/gscovwgji.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.m.share.fehbvm.com/Article/details/giyhcfiwx.sHtML

[Q68] 保存点
来源：http://mobile.fehbvm.com/Article/details/gokkyymjo.sHtML

SAVEPOINT sp1;
来源：http://mobile.zdbjq.cn/Article/details/glzpifsbi.sHtML

ROLLBACK TO sp1;
来源：http://read.share.fehbvm.com/Article/details/gpafzmdnv.sHtML

[Q69] 查看执行计划
来源：http://baike.hesvh.cn/Article/details/glydtppdr.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.zdbjq.cn/Article/details/gdakqrqzg.sHtML

[Q70] 更新统计信息
来源：http://wap.fehbvm.com/Article/details/gimelzcxv.sHtML

ANALYZE TABLE users;
来源：http://baike.hesvh.cn/Article/details/gnqsvwwag.sHtML

[Q71] 查看建表语句
来源：http://read.share.hesvh.cn/Article/details/gwujkmucr.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.fehbvm.com/Article/details/gccehjlmu.sHtML

[Q72] 查看索引
来源：http://mobile.zdbjq.cn/Article/details/gtwerdpfs.sHtML

SHOW INDEX FROM users;
来源：http://mobile.hesvh.cn/Article/details/grgyfukbp.sHtML

[Q73] 查看表状态
来源：http://blog.fehbvm.com/Article/details/gnnjqlstx.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.zdbjq.cn/Article/details/gwetiwyfc.sHtML

[Q74] 强制使用索引
来源：http://m.share.zdbjq.cn/Article/details/gkjwhvpum.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://read.share.hesvh.cn/Article/details/grsqusqln.sHtML

[Q75] 日期格式化
来源：http://m.share.hesvh.cn/Article/details/goobmceji.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/gamyalcmg.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mobile.fehbvm.com/Article/details/gyxzkssek.sHtML

[Q76] 按天统计
来源：http://mobile.zdbjq.cn/Article/details/gzbdwzvnr.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://3g.hesvh.cn/Article/details/glwfifzkm.sHtML

[Q77] 时间加减
来源：http://wap.fehbvm.com/Article/details/guuieqxac.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.zdbjq.cn/Article/details/gboebamkt.sHtML

[Q78] 当前时间
来源：http://www.m.share.zdbjq.cn/Article/details/gxvzpewqm.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.hesvh.cn/Article/details/grztilnwi.sHtML

[Q79] 字符串拼接
来源：http://www.share.hesvh.cn/Article/details/gkkqpyxqm.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.fehbvm.com/Article/details/gfxhrpuxm.sHtML

[Q80] 字符串截取
来源：http://wap.zdbjq.cn/Article/details/ggttqslyx.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mobile.fehbvm.com/Article/details/gblnvqjgw.sHtML

[Q81] 字符串替换
来源：http://3g.hesvh.cn/Article/details/gjoqrstcg.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.hesvh.cn/Article/details/grolxdehf.sHtML

[Q82] 字符长度与字节长度
来源：http://blog.hesvh.cn/Article/details/gxujqjkid.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://baike.hesvh.cn/Article/details/gvpsltwsh.sHtML

[Q83] 大小写转换
来源：http://read.share.zdbjq.cn/Article/details/gbkwnuyvr.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.hesvh.cn/Article/details/gzjakzytq.sHtML

[Q84] 去除首尾空格
来源：http://blog.hesvh.cn/Article/details/ghuaoggnk.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.hesvh.cn/Article/details/gshondybp.sHtML

[Q85] 数值取整
来源：http://wap.fehbvm.com/Article/details/glrsnucor.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.fehbvm.com/Article/details/ggctapaem.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.fehbvm.com/Article/details/gusorgqed.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.zdbjq.cn/Article/details/gmjygjkhw.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.zdbjq.cn/Article/details/gnnrgkzdg.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.fehbvm.com/Article/details/gtetedftz.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.share.zdbjq.cn/Article/details/gymsayzas.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.hesvh.cn/Article/details/givnrqawn.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.hesvh.cn/Article/details/ghtxgcjjz.sHtML

[Q89] 判断表是否存在
来源：http://www.share.hesvh.cn/Article/details/ghboqkgwz.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.fehbvm.com/Article/details/gfyjwillk.sHtML

[Q90] 生成序号列
来源：http://baike.fehbvm.com/Article/details/glpmdqckc.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://3g.fehbvm.com/Article/details/gmzlvslga.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/guquhucti.sHtML

R. Bash 专题
来源：http://wap.zdbjq.cn/Article/details/glpkvwyxm.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/ghitxhnkb.sHtML

[R01] shebang 与严格模式
来源：http://baike.fehbvm.com/Article/details/gtkshmasa.sHtML

#!/usr/bin/env bash
来源：http://3g.zdbjq.cn/Article/details/gmkoaxuiq.sHtML

set -euo pipefail
来源：http://wap.hesvh.cn/Article/details/gjtczvlfx.sHtML

[R02] 变量赋值与使用
来源：http://m.share.fehbvm.com/Article/details/gxnjvwalx.sHtML

name="Tom"; echo "$name"
来源：http://3g.zdbjq.cn/Article/details/gareszayi.sHtML

[R03] 只读变量
来源：http://mobile.hesvh.cn/Article/details/gdlniytjb.sHtML

readonly PI=3.14
来源：http://mobile.fehbvm.com/Article/details/gjebptwbj.sHtML

[R04] 位置参数
来源：http://blog.zdbjq.cn/Article/details/ghlhikbkc.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.zdbjq.cn/Article/details/gtbrrdwgx.sHtML

[R05] 参数默认值
来源：http://m.share.fehbvm.com/Article/details/gzylavoqs.sHtML

name="${1:-default}"
来源：http://www.share.zdbjq.cn/Article/details/gbeltiqna.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.zdbjq.cn/Article/details/gnkjxtzgr.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.fehbvm.com/Article/details/gbnjhxbca.sHtML

[R07] if 判断文件
来源：http://3g.fehbvm.com/Article/details/gcvtkeiqa.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.hesvh.cn/Article/details/guwinyktq.sHtML

[R08] 数值比较
来源：http://baike.fehbvm.com/Article/details/gehexgitd.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.hesvh.cn/Article/details/gbcajjsng.sHtML

[R09] 字符串比较
来源：http://read.share.fehbvm.com/Article/details/gbctvukck.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.hesvh.cn/Article/details/gappqgqev.sHtML

[R10] 正则匹配
来源：http://www.m.share.zdbjq.cn/Article/details/gwlsegund.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.hesvh.cn/Article/details/ggkldorti.sHtML

[R11] case 多分支
来源：http://www.blog.zdbjq.cn/Article/details/gwiowutpt.sHtML

case "$1" in
来源：http://baike.hesvh.cn/Article/details/gzlafbmgp.sHtML

start) echo "启动" ;;
来源：http://baike.hesvh.cn/Article/details/gkfpjqkup.sHtML

stop)  echo "停止" ;;
来源：http://baike.hesvh.cn/Article/details/ghtwtkxqz.sHtML

*)     echo "未知命令" ;;
来源：http://3g.zdbjq.cn/Article/details/ghfotdcxf.sHtML

esac
来源：http://www.share.zdbjq.cn/Article/details/gchskoezt.sHtML

[R12] for 遍历文件
来源：http://mobile.fehbvm.com/Article/details/gbcnqxfkt.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.fehbvm.com/Article/details/gzgpkznri.sHtML

[R13] for 计数循环
来源：http://mobile.fehbvm.com/Article/details/gjqjdaspf.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.hesvh.cn/Article/details/gpuhliwrf.sHtML

[R14] C 风格 for
来源：http://www.share.fehbvm.com/Article/details/gxpyekpne.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.hesvh.cn/Article/details/glmvrvltp.sHtML

[R15] while 逐行读文件
来源：http://www.share.fehbvm.com/Article/details/gxyolunaf.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.hesvh.cn/Article/details/gnoxzmjst.sHtML

[R16] until 等待条件
来源：http://mobile.zdbjq.cn/Article/details/gvbmpkbju.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.zdbjq.cn/Article/details/gvqovefkt.sHtML

[R17] 数组定义与取值
来源：http://baike.fehbvm.com/Article/details/gxfmjfgbp.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.zdbjq.cn/Article/details/gbnrvqbgc.sHtML

[R18] 遍历数组
来源：http://m.share.zdbjq.cn/Article/details/gglloptaj.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.fehbvm.com/Article/details/gvjzjtcfs.sHtML

[R19] 数组长度
来源：http://www.blog.zdbjq.cn/Article/details/ggwdqxoau.sHtML

echo "${#arr[@]}"
来源：http://wap.fehbvm.com/Article/details/gwzihinnm.sHtML

[R20] 关联数组（字典）
来源：http://baike.zdbjq.cn/Article/details/gpzgcsthy.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.zdbjq.cn/Article/details/ggehzrayf.sHtML

[R21] 字符串长度
来源：http://3g.fehbvm.com/Article/details/gwkbzjzkk.sHtML

echo "${#s}"
来源：http://3g.fehbvm.com/Article/details/gswmbpiwl.sHtML

[R22] 截取子串
来源：http://blog.zdbjq.cn/Article/details/gbimwdksj.sHtML

echo "${s:0:5}"
来源：http://www.m.share.hesvh.cn/Article/details/gytmmwlud.sHtML

[R23] 字符串替换
来源：http://m.share.fehbvm.com/Article/details/golssxtge.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.fehbvm.com/Article/details/gpzqdefjb.sHtML

[R24] 大小写转换
来源：http://m.share.fehbvm.com/Article/details/gbmvbmcbe.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.zdbjq.cn/Article/details/glfidedtk.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.hesvh.cn/Article/details/ggxobsfjl.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.zdbjq.cn/Article/details/gmxkyltes.sHtML

[R26] 命令替换
来源：http://wap.hesvh.cn/Article/details/gzkwiafmf.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.hesvh.cn/Article/details/gsbydasvq.sHtML

[R27] 算术展开
来源：http://3g.fehbvm.com/Article/details/gwmadoxea.sHtML

echo $((1 + 2 * 3))
来源：http://baike.zdbjq.cn/Article/details/glezltwej.sHtML

[R28] 浮点运算
来源：http://www.blog.zdbjq.cn/Article/details/gahklqhdh.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.zdbjq.cn/Article/details/gzxazsnzj.sHtML

[R29] 定义函数
来源：http://www.share.hesvh.cn/Article/details/gpcpnajkg.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.zdbjq.cn/Article/details/gxzczrejx.sHtML

[R30] 函数返回状态码
来源：http://baike.fehbvm.com/Article/details/gxkfgnoqo.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.zdbjq.cn/Article/details/gvlcsawma.sHtML

[R31] 局部变量
来源：http://m.share.zdbjq.cn/Article/details/gmhpafjtn.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gjfemkznf.sHtML

[R32] 参数个数校验
来源：http://www.share.zdbjq.cn/Article/details/glvbelfva.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.hesvh.cn/Article/details/guefcaflt.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.hesvh.cn/Article/details/gakohhpiq.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.zdbjq.cn/Article/details/gmnqxokvp.sHtML

[R34] 退出时清理
来源：http://blog.hesvh.cn/Article/details/gmsfiwkzg.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.fehbvm.com/Article/details/gjnsbnlxv.sHtML

[R35] 后台执行并等待
来源：http://baike.fehbvm.com/Article/details/ghzcyzrwr.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.zdbjq.cn/Article/details/gqkurtzue.sHtML

[R36] 并发执行多个任务
来源：http://read.share.fehbvm.com/Article/details/gcailqixj.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.fehbvm.com/Article/details/gituiwdkw.sHtML

[R37] 把输出赋给变量
来源：http://m.share.hesvh.cn/Article/details/gcdzypkbu.sHtML

files=$(ls -1)
来源：http://baike.fehbvm.com/Article/details/gslgispsm.sHtML

[R38] 管道串联
来源：http://blog.fehbvm.com/Article/details/glmvduoji.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.zdbjq.cn/Article/details/giokfsyqe.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.hesvh.cn/Article/details/gkkgvljfi.sHtML

cmd > out.log 2>&1
来源：http://www.blog.zdbjq.cn/Article/details/ghkfgopld.sHtML

[R40] 追加写日志
来源：http://m.share.hesvh.cn/Article/details/gbysbofny.sHtML

echo "log" >> out.log
来源：http://www.m.share.fehbvm.com/Article/details/gopbkdgfl.sHtML

[R41] 丢弃输出
来源：http://3g.zdbjq.cn/Article/details/gvllhcvat.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.hesvh.cn/Article/details/ghcyfgett.sHtML

[R42] 输入重定向
来源：http://blog.fehbvm.com/Article/details/gcgqzaotg.sHtML

wc -l < a.txt
来源：http://baike.hesvh.cn/Article/details/gwjzmbvjo.sHtML

[R43] 按名字查找文件
来源：http://www.share.fehbvm.com/Article/details/gzbfsunyo.sHtML

find . -name "*.log" -type f
来源：http://wap.zdbjq.cn/Article/details/ghghdkhfr.sHtML

[R44] 按修改时间查找
来源：http://www.blog.zdbjq.cn/Article/details/gzazzxuwj.sHtML

find . -mtime -7 -type f
来源：http://wap.hesvh.cn/Article/details/gvmlzcbwk.sHtML

[R45] 批量删除
来源：http://baike.zdbjq.cn/Article/details/glydsxzvi.sHtML

find . -name "*.tmp" -delete
来源：http://3g.zdbjq.cn/Article/details/gzgpkbfjn.sHtML

[R46] 递归替换文件内容
来源：http://read.share.zdbjq.cn/Article/details/gqzmrkzvt.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.fehbvm.com/Article/details/gayyihurb.sHtML

[R47] sed 单行替换
来源：http://read.share.fehbvm.com/Article/details/gftalizbj.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.fehbvm.com/Article/details/gpklkhmvj.sHtML

[R48] awk 取指定列
来源：http://www.blog.zdbjq.cn/Article/details/gjtjyebvw.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.fehbvm.com/Article/details/gqopgwlit.sHtML

[R49] awk 带条件
来源：http://m.share.hesvh.cn/Article/details/gawjvocyb.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.zdbjq.cn/Article/details/gulxdjrug.sHtML

[R50] awk 求和
来源：http://blog.fehbvm.com/Article/details/gzcwtdxtr.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.hesvh.cn/Article/details/gnzaxfvpy.sHtML

[R51] 排序去重取前几
来源：http://www.share.hesvh.cn/Article/details/gbbrmxvtz.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.fehbvm.com/Article/details/gjwocyvhr.sHtML

[R52] 统计行数
来源：http://wap.zdbjq.cn/Article/details/gsowziezq.sHtML

wc -l a.txt
来源：http://www.blog.zdbjq.cn/Article/details/gnmrasjtp.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.hesvh.cn/Article/details/gdyzwgiyw.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.hesvh.cn/Article/details/gnsktfdaq.sHtML

[R54] 比较两个文件
来源：http://wap.hesvh.cn/Article/details/ggxpdpemt.sHtML

diff a.txt b.txt
来源：http://mobile.zdbjq.cn/Article/details/gcmwoipmp.sHtML

[R55] 压缩与解压
来源：http://mobile.zdbjq.cn/Article/details/gdiukcjlw.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.zdbjq.cn/Article/details/gsqrcvngp.sHtML

[R56] 远程拷贝
来源：http://wap.hesvh.cn/Article/details/gdjdplfsh.sHtML

scp file user@host:/path/
来源：http://m.share.hesvh.cn/Article/details/gtsgigrcl.sHtML

[R57] 远程执行命令
来源：http://www.m.share.fehbvm.com/Article/details/ggekqycjt.sHtML

ssh user@host 'uptime'
来源：http://wap.hesvh.cn/Article/details/ggxesiofr.sHtML

[R58] 下载文件
来源：http://read.share.fehbvm.com/Article/details/goiemjpjo.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.zdbjq.cn/Article/details/gfqgufbcg.sHtML

[R59] 发 POST JSON
来源：http://mobile.fehbvm.com/Article/details/gzobdmkuu.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.hesvh.cn/Article/details/gtdujbypo.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.fehbvm.com/Article/details/gnpfrglbt.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.zdbjq.cn/Article/details/gddcbblrv.sHtML

[R61] 磁盘占用
来源：http://baike.hesvh.cn/Article/details/gfybxevdm.sHtML

df -h;  du -sh *
来源：http://3g.fehbvm.com/Article/details/gtllfmptk.sHtML

[R62] 找最占空间的文件
来源：http://www.share.hesvh.cn/Article/details/gdkygcdzi.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.hesvh.cn/Article/details/gwofubzhc.sHtML

[R63] 内存与进程
来源：http://www.blog.zdbjq.cn/Article/details/gpxagxskw.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.fehbvm.com/Article/details/gjgeffehn.sHtML

[R64] 结束进程
来源：http://mobile.hesvh.cn/Article/details/gqjyyvwcu.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.zdbjq.cn/Article/details/gurdxrxpe.sHtML

[R65] 查看端口占用
来源：http://www.share.fehbvm.com/Article/details/giaqananj.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.fehbvm.com/Article/details/ggiegkpow.sHtML

[R66] 定时任务
来源：http://www.m.share.zdbjq.cn/Article/details/gwrxxwfwk.sHtML

crontab -e;  crontab -l
来源：http://www.blog.fehbvm.com/Article/details/gquutcmyv.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.hesvh.cn/Article/details/gbvgcsrrj.sHtML

openssl rand -hex 16
来源：http://blog.fehbvm.com/Article/details/gxwondsrc.sHtML

[R68] 计算文件校验值
来源：http://3g.zdbjq.cn/Article/details/gxlleealk.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.fehbvm.com/Article/details/govzbyrsc.sHtML

[R69] 生成随机密码
来源：http://www.m.share.hesvh.cn/Article/details/gpajterga.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.hesvh.cn/Article/details/gyeehsnpv.sHtML

[R70] 时间戳与互转
来源：http://blog.zdbjq.cn/Article/details/gndyagvey.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.fehbvm.com/Article/details/ghronahyc.sHtML

[R71] 日期格式化
来源：http://www.blog.fehbvm.com/Article/details/guqesjfxy.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.hesvh.cn/Article/details/gbcwfnqpn.sHtML

[R72] 等待端口就绪
来源：http://mobile.zdbjq.cn/Article/details/gfumzowmc.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.hesvh.cn/Article/details/ghepccowl.sHtML

[R73] 分割大日志
来源：http://mobile.hesvh.cn/Article/details/goeqearhh.sHtML

split -l 1000 big.log part_
来源：http://3g.fehbvm.com/Article/details/glfmvfknj.sHtML

[R74] 批量重命名
来源：http://blog.fehbvm.com/Article/details/gcrvjeltg.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.zdbjq.cn/Article/details/guhyyieqb.sHtML

[R75] 导出环境变量
来源：http://www.blog.fehbvm.com/Article/details/gypzntvfz.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.hesvh.cn/Article/details/gmcypapyo.sHtML

[R76] 使用临时文件
来源：http://3g.hesvh.cn/Article/details/grhwkdhho.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fehbvm.com/Article/details/guklaanqw.sHtML

[R77] 读取用户输入
来源：http://baike.fehbvm.com/Article/details/gmfmhkqec.sHtML

read -rp "请输入: " ans
来源：http://mobile.fehbvm.com/Article/details/gkunxtkmf.sHtML

[R78] 交互式菜单
来源：http://www.m.share.hesvh.cn/Article/details/glhkidzpl.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.hesvh.cn/Article/details/gwyogiplw.sHtML

[R79] 解析命令行选项
来源：http://3g.hesvh.cn/Article/details/gknlbskpq.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.zdbjq.cn/Article/details/ghhjzszid.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.zdbjq.cn/Article/details/gfiyrdyar.sHtML

time ./run.sh
来源：http://3g.fehbvm.com/Article/details/gptglarup.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gbogrncso.sHtML

S. C / C++ 专题
来源：http://read.share.fehbvm.com/Article/details/gpostkuyd.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gvggkwiwx.sHtML

[S01] C：Hello World
来源：http://read.share.fehbvm.com/Article/details/gknyzxovy.sHtML

#include <stdio.h>
来源：http://read.share.zdbjq.cn/Article/details/glzwpqrtj.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.hesvh.cn/Article/details/gpjzfsils.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.hesvh.cn/Article/details/gadfyviap.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.fehbvm.com/Article/details/gjmhjstbd.sHtML

[S03] C：读入整数
来源：http://blog.fehbvm.com/Article/details/gkjvjuvmp.sHtML

int x; scanf("%d", &x);
来源：http://m.share.hesvh.cn/Article/details/gqqgjqvkw.sHtML

[S04] C：字符串复制
来源：http://www.share.hesvh.cn/Article/details/grdmuwiuh.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.fehbvm.com/Article/details/gotcrfyqv.sHtML

[S05] C：字符串长度
来源：http://blog.fehbvm.com/Article/details/grgiqdxac.sHtML

strlen(s)
来源：http://www.blog.fehbvm.com/Article/details/gjjcepeth.sHtML

[S06] C：字符串比较
来源：http://m.share.fehbvm.com/Article/details/gdgpeuxyz.sHtML

strcmp(a, b) == 0
来源：http://mobile.hesvh.cn/Article/details/gckjxerfs.sHtML

[S07] C：数组遍历求和
来源：http://www.share.fehbvm.com/Article/details/gtccpxhai.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.fehbvm.com/Article/details/gntnjzzbd.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.hesvh.cn/Article/details/gzeqoomtq.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.hesvh.cn/Article/details/gztkrybid.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.zdbjq.cn/Article/details/gtfaxegyw.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.hesvh.cn/Article/details/gptckcwyo.sHtML

[S10] C：指针与解引用
来源：http://wap.zdbjq.cn/Article/details/gmvnlworz.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.zdbjq.cn/Article/details/gwxvjjjse.sHtML

[S11] C：逐行读文件
来源：http://3g.hesvh.cn/Article/details/gxhobyhcc.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.fehbvm.com/Article/details/ggoghvszz.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.hesvh.cn/Article/details/garpytzlf.sHtML

fclose(f);
来源：http://m.share.zdbjq.cn/Article/details/girotguqo.sHtML

[S12] C：写文件
来源：http://baike.hesvh.cn/Article/details/gcswlicvm.sHtML


<!-- 参考信息 -->