代发 wailian999

SELECT u.name, o.amount FROM users u
来源：http://baike.fanxiaobao.xyz/Article/details/gukvkzzia.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyeednumw.sHtML

[Q43] 标量子查询
来源：http://blog.fanxiaobao.xyz/Article/details/gcqozbypt.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://blog.fanxiaobao.xyz/Article/details/gstngwbnn.sHtML

[Q44] IN 子查询
来源：http://blog.fanxiaobao.xyz/Article/details/giwufadrt.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://m.share.fanxiaobao.xyz/Article/details/gsdptdglg.sHtML

[Q45] EXISTS 判断存在
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcjexdkwq.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.fanxiaobao.xyz/Article/details/glqekjsyz.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://3g.fanxiaobao.xyz/Article/details/gnakfssol.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.fanxiaobao.xyz/Article/details/gvrdesyhp.sHtML

[Q47] 与平均值比较
来源：http://blog.fanxiaobao.xyz/Article/details/gzkktcfbk.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnewgjigl.sHtML

[Q48] CTE 公用表表达式
来源：http://mobile.fanxiaobao.xyz/Article/details/gqexmqusq.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.fanxiaobao.xyz/Article/details/gvhrzbpun.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://3g.fanxiaobao.xyz/Article/details/gurgqhdql.sHtML

[Q49] 更新单行
来源：http://blog.fanxiaobao.xyz/Article/details/gllwyvlhg.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.blog.fanxiaobao.xyz/Article/details/glwoiixno.sHtML

[Q50] 批量更新
来源：http://blog.fanxiaobao.xyz/Article/details/ggzxppjcv.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaawqocaz.sHtML

[Q51] 用子查询更新
来源：http://baike.fanxiaobao.xyz/Article/details/gnytyxtik.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gfqssmwdg.sHtML

[Q52] 删除指定行
来源：http://baike.fanxiaobao.xyz/Article/details/gzrqxkfiv.sHtML

DELETE FROM users WHERE id = 10;
来源：http://baike.fanxiaobao.xyz/Article/details/glrlqafzk.sHtML

[Q53] 按条件删除
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbhqzkgqs.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wap.fanxiaobao.xyz/Article/details/gfjrdjiwi.sHtML

[Q54] 清空表
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjypwnryi.sHtML

TRUNCATE TABLE logs;
来源：http://blog.fanxiaobao.xyz/Article/details/gfealvmye.sHtML

[Q55] 排名（并列占位）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtvigrnip.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://m.share.fanxiaobao.xyz/Article/details/gecwgsjsa.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.fanxiaobao.xyz/Article/details/gvtyvfgah.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqivqrohe.sHtML

[Q57] 行号
来源：http://www.blog.fanxiaobao.xyz/Article/details/grbzpvpvk.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gztddjjlj.sHtML

[Q58] 累计求和
来源：http://3g.fanxiaobao.xyz/Article/details/gyoprzmgi.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.fanxiaobao.xyz/Article/details/gttcwdhid.sHtML

[Q59] 分组内累计
来源：http://3g.fanxiaobao.xyz/Article/details/goqyktsuc.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.fanxiaobao.xyz/Article/details/giwsgootz.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.fanxiaobao.xyz/Article/details/gfbrmbidd.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.fanxiaobao.xyz/Article/details/gzazerbnw.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.fanxiaobao.xyz/Article/details/gpwlkhzln.sHtML

[Q61] 移动平均
来源：http://wap.fanxiaobao.xyz/Article/details/gkkqwjfpn.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.fanxiaobao.xyz/Article/details/gbxpsyxxc.sHtML

[Q62] 分组占比
来源：http://www.share.fanxiaobao.xyz/Article/details/gnncsuhpn.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.fanxiaobao.xyz/Article/details/getdehkyd.sHtML

[Q63] 开启事务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyfanmdrf.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzctjkqfi.sHtML

[Q64] 提交事务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxfiaikyx.sHtML

COMMIT;
来源：http://mobile.fanxiaobao.xyz/Article/details/gkogpycjn.sHtML

[Q65] 回滚事务
来源：http://blog.fanxiaobao.xyz/Article/details/gvhyqmbbd.sHtML

ROLLBACK;
来源：http://blog.fanxiaobao.xyz/Article/details/gomefevhl.sHtML

[Q66] 行锁查询
来源：http://3g.fanxiaobao.xyz/Article/details/gmacrfmjb.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.fanxiaobao.xyz/Article/details/gcqifqggg.sHtML

[Q67] 设置隔离级别
来源：http://www.share.fanxiaobao.xyz/Article/details/gdiqwdzpd.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvdbgljor.sHtML

[Q68] 保存点
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gizibxkvz.sHtML

SAVEPOINT sp1;
来源：http://baike.fanxiaobao.xyz/Article/details/glvwmjdwi.sHtML

ROLLBACK TO sp1;
来源：http://blog.fanxiaobao.xyz/Article/details/gtsofsebf.sHtML

[Q69] 查看执行计划
来源：http://wap.fanxiaobao.xyz/Article/details/ghzxegreu.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.fanxiaobao.xyz/Article/details/gplkgaubm.sHtML

[Q70] 更新统计信息
来源：http://read.share.fanxiaobao.xyz/Article/details/gylzkjlbk.sHtML

ANALYZE TABLE users;
来源：http://blog.fanxiaobao.xyz/Article/details/gantcdfgd.sHtML

[Q71] 查看建表语句
来源：http://blog.fanxiaobao.xyz/Article/details/gvlmgucye.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.fanxiaobao.xyz/Article/details/gthpgabaz.sHtML

[Q72] 查看索引
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqowuihpw.sHtML

SHOW INDEX FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gaiuzpdbk.sHtML

[Q73] 查看表状态
来源：http://blog.fanxiaobao.xyz/Article/details/gdifbzlcg.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.fanxiaobao.xyz/Article/details/gufxyxjqy.sHtML

[Q74] 强制使用索引
来源：http://3g.fanxiaobao.xyz/Article/details/ggzftjnid.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://read.share.fanxiaobao.xyz/Article/details/gsusbscer.sHtML

[Q75] 日期格式化
来源：http://m.share.fanxiaobao.xyz/Article/details/gqonwkfck.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/gseimardf.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mobile.fanxiaobao.xyz/Article/details/gwphenacm.sHtML

[Q76] 按天统计
来源：http://read.share.fanxiaobao.xyz/Article/details/ghbazkgkz.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxczmrykn.sHtML

[Q77] 时间加减
来源：http://mobile.fanxiaobao.xyz/Article/details/ggxdmrour.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.fanxiaobao.xyz/Article/details/gkhhzlvhp.sHtML

[Q78] 当前时间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbekyqlhn.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.fanxiaobao.xyz/Article/details/gwqxxyrhh.sHtML

[Q79] 字符串拼接
来源：http://mobile.fanxiaobao.xyz/Article/details/ghfrcfzax.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.fanxiaobao.xyz/Article/details/gwusbqjhq.sHtML

[Q80] 字符串截取
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtslcipsl.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gihqhskbg.sHtML

[Q81] 字符串替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gkbesrfzg.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/glgmoikvo.sHtML

[Q82] 字符长度与字节长度
来源：http://m.share.fanxiaobao.xyz/Article/details/grncakguu.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gdxptkzxs.sHtML

[Q83] 大小写转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gelduhtaj.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gcrdwjyjg.sHtML

[Q84] 去除首尾空格
来源：http://baike.fanxiaobao.xyz/Article/details/gwkimbkyo.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbixxkmgw.sHtML

[Q85] 数值取整
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcnvgapla.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.fanxiaobao.xyz/Article/details/gdsvpkyra.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.fanxiaobao.xyz/Article/details/goxnkmwtw.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.fanxiaobao.xyz/Article/details/gnfzksbnm.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.fanxiaobao.xyz/Article/details/gciplgztf.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.fanxiaobao.xyz/Article/details/gvfwlbius.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.fanxiaobao.xyz/Article/details/gkpkpnqvh.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.fanxiaobao.xyz/Article/details/ghwwhgrmm.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gpfvgxduf.sHtML

[Q89] 判断表是否存在
来源：http://www.share.fanxiaobao.xyz/Article/details/goofgzmlk.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.fanxiaobao.xyz/Article/details/gnneaanpu.sHtML

[Q90] 生成序号列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gruhlxmhq.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.fanxiaobao.xyz/Article/details/gmguoudlw.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gvfevsmlb.sHtML

R. Bash 专题
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsudfceff.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gijbegtuv.sHtML

[R01] shebang 与严格模式
来源：http://m.share.fanxiaobao.xyz/Article/details/gnebllfpq.sHtML

#!/usr/bin/env bash
来源：http://wap.fanxiaobao.xyz/Article/details/giwqhhgxb.sHtML

set -euo pipefail
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghhsticnd.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gotnauvmy.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsenwplvz.sHtML

[R03] 只读变量
来源：http://baike.fanxiaobao.xyz/Article/details/gtzsxncnn.sHtML

readonly PI=3.14
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcfniktdq.sHtML

[R04] 位置参数
来源：http://mobile.fanxiaobao.xyz/Article/details/gxrwwranb.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.fanxiaobao.xyz/Article/details/gfrbhwloj.sHtML

[R05] 参数默认值
来源：http://read.share.fanxiaobao.xyz/Article/details/ghqhsoixw.sHtML

name="${1:-default}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gtlfpdaew.sHtML

[R06] 判断命令是否存在
来源：http://mobile.fanxiaobao.xyz/Article/details/gahqwbijg.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gnhhykmkw.sHtML

[R07] if 判断文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gbcwyrlgn.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://baike.fanxiaobao.xyz/Article/details/gewjsroqz.sHtML

[R08] 数值比较
来源：http://read.share.fanxiaobao.xyz/Article/details/galtdlyby.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdlpnfugg.sHtML

[R09] 字符串比较
来源：http://baike.fanxiaobao.xyz/Article/details/gmzihcflq.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.fanxiaobao.xyz/Article/details/gdloicbsb.sHtML

[R10] 正则匹配
来源：http://wap.fanxiaobao.xyz/Article/details/giktasndb.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmlksagjl.sHtML

[R11] case 多分支
来源：http://blog.fanxiaobao.xyz/Article/details/gfhpjuubg.sHtML

case "$1" in
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkqmofbqm.sHtML

start) echo "启动" ;;
来源：http://3g.fanxiaobao.xyz/Article/details/ggbdxzhsh.sHtML

stop)  echo "停止" ;;
来源：http://www.share.fanxiaobao.xyz/Article/details/glaexjziq.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.fanxiaobao.xyz/Article/details/gxwbbnixs.sHtML

esac
来源：http://m.share.fanxiaobao.xyz/Article/details/gsbvpfyil.sHtML

[R12] for 遍历文件
来源：http://3g.fanxiaobao.xyz/Article/details/gwjsjzrzs.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gojhcofro.sHtML

[R13] for 计数循环
来源：http://www.share.fanxiaobao.xyz/Article/details/gogumqlwh.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gcfqwjipm.sHtML

[R14] C 风格 for
来源：http://baike.fanxiaobao.xyz/Article/details/gacljbfyg.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gutiidpyc.sHtML

[R15] while 逐行读文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdwvvguoq.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gljadsugf.sHtML

[R16] until 等待条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glchqgnrp.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.fanxiaobao.xyz/Article/details/guohqtywp.sHtML

[R17] 数组定义与取值
来源：http://blog.fanxiaobao.xyz/Article/details/gmqlfroan.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gecjlmneq.sHtML

[R18] 遍历数组
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkzwawvxn.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gfeqrkaxw.sHtML

[R19] 数组长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdtxvvzmz.sHtML

echo "${#arr[@]}"
来源：http://wap.fanxiaobao.xyz/Article/details/gqmacarvq.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbhqwezkx.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gvsqobdaj.sHtML

[R21] 字符串长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjnmxuboh.sHtML

echo "${#s}"
来源：http://mobile.fanxiaobao.xyz/Article/details/geqpcsfqt.sHtML

[R22] 截取子串
来源：http://www.share.fanxiaobao.xyz/Article/details/geyhdkskp.sHtML

echo "${s:0:5}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gekzqzdyk.sHtML

[R23] 字符串替换
来源：http://wap.fanxiaobao.xyz/Article/details/geiwppymp.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giflxkjwx.sHtML

[R24] 大小写转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghnsxfkem.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.fanxiaobao.xyz/Article/details/gbkkormfo.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbxuedygu.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.fanxiaobao.xyz/Article/details/ggdpchidh.sHtML

[R26] 命令替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxapwqibj.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.fanxiaobao.xyz/Article/details/gozkjnujl.sHtML

[R27] 算术展开
来源：http://www.share.fanxiaobao.xyz/Article/details/gpktvqdgb.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.fanxiaobao.xyz/Article/details/gybrulxpb.sHtML

[R28] 浮点运算
来源：http://wap.fanxiaobao.xyz/Article/details/gulihuxqn.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.fanxiaobao.xyz/Article/details/gkclrdcyx.sHtML

[R29] 定义函数
来源：http://blog.fanxiaobao.xyz/Article/details/guzumfchn.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gmykinqvk.sHtML

[R30] 函数返回状态码
来源：http://baike.fanxiaobao.xyz/Article/details/gzfvajmqi.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.fanxiaobao.xyz/Article/details/grvlxasts.sHtML

[R31] 局部变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/giyryhbht.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzxkvjfmo.sHtML

[R32] 参数个数校验
来源：http://baike.fanxiaobao.xyz/Article/details/gqyyvromc.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gbmrakvgv.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdfrsthrb.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.fanxiaobao.xyz/Article/details/gfadnfyht.sHtML

[R34] 退出时清理
来源：http://blog.fanxiaobao.xyz/Article/details/gbhkucedq.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.fanxiaobao.xyz/Article/details/ghfmwqhhz.sHtML

[R35] 后台执行并等待
来源：http://read.share.fanxiaobao.xyz/Article/details/gzbhzdklh.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.fanxiaobao.xyz/Article/details/gtrrfdudw.sHtML

[R36] 并发执行多个任务
来源：http://m.share.fanxiaobao.xyz/Article/details/gjqvrsxbg.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.fanxiaobao.xyz/Article/details/gnnlqiwwb.sHtML

[R37] 把输出赋给变量
来源：http://baike.fanxiaobao.xyz/Article/details/gsdmalhxh.sHtML

files=$(ls -1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gchgoamim.sHtML

[R38] 管道串联
来源：http://3g.fanxiaobao.xyz/Article/details/gioiarhqp.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.fanxiaobao.xyz/Article/details/gmtrzeudw.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.fanxiaobao.xyz/Article/details/gfzoazxvi.sHtML

cmd > out.log 2>&1
来源：http://read.share.fanxiaobao.xyz/Article/details/gjzpeksys.sHtML

[R40] 追加写日志
来源：http://3g.fanxiaobao.xyz/Article/details/gnadbawpi.sHtML

echo "log" >> out.log
来源：http://read.share.fanxiaobao.xyz/Article/details/ggagkdova.sHtML

[R41] 丢弃输出
来源：http://m.share.fanxiaobao.xyz/Article/details/gokuubtwj.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.fanxiaobao.xyz/Article/details/glusnqhjn.sHtML

[R42] 输入重定向
来源：http://www.blog.fanxiaobao.xyz/Article/details/geinggadc.sHtML

wc -l < a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwmqzfxvs.sHtML

[R43] 按名字查找文件
来源：http://baike.fanxiaobao.xyz/Article/details/grugqpczc.sHtML

find . -name "*.log" -type f
来源：http://blog.fanxiaobao.xyz/Article/details/gbwwkecfb.sHtML

[R44] 按修改时间查找
来源：http://read.share.fanxiaobao.xyz/Article/details/gvpzshtqn.sHtML

find . -mtime -7 -type f
来源：http://m.share.fanxiaobao.xyz/Article/details/gldnoeukq.sHtML

[R45] 批量删除
来源：http://3g.fanxiaobao.xyz/Article/details/gflrlbgsf.sHtML

find . -name "*.tmp" -delete
来源：http://3g.fanxiaobao.xyz/Article/details/gkdejqsvg.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.fanxiaobao.xyz/Article/details/goedydxhz.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.fanxiaobao.xyz/Article/details/gndmklybw.sHtML

[R47] sed 单行替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/grsbqqpfu.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyfwfmacg.sHtML

[R48] awk 取指定列
来源：http://read.share.fanxiaobao.xyz/Article/details/gafmbncjf.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/ggkrqdidw.sHtML

[R49] awk 带条件
来源：http://blog.fanxiaobao.xyz/Article/details/gtekrwpby.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfbuvwvhl.sHtML

[R50] awk 求和
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbymwwnew.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gaujdqevd.sHtML

[R51] 排序去重取前几
来源：http://blog.fanxiaobao.xyz/Article/details/grotqgvjv.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.fanxiaobao.xyz/Article/details/gswkdrcae.sHtML

[R52] 统计行数
来源：http://baike.fanxiaobao.xyz/Article/details/gcqouycid.sHtML

wc -l a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gdjyceknw.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjgcmszch.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.fanxiaobao.xyz/Article/details/gaxowxjxn.sHtML

[R54] 比较两个文件
来源：http://blog.fanxiaobao.xyz/Article/details/gkejrxlwu.sHtML

diff a.txt b.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/guygihhfl.sHtML

[R55] 压缩与解压
来源：http://wap.fanxiaobao.xyz/Article/details/gqmqhvaxl.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.fanxiaobao.xyz/Article/details/gfjgbusoh.sHtML

[R56] 远程拷贝
来源：http://baike.fanxiaobao.xyz/Article/details/glyqnwuzs.sHtML

scp file user@host:/path/
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcdlallgn.sHtML

[R57] 远程执行命令
来源：http://3g.fanxiaobao.xyz/Article/details/gvxokaglh.sHtML

ssh user@host 'uptime'
来源：http://m.share.fanxiaobao.xyz/Article/details/gbzxqccbj.sHtML

[R58] 下载文件
来源：http://wap.fanxiaobao.xyz/Article/details/gtimdqyrx.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.fanxiaobao.xyz/Article/details/girzcheyv.sHtML

[R59] 发 POST JSON
来源：http://3g.fanxiaobao.xyz/Article/details/guuonbrtp.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.fanxiaobao.xyz/Article/details/gwmucsgoy.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.fanxiaobao.xyz/Article/details/gnjjkdmxp.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.fanxiaobao.xyz/Article/details/grolqzlay.sHtML

[R61] 磁盘占用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvcibxtac.sHtML

df -h;  du -sh *
来源：http://3g.fanxiaobao.xyz/Article/details/guyisrsul.sHtML

[R62] 找最占空间的文件
来源：http://blog.fanxiaobao.xyz/Article/details/gudrltkro.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.fanxiaobao.xyz/Article/details/gzubgzlme.sHtML

[R63] 内存与进程
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggrjiwdgv.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.fanxiaobao.xyz/Article/details/gtdspvilh.sHtML

[R64] 结束进程
来源：http://mobile.fanxiaobao.xyz/Article/details/gkooncsde.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtwwfmrtb.sHtML

[R65] 查看端口占用
来源：http://baike.fanxiaobao.xyz/Article/details/ggwfzkbjk.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.fanxiaobao.xyz/Article/details/gxfstlbbd.sHtML

[R66] 定时任务
来源：http://baike.fanxiaobao.xyz/Article/details/gsgnperrr.sHtML

crontab -e;  crontab -l
来源：http://mobile.fanxiaobao.xyz/Article/details/gchxygprv.sHtML

[R67] 生成随机十六进制串
来源：http://blog.fanxiaobao.xyz/Article/details/gpqawibkx.sHtML

openssl rand -hex 16
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geibhrxxf.sHtML

[R68] 计算文件校验值
来源：http://m.share.fanxiaobao.xyz/Article/details/gymvtyvua.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gekrzhbbn.sHtML

[R69] 生成随机密码
来源：http://wap.fanxiaobao.xyz/Article/details/ghxlvxudg.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.fanxiaobao.xyz/Article/details/gbxzclesb.sHtML

[R70] 时间戳与互转
来源：http://3g.fanxiaobao.xyz/Article/details/gidcywaly.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpzydrqss.sHtML

[R71] 日期格式化
来源：http://mobile.fanxiaobao.xyz/Article/details/gpujpkier.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwtrdccwt.sHtML

[R72] 等待端口就绪
来源：http://3g.fanxiaobao.xyz/Article/details/godhfezri.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.fanxiaobao.xyz/Article/details/gabjpvadb.sHtML

[R73] 分割大日志
来源：http://www.blog.fanxiaobao.xyz/Article/details/geddvxqui.sHtML

split -l 1000 big.log part_
来源：http://mobile.fanxiaobao.xyz/Article/details/gdegwjzce.sHtML

[R74] 批量重命名
来源：http://blog.fanxiaobao.xyz/Article/details/gkdhpbvhr.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/grheevxzj.sHtML

[R75] 导出环境变量
来源：http://3g.fanxiaobao.xyz/Article/details/goyxpulpq.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.fanxiaobao.xyz/Article/details/gxafvnbfs.sHtML

[R76] 使用临时文件
来源：http://blog.fanxiaobao.xyz/Article/details/gdkelesng.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkxlavpgi.sHtML

[R77] 读取用户输入
来源：http://blog.fanxiaobao.xyz/Article/details/gzaavdraj.sHtML

read -rp "请输入: " ans
来源：http://blog.fanxiaobao.xyz/Article/details/gorjjgknu.sHtML

[R78] 交互式菜单
来源：http://read.share.fanxiaobao.xyz/Article/details/gxiosyhbm.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.fanxiaobao.xyz/Article/details/glysdhxek.sHtML

[R79] 解析命令行选项
来源：http://m.share.fanxiaobao.xyz/Article/details/gmcnppmgy.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.fanxiaobao.xyz/Article/details/gifdhfupq.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.fanxiaobao.xyz/Article/details/gkptxrmkr.sHtML

time ./run.sh
来源：http://read.share.fanxiaobao.xyz/Article/details/gvfghomix.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gffkjgric.sHtML

S. C / C++ 专题
来源：http://read.share.fanxiaobao.xyz/Article/details/ggytmiszi.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grdlqfwrq.sHtML

[S01] C：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjqycosiz.sHtML

#include <stdio.h>
来源：http://m.share.fanxiaobao.xyz/Article/details/geblfgrcb.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.fanxiaobao.xyz/Article/details/gcfupupix.sHtML

[S02] C：变量与格式化输出
来源：http://wap.fanxiaobao.xyz/Article/details/gbqxbtbsz.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.fanxiaobao.xyz/Article/details/ggypskrhr.sHtML

[S03] C：读入整数
来源：http://3g.fanxiaobao.xyz/Article/details/gqwkjrtwh.sHtML

int x; scanf("%d", &x);
来源：http://www.share.fanxiaobao.xyz/Article/details/gkgulfoiy.sHtML

[S04] C：字符串复制
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxwwroals.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.fanxiaobao.xyz/Article/details/giwqowayl.sHtML

[S05] C：字符串长度
来源：http://mobile.fanxiaobao.xyz/Article/details/gufyiciyw.sHtML

strlen(s)
来源：http://3g.fanxiaobao.xyz/Article/details/gikktixyq.sHtML

[S06] C：字符串比较
来源：http://baike.fanxiaobao.xyz/Article/details/gjzaawmzr.sHtML

strcmp(a, b) == 0
来源：http://mobile.fanxiaobao.xyz/Article/details/gebwvzqty.sHtML

[S07] C：数组遍历求和
来源：http://www.share.fanxiaobao.xyz/Article/details/ghgdqfgka.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.fanxiaobao.xyz/Article/details/gatblfkif.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.fanxiaobao.xyz/Article/details/gwfvdwgwd.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.fanxiaobao.xyz/Article/details/gxoxcohwq.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.fanxiaobao.xyz/Article/details/gltkdxyqm.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.fanxiaobao.xyz/Article/details/gbcgvrdyr.sHtML

[S10] C：指针与解引用
来源：http://wap.fanxiaobao.xyz/Article/details/ghdiclehj.sHtML

int *p = &a;  *p = 5;
来源：http://baike.fanxiaobao.xyz/Article/details/ggeaiptku.sHtML

[S11] C：逐行读文件
来源：http://wap.fanxiaobao.xyz/Article/details/gyoezbppn.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.fanxiaobao.xyz/Article/details/gyjbpijja.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.fanxiaobao.xyz/Article/details/gyugefavy.sHtML

fclose(f);
来源：http://m.share.fanxiaobao.xyz/Article/details/gddoxbfyo.sHtML

[S12] C：写文件
来源：http://3g.fanxiaobao.xyz/Article/details/gqrpjwyok.sHtML


<!-- 参考信息 -->