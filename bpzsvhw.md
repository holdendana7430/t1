代发 wailian999

SELECT u.name, o.amount FROM users u
来源：http://mobile.fanxiaobao.xyz/Article/details/gbcshhbhc.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.fanxiaobao.xyz/Article/details/govanzejg.sHtML

[Q43] 标量子查询
来源：http://read.share.fanxiaobao.xyz/Article/details/gacmcsjlk.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.fanxiaobao.xyz/Article/details/gzlgshraj.sHtML

[Q44] IN 子查询
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gamdwaxnb.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://m.share.fanxiaobao.xyz/Article/details/gycttiwlo.sHtML

[Q45] EXISTS 判断存在
来源：http://wap.fanxiaobao.xyz/Article/details/gtlcrssrg.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.fanxiaobao.xyz/Article/details/gdojyouxz.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.fanxiaobao.xyz/Article/details/ghwxvgzit.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.fanxiaobao.xyz/Article/details/gkuqeiatp.sHtML

[Q47] 与平均值比较
来源：http://baike.fanxiaobao.xyz/Article/details/glijmabqk.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://baike.fanxiaobao.xyz/Article/details/grtbkjgpq.sHtML

[Q48] CTE 公用表表达式
来源：http://m.share.fanxiaobao.xyz/Article/details/guqqcujyt.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.share.fanxiaobao.xyz/Article/details/gkcafulop.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://mobile.fanxiaobao.xyz/Article/details/gdhxfpsna.sHtML

[Q49] 更新单行
来源：http://www.share.fanxiaobao.xyz/Article/details/gnjcwmmrg.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggebwpghy.sHtML

[Q50] 批量更新
来源：http://mobile.fanxiaobao.xyz/Article/details/gaafcxjln.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gapgvopxf.sHtML

[Q51] 用子查询更新
来源：http://wap.fanxiaobao.xyz/Article/details/guezuwire.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://blog.fanxiaobao.xyz/Article/details/gmuewntbf.sHtML

[Q52] 删除指定行
来源：http://mobile.fanxiaobao.xyz/Article/details/gfcexmsjj.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gskpapepx.sHtML

[Q53] 按条件删除
来源：http://mobile.fanxiaobao.xyz/Article/details/goinagttc.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.fanxiaobao.xyz/Article/details/gkpbpcgss.sHtML

[Q54] 清空表
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnisgmmfb.sHtML

TRUNCATE TABLE logs;
来源：http://blog.fanxiaobao.xyz/Article/details/galxydupb.sHtML

[Q55] 排名（并列占位）
来源：http://baike.fanxiaobao.xyz/Article/details/genntayqh.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.fanxiaobao.xyz/Article/details/gxsfpvmqx.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.fanxiaobao.xyz/Article/details/ggxgkmbpv.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsptpkqjv.sHtML

[Q57] 行号
来源：http://www.share.fanxiaobao.xyz/Article/details/gfajkcihd.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gfatkomcu.sHtML

[Q58] 累计求和
来源：http://mobile.fanxiaobao.xyz/Article/details/gkgvpyrtx.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.fanxiaobao.xyz/Article/details/gijgtupxq.sHtML

[Q59] 分组内累计
来源：http://wap.fanxiaobao.xyz/Article/details/gcmlptcfy.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://3g.fanxiaobao.xyz/Article/details/gahdvrtoz.sHtML

[Q60] 取上一行 / 下一行
来源：http://read.share.fanxiaobao.xyz/Article/details/ghztymibj.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.fanxiaobao.xyz/Article/details/gsrlstqyt.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/gxrytasah.sHtML

[Q61] 移动平均
来源：http://www.share.fanxiaobao.xyz/Article/details/gcspivuwh.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://3g.fanxiaobao.xyz/Article/details/gmkkcqckq.sHtML

[Q62] 分组占比
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghiaqkply.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mobile.fanxiaobao.xyz/Article/details/gcocqwzac.sHtML

[Q63] 开启事务
来源：http://m.share.fanxiaobao.xyz/Article/details/gmsvdynuz.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.fanxiaobao.xyz/Article/details/gtuyynirm.sHtML

[Q64] 提交事务
来源：http://mobile.fanxiaobao.xyz/Article/details/gbxgcwyed.sHtML

COMMIT;
来源：http://read.share.fanxiaobao.xyz/Article/details/grugasrgf.sHtML

[Q65] 回滚事务
来源：http://mobile.fanxiaobao.xyz/Article/details/gapgewvlw.sHtML

ROLLBACK;
来源：http://www.blog.fanxiaobao.xyz/Article/details/glnlbchxv.sHtML

[Q66] 行锁查询
来源：http://blog.fanxiaobao.xyz/Article/details/geqafxzhz.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.fanxiaobao.xyz/Article/details/geonwnhho.sHtML

[Q67] 设置隔离级别
来源：http://m.share.fanxiaobao.xyz/Article/details/gilrpmdqm.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wap.fanxiaobao.xyz/Article/details/gvlyzwiik.sHtML

[Q68] 保存点
来源：http://wap.fanxiaobao.xyz/Article/details/gcnsziaqq.sHtML

SAVEPOINT sp1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gmyynnjnc.sHtML

ROLLBACK TO sp1;
来源：http://m.share.fanxiaobao.xyz/Article/details/grykblcpt.sHtML

[Q69] 查看执行计划
来源：http://blog.fanxiaobao.xyz/Article/details/ghidwryxn.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.fanxiaobao.xyz/Article/details/gviifdoog.sHtML

[Q70] 更新统计信息
来源：http://3g.fanxiaobao.xyz/Article/details/gxhecauie.sHtML

ANALYZE TABLE users;
来源：http://3g.fanxiaobao.xyz/Article/details/gqdiafcsz.sHtML

[Q71] 查看建表语句
来源：http://blog.fanxiaobao.xyz/Article/details/glscyrrps.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.fanxiaobao.xyz/Article/details/gqegpxdkk.sHtML

[Q72] 查看索引
来源：http://m.share.fanxiaobao.xyz/Article/details/ghpgmipqi.sHtML

SHOW INDEX FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gezogzgfz.sHtML

[Q73] 查看表状态
来源：http://baike.fanxiaobao.xyz/Article/details/gracdkwav.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://3g.fanxiaobao.xyz/Article/details/giygwykbz.sHtML

[Q74] 强制使用索引
来源：http://baike.fanxiaobao.xyz/Article/details/gpjhzierl.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.fanxiaobao.xyz/Article/details/gfojotrxb.sHtML

[Q75] 日期格式化
来源：http://mobile.fanxiaobao.xyz/Article/details/gdylrqcze.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.fanxiaobao.xyz/Article/details/gvskrhxmt.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyubmofkt.sHtML

[Q76] 按天统计
来源：http://mobile.fanxiaobao.xyz/Article/details/gzexhjvpt.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gymnjjnno.sHtML

[Q77] 时间加减
来源：http://blog.fanxiaobao.xyz/Article/details/gmphiglxq.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://baike.fanxiaobao.xyz/Article/details/gqyhlebcx.sHtML

[Q78] 当前时间
来源：http://m.share.fanxiaobao.xyz/Article/details/gdvoifkft.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.fanxiaobao.xyz/Article/details/gmbcvrkne.sHtML

[Q79] 字符串拼接
来源：http://www.share.fanxiaobao.xyz/Article/details/ggrfxeicj.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvezfqsbp.sHtML

[Q80] 字符串截取
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gffxdaeak.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gnygunkwu.sHtML

[Q81] 字符串替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glklgffbs.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gfhiaorwm.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.fanxiaobao.xyz/Article/details/gnblcruhd.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/guuufwpxr.sHtML

[Q83] 大小写转换
来源：http://www.share.fanxiaobao.xyz/Article/details/gcagrmmrt.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gkspazpmf.sHtML

[Q84] 去除首尾空格
来源：http://wap.fanxiaobao.xyz/Article/details/gqgecbsob.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/ghzcjgelr.sHtML

[Q85] 数值取整
来源：http://baike.fanxiaobao.xyz/Article/details/gshqdxkcl.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.fanxiaobao.xyz/Article/details/gmppzhfcd.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.fanxiaobao.xyz/Article/details/gydqhqbty.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.fanxiaobao.xyz/Article/details/grrvenogb.sHtML

[Q87] JSON 字段做条件
来源：http://wap.fanxiaobao.xyz/Article/details/gzbszqzbr.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://baike.fanxiaobao.xyz/Article/details/gpvulhmtc.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.fanxiaobao.xyz/Article/details/glmxpnzfj.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbtgpmaxb.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/ghipelast.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmynytuab.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.fanxiaobao.xyz/Article/details/gwwvuiiia.sHtML

[Q90] 生成序号列
来源：http://blog.fanxiaobao.xyz/Article/details/gezhclzen.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwietrcps.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gdesusqvm.sHtML

R. Bash 专题
来源：http://wap.fanxiaobao.xyz/Article/details/gzsgecyol.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gulqvoxdw.sHtML

[R01] shebang 与严格模式
来源：http://baike.fanxiaobao.xyz/Article/details/glscrdvzw.sHtML

#!/usr/bin/env bash
来源：http://www.share.fanxiaobao.xyz/Article/details/grjnikzpe.sHtML

set -euo pipefail
来源：http://read.share.fanxiaobao.xyz/Article/details/gawqwzqiu.sHtML

[R02] 变量赋值与使用
来源：http://3g.fanxiaobao.xyz/Article/details/gashbkkjk.sHtML

name="Tom"; echo "$name"
来源：http://3g.fanxiaobao.xyz/Article/details/gmnhziesk.sHtML

[R03] 只读变量
来源：http://blog.fanxiaobao.xyz/Article/details/gnnyhyzjz.sHtML

readonly PI=3.14
来源：http://m.share.fanxiaobao.xyz/Article/details/gwdnkmhgq.sHtML

[R04] 位置参数
来源：http://m.share.fanxiaobao.xyz/Article/details/grdofgqmj.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.fanxiaobao.xyz/Article/details/grthiztsl.sHtML

[R05] 参数默认值
来源：http://mobile.fanxiaobao.xyz/Article/details/gbnnoowgm.sHtML

name="${1:-default}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gojrwtqbh.sHtML

[R06] 判断命令是否存在
来源：http://m.share.fanxiaobao.xyz/Article/details/ghsbwrgbm.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.fanxiaobao.xyz/Article/details/gphsfuysz.sHtML

[R07] if 判断文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnmpyolyn.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://baike.fanxiaobao.xyz/Article/details/glzkkbany.sHtML

[R08] 数值比较
来源：http://baike.fanxiaobao.xyz/Article/details/gnirbxaep.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gblwloawz.sHtML

[R09] 字符串比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gopnlatnx.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/gwtfexeee.sHtML

[R10] 正则匹配
来源：http://3g.fanxiaobao.xyz/Article/details/gyvcawwnv.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/gxllhxuqi.sHtML

[R11] case 多分支
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyczokwaj.sHtML

case "$1" in
来源：http://mobile.fanxiaobao.xyz/Article/details/gmtcmiium.sHtML

start) echo "启动" ;;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkmbzeagb.sHtML

stop)  echo "停止" ;;
来源：http://blog.fanxiaobao.xyz/Article/details/grjixbqum.sHtML

*)     echo "未知命令" ;;
来源：http://wap.fanxiaobao.xyz/Article/details/gobjuorpc.sHtML

esac
来源：http://www.share.fanxiaobao.xyz/Article/details/gbyopcpcm.sHtML

[R12] for 遍历文件
来源：http://wap.fanxiaobao.xyz/Article/details/gbemsgcdo.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gyjogmaby.sHtML

[R13] for 计数循环
来源：http://baike.fanxiaobao.xyz/Article/details/gavwpuvnu.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gyyafpeoa.sHtML

[R14] C 风格 for
来源：http://m.share.fanxiaobao.xyz/Article/details/givpugttv.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gkhzwzwcj.sHtML

[R15] while 逐行读文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gfvrhvsyz.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gchjydvge.sHtML

[R16] until 等待条件
来源：http://www.share.fanxiaobao.xyz/Article/details/gtfnqhgnl.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.fanxiaobao.xyz/Article/details/gboilvlwk.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcuzrsmeh.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.fanxiaobao.xyz/Article/details/gzcdlqttq.sHtML

[R18] 遍历数组
来源：http://www.blog.fanxiaobao.xyz/Article/details/gszkjphyo.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gxqgmltrr.sHtML

[R19] 数组长度
来源：http://www.share.fanxiaobao.xyz/Article/details/gbcrhpudu.sHtML

echo "${#arr[@]}"
来源：http://wap.fanxiaobao.xyz/Article/details/gntzfbwxp.sHtML

[R20] 关联数组（字典）
来源：http://3g.fanxiaobao.xyz/Article/details/gcduhazyf.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gytgsjozd.sHtML

[R21] 字符串长度
来源：http://wap.fanxiaobao.xyz/Article/details/gcixvdqzm.sHtML

echo "${#s}"
来源：http://baike.fanxiaobao.xyz/Article/details/gjudxzdyc.sHtML

[R22] 截取子串
来源：http://read.share.fanxiaobao.xyz/Article/details/gzdfieteb.sHtML

echo "${s:0:5}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkhzjtldm.sHtML

[R23] 字符串替换
来源：http://wap.fanxiaobao.xyz/Article/details/gstfgucxq.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzkakhkit.sHtML

[R24] 大小写转换
来源：http://wap.fanxiaobao.xyz/Article/details/gkgffwuvb.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gbickakar.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.fanxiaobao.xyz/Article/details/gfdmqdkyx.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.fanxiaobao.xyz/Article/details/gpllozwff.sHtML

[R26] 命令替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gxqfnifmj.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.fanxiaobao.xyz/Article/details/gssfkkhms.sHtML

[R27] 算术展开
来源：http://mobile.fanxiaobao.xyz/Article/details/gbwyuwfib.sHtML

echo $((1 + 2 * 3))
来源：http://blog.fanxiaobao.xyz/Article/details/gtsvqlxlz.sHtML

[R28] 浮点运算
来源：http://m.share.fanxiaobao.xyz/Article/details/glfckyjan.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.fanxiaobao.xyz/Article/details/gsxmevbyd.sHtML

[R29] 定义函数
来源：http://m.share.fanxiaobao.xyz/Article/details/guflcpdma.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.fanxiaobao.xyz/Article/details/ggcwewzop.sHtML

[R30] 函数返回状态码
来源：http://m.share.fanxiaobao.xyz/Article/details/guuexojmr.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.fanxiaobao.xyz/Article/details/gymkscqcw.sHtML

[R31] 局部变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glshffslz.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gmmybnkvx.sHtML

[R32] 参数个数校验
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjshmkkvc.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsedtwhme.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.fanxiaobao.xyz/Article/details/gkfmzcaab.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.fanxiaobao.xyz/Article/details/glxcgsmox.sHtML

[R34] 退出时清理
来源：http://3g.fanxiaobao.xyz/Article/details/glthaurut.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fanxiaobao.xyz/Article/details/gipvyprpa.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkplzuvjx.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.fanxiaobao.xyz/Article/details/gdwbjawqu.sHtML

[R36] 并发执行多个任务
来源：http://wap.fanxiaobao.xyz/Article/details/gklwapeva.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghitbotuy.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/guzzdglki.sHtML

files=$(ls -1)
来源：http://blog.fanxiaobao.xyz/Article/details/gbgkoscrb.sHtML

[R38] 管道串联
来源：http://m.share.fanxiaobao.xyz/Article/details/gfppgfmon.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.fanxiaobao.xyz/Article/details/gitwbvhxo.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.fanxiaobao.xyz/Article/details/ghdtoniyg.sHtML

cmd > out.log 2>&1
来源：http://wap.fanxiaobao.xyz/Article/details/gtaktwypk.sHtML

[R40] 追加写日志
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glkbvskes.sHtML

echo "log" >> out.log
来源：http://mobile.fanxiaobao.xyz/Article/details/gxvagdndh.sHtML

[R41] 丢弃输出
来源：http://3g.fanxiaobao.xyz/Article/details/gdsmwxwvv.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.fanxiaobao.xyz/Article/details/ghmbzxniq.sHtML

[R42] 输入重定向
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtxxobzcu.sHtML

wc -l < a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gawibmjga.sHtML

[R43] 按名字查找文件
来源：http://3g.fanxiaobao.xyz/Article/details/gjckjnihy.sHtML

find . -name "*.log" -type f
来源：http://baike.fanxiaobao.xyz/Article/details/grnzuzchm.sHtML

[R44] 按修改时间查找
来源：http://blog.fanxiaobao.xyz/Article/details/gomhfiiys.sHtML

find . -mtime -7 -type f
来源：http://baike.fanxiaobao.xyz/Article/details/gzidqyfxc.sHtML

[R45] 批量删除
来源：http://m.share.fanxiaobao.xyz/Article/details/grdvvmdrx.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsdvkowzr.sHtML

[R46] 递归替换文件内容
来源：http://3g.fanxiaobao.xyz/Article/details/gsibsvilt.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.fanxiaobao.xyz/Article/details/gbhziowxc.sHtML

[R47] sed 单行替换
来源：http://www.share.fanxiaobao.xyz/Article/details/guqrswiwb.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gnxguavyk.sHtML

[R48] awk 取指定列
来源：http://m.share.fanxiaobao.xyz/Article/details/guaihxjru.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gnavirxck.sHtML

[R49] awk 带条件
来源：http://blog.fanxiaobao.xyz/Article/details/gfeeypwzo.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.fanxiaobao.xyz/Article/details/goqsfbwol.sHtML

[R50] awk 求和
来源：http://read.share.fanxiaobao.xyz/Article/details/gxpenwicp.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gqubcccih.sHtML

[R51] 排序去重取前几
来源：http://m.share.fanxiaobao.xyz/Article/details/gnkphpemu.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.fanxiaobao.xyz/Article/details/gnpriqfhl.sHtML

[R52] 统计行数
来源：http://3g.fanxiaobao.xyz/Article/details/gpzbbqrcp.sHtML

wc -l a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gnvqnwitl.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.fanxiaobao.xyz/Article/details/gjhafcevn.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.fanxiaobao.xyz/Article/details/gbnbkuygn.sHtML

[R54] 比较两个文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gkslwzhth.sHtML

diff a.txt b.txt
来源：http://blog.fanxiaobao.xyz/Article/details/giuortxsl.sHtML

[R55] 压缩与解压
来源：http://wap.fanxiaobao.xyz/Article/details/glrbvhntp.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.fanxiaobao.xyz/Article/details/gtrzgvyab.sHtML

[R56] 远程拷贝
来源：http://3g.fanxiaobao.xyz/Article/details/gsvcbqfjt.sHtML

scp file user@host:/path/
来源：http://m.share.fanxiaobao.xyz/Article/details/ghfafimux.sHtML

[R57] 远程执行命令
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfstcnapg.sHtML

ssh user@host 'uptime'
来源：http://www.blog.fanxiaobao.xyz/Article/details/glhsxqjpx.sHtML

[R58] 下载文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtvmzdocz.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.fanxiaobao.xyz/Article/details/gpfvsqvzw.sHtML

[R59] 发 POST JSON
来源：http://wap.fanxiaobao.xyz/Article/details/gfjnaozlw.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.fanxiaobao.xyz/Article/details/ggixhncuf.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.fanxiaobao.xyz/Article/details/gfgjobwbz.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.fanxiaobao.xyz/Article/details/gzfuxucuj.sHtML

[R61] 磁盘占用
来源：http://blog.fanxiaobao.xyz/Article/details/ggwuluuon.sHtML

df -h;  du -sh *
来源：http://m.share.fanxiaobao.xyz/Article/details/gztltcqtq.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gooqwcfcm.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.fanxiaobao.xyz/Article/details/gmzmidavq.sHtML

[R63] 内存与进程
来源：http://3g.fanxiaobao.xyz/Article/details/gogmvifcq.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gccexcjop.sHtML

[R64] 结束进程
来源：http://baike.fanxiaobao.xyz/Article/details/gbnxqyite.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.fanxiaobao.xyz/Article/details/gugiupgkv.sHtML

[R65] 查看端口占用
来源：http://baike.fanxiaobao.xyz/Article/details/gxmludpia.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.fanxiaobao.xyz/Article/details/gzwztccqn.sHtML

[R66] 定时任务
来源：http://mobile.fanxiaobao.xyz/Article/details/gkhsswqiv.sHtML

crontab -e;  crontab -l
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghdldvoao.sHtML

[R67] 生成随机十六进制串
来源：http://wap.fanxiaobao.xyz/Article/details/ganwfmdls.sHtML

openssl rand -hex 16
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqltfgcns.sHtML

[R68] 计算文件校验值
来源：http://3g.fanxiaobao.xyz/Article/details/ganxfywlb.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gohiprquy.sHtML

[R69] 生成随机密码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsubrufch.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.fanxiaobao.xyz/Article/details/gvugcvrwx.sHtML

[R70] 时间戳与互转
来源：http://mobile.fanxiaobao.xyz/Article/details/gbpwhysmo.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.fanxiaobao.xyz/Article/details/gdjbahhad.sHtML

[R71] 日期格式化
来源：http://mobile.fanxiaobao.xyz/Article/details/gdvdrqqvc.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.fanxiaobao.xyz/Article/details/gydcipzel.sHtML

[R72] 等待端口就绪
来源：http://m.share.fanxiaobao.xyz/Article/details/grvxulkqm.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gumfsafzx.sHtML

[R73] 分割大日志
来源：http://m.share.fanxiaobao.xyz/Article/details/gsuymyrnu.sHtML

split -l 1000 big.log part_
来源：http://read.share.fanxiaobao.xyz/Article/details/geitepchs.sHtML

[R74] 批量重命名
来源：http://3g.fanxiaobao.xyz/Article/details/ggvtldpcb.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gfqcgbdym.sHtML

[R75] 导出环境变量
来源：http://blog.fanxiaobao.xyz/Article/details/gtunvwshs.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.fanxiaobao.xyz/Article/details/gvysktaaj.sHtML

[R76] 使用临时文件
来源：http://wap.fanxiaobao.xyz/Article/details/gjtxeoxre.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.fanxiaobao.xyz/Article/details/gxdvqmxdh.sHtML

[R77] 读取用户输入
来源：http://www.blog.fanxiaobao.xyz/Article/details/grgkavxfh.sHtML

read -rp "请输入: " ans
来源：http://www.share.fanxiaobao.xyz/Article/details/gxtfsixqb.sHtML

[R78] 交互式菜单
来源：http://wap.fanxiaobao.xyz/Article/details/gaycpjyqk.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggsvhgrot.sHtML

[R79] 解析命令行选项
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcapllycg.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gknlktbke.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.fanxiaobao.xyz/Article/details/ggdetiris.sHtML

time ./run.sh
来源：http://wap.fanxiaobao.xyz/Article/details/glzzfixnu.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gcfbdvntm.sHtML

S. C / C++ 专题
来源：http://mobile.fanxiaobao.xyz/Article/details/gonbkihzn.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gvzgauqmz.sHtML

[S01] C：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gszqgdysh.sHtML

#include <stdio.h>
来源：http://m.share.fanxiaobao.xyz/Article/details/ggibgentm.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.fanxiaobao.xyz/Article/details/gbedbpbkd.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.fanxiaobao.xyz/Article/details/gszpucccv.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzreeoeas.sHtML

[S03] C：读入整数
来源：http://m.share.fanxiaobao.xyz/Article/details/gqnfpvaax.sHtML

int x; scanf("%d", &x);
来源：http://m.share.fanxiaobao.xyz/Article/details/gjfhwsbef.sHtML

[S04] C：字符串复制
来源：http://read.share.fanxiaobao.xyz/Article/details/gtsqdzzct.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtullqocz.sHtML

[S05] C：字符串长度
来源：http://wap.fanxiaobao.xyz/Article/details/gzyvmfrot.sHtML

strlen(s)
来源：http://3g.fanxiaobao.xyz/Article/details/gvdfyboin.sHtML

[S06] C：字符串比较
来源：http://www.share.fanxiaobao.xyz/Article/details/grrhewrxp.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmrqksmdw.sHtML

[S07] C：数组遍历求和
来源：http://www.share.fanxiaobao.xyz/Article/details/givvctckz.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.fanxiaobao.xyz/Article/details/gbszazpqx.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.fanxiaobao.xyz/Article/details/gvsqfybvz.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcbvrnocj.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.fanxiaobao.xyz/Article/details/giwyxzpzh.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.fanxiaobao.xyz/Article/details/gjasmqewv.sHtML

[S10] C：指针与解引用
来源：http://read.share.fanxiaobao.xyz/Article/details/gylupqhkh.sHtML

int *p = &a;  *p = 5;
来源：http://baike.fanxiaobao.xyz/Article/details/gvasgsipm.sHtML

[S11] C：逐行读文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/guyeoobnm.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.fanxiaobao.xyz/Article/details/guznrqvvk.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.fanxiaobao.xyz/Article/details/gkbthgjik.sHtML

fclose(f);
来源：http://www.share.fanxiaobao.xyz/Article/details/gcwjvcobs.sHtML

[S12] C：写文件
来源：http://3g.fanxiaobao.xyz/Article/details/gvyovelul.sHtML


<!-- 参考信息 -->