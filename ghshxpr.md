代发 wailian999

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.fanxiaobao.xyz/Article/details/gxofpqzwp.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.share.fanxiaobao.xyz/Article/details/gnbwlixhu.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.fanxiaobao.xyz/Article/details/gnwhkaxia.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfztmbwsn.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxdgywlpu.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.fanxiaobao.xyz/Article/details/gphiwudvf.sHtML

[Q43] 标量子查询
来源：http://3g.fanxiaobao.xyz/Article/details/gefdpjueo.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.fanxiaobao.xyz/Article/details/gjfmzhlgm.sHtML

[Q44] IN 子查询
来源：http://baike.fanxiaobao.xyz/Article/details/gxzawrvpv.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmnbbrssy.sHtML

[Q45] EXISTS 判断存在
来源：http://3g.fanxiaobao.xyz/Article/details/gaetpwgut.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.fanxiaobao.xyz/Article/details/gxziufgnv.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gumbfeioz.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guxfbsdiy.sHtML

[Q47] 与平均值比较
来源：http://baike.fanxiaobao.xyz/Article/details/gtwvxuldp.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.fanxiaobao.xyz/Article/details/gmgkftfeq.sHtML

[Q48] CTE 公用表表达式
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfaklxfme.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.fanxiaobao.xyz/Article/details/gyvrhittc.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://3g.fanxiaobao.xyz/Article/details/ghvxlezfw.sHtML

[Q49] 更新单行
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gphqzaugk.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.fanxiaobao.xyz/Article/details/gvculstqu.sHtML

[Q50] 批量更新
来源：http://www.share.fanxiaobao.xyz/Article/details/gdmwxuwyd.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://baike.fanxiaobao.xyz/Article/details/gukhuoqqq.sHtML

[Q51] 用子查询更新
来源：http://wap.fanxiaobao.xyz/Article/details/gcbetvzzw.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwacvyaax.sHtML

[Q52] 删除指定行
来源：http://wap.fanxiaobao.xyz/Article/details/gvhubdcha.sHtML

DELETE FROM users WHERE id = 10;
来源：http://blog.fanxiaobao.xyz/Article/details/gyaajvujo.sHtML

[Q53] 按条件删除
来源：http://mobile.fanxiaobao.xyz/Article/details/gashxobto.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.fanxiaobao.xyz/Article/details/gyswxnssx.sHtML

[Q54] 清空表
来源：http://wap.fanxiaobao.xyz/Article/details/gonpsausq.sHtML

TRUNCATE TABLE logs;
来源：http://blog.fanxiaobao.xyz/Article/details/gbhuohqso.sHtML

[Q55] 排名（并列占位）
来源：http://m.share.fanxiaobao.xyz/Article/details/gwzjhnlgm.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.fanxiaobao.xyz/Article/details/ghbtbvhrw.sHtML

[Q56] 密集排名（并列不占位）
来源：http://blog.fanxiaobao.xyz/Article/details/gnwrlhsnr.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.fanxiaobao.xyz/Article/details/gxioyeqrb.sHtML

[Q57] 行号
来源：http://3g.fanxiaobao.xyz/Article/details/gcnhbmgjz.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzhpchbla.sHtML

[Q58] 累计求和
来源：http://mobile.fanxiaobao.xyz/Article/details/gqzmcxadn.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/gftnsmjqo.sHtML

[Q59] 分组内累计
来源：http://wap.fanxiaobao.xyz/Article/details/gaiixpvcq.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzrnnkotn.sHtML

[Q60] 取上一行 / 下一行
来源：http://m.share.fanxiaobao.xyz/Article/details/gmwyowqvs.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.fanxiaobao.xyz/Article/details/gqtjgjvuf.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/ggtkofgep.sHtML

[Q61] 移动平均
来源：http://blog.fanxiaobao.xyz/Article/details/grcfsnnjy.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/gkltgitvc.sHtML

[Q62] 分组占比
来源：http://blog.fanxiaobao.xyz/Article/details/ghltzexwp.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mobile.fanxiaobao.xyz/Article/details/gybjlaylv.sHtML

[Q63] 开启事务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtgrsmnun.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://3g.fanxiaobao.xyz/Article/details/gwcaxkmta.sHtML

[Q64] 提交事务
来源：http://read.share.fanxiaobao.xyz/Article/details/gjtxlbgql.sHtML

COMMIT;
来源：http://mobile.fanxiaobao.xyz/Article/details/gjgzaizgm.sHtML

[Q65] 回滚事务
来源：http://m.share.fanxiaobao.xyz/Article/details/glvtqryuz.sHtML

ROLLBACK;
来源：http://m.share.fanxiaobao.xyz/Article/details/gxdyiuibw.sHtML

[Q66] 行锁查询
来源：http://mobile.fanxiaobao.xyz/Article/details/gxnglqinm.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://blog.fanxiaobao.xyz/Article/details/gnrbslvhl.sHtML

[Q67] 设置隔离级别
来源：http://m.share.fanxiaobao.xyz/Article/details/gkokqkdyx.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.fanxiaobao.xyz/Article/details/gpawqxusa.sHtML

[Q68] 保存点
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfyzwhxwx.sHtML

SAVEPOINT sp1;
来源：http://m.share.fanxiaobao.xyz/Article/details/grvhcijop.sHtML

ROLLBACK TO sp1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gqiyefkve.sHtML

[Q69] 查看执行计划
来源：http://baike.fanxiaobao.xyz/Article/details/gxnujxslg.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.fanxiaobao.xyz/Article/details/gcvrfhahk.sHtML

[Q70] 更新统计信息
来源：http://3g.fanxiaobao.xyz/Article/details/geraflrqs.sHtML

ANALYZE TABLE users;
来源：http://baike.fanxiaobao.xyz/Article/details/giktneeem.sHtML

[Q71] 查看建表语句
来源：http://3g.fanxiaobao.xyz/Article/details/ginxzmdyg.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.fanxiaobao.xyz/Article/details/gcmbfdtio.sHtML

[Q72] 查看索引
来源：http://www.share.fanxiaobao.xyz/Article/details/gzqxsugxt.sHtML

SHOW INDEX FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gtctfwzvx.sHtML

[Q73] 查看表状态
来源：http://read.share.fanxiaobao.xyz/Article/details/glnjvhljr.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gricwjvuh.sHtML

[Q74] 强制使用索引
来源：http://blog.fanxiaobao.xyz/Article/details/gikijxymj.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.fanxiaobao.xyz/Article/details/gggoqcamt.sHtML

[Q75] 日期格式化
来源：http://read.share.fanxiaobao.xyz/Article/details/ggllqhkmz.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/gvhnrvsbq.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmcnlahpt.sHtML

[Q76] 按天统计
来源：http://read.share.fanxiaobao.xyz/Article/details/ginfxusqd.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.fanxiaobao.xyz/Article/details/gfxkwqvwx.sHtML

[Q77] 时间加减
来源：http://3g.fanxiaobao.xyz/Article/details/gpvouyryy.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.share.fanxiaobao.xyz/Article/details/gqyygwite.sHtML

[Q78] 当前时间
来源：http://3g.fanxiaobao.xyz/Article/details/gwueekueo.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gihawdsyr.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gubwwqlsh.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.fanxiaobao.xyz/Article/details/gdohalbkt.sHtML

[Q80] 字符串截取
来源：http://www.share.fanxiaobao.xyz/Article/details/gdytgpgct.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gqiamswiu.sHtML

[Q81] 字符串替换
来源：http://3g.fanxiaobao.xyz/Article/details/grgebbtam.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/ghawpcrlj.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsypjjixw.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gufdssiqm.sHtML

[Q83] 大小写转换
来源：http://baike.fanxiaobao.xyz/Article/details/gmbjgohyc.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gyptdrxhm.sHtML

[Q84] 去除首尾空格
来源：http://baike.fanxiaobao.xyz/Article/details/gxytmenuo.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gzyvptgyz.sHtML

[Q85] 数值取整
来源：http://baike.fanxiaobao.xyz/Article/details/gygykheag.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.fanxiaobao.xyz/Article/details/gsidbsyls.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.fanxiaobao.xyz/Article/details/gyjatoikz.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.fanxiaobao.xyz/Article/details/giwwlnlxi.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghsqynwel.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.fanxiaobao.xyz/Article/details/gbsttwhqi.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfpebwwnz.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.fanxiaobao.xyz/Article/details/gzxpfkygh.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gafzcuhzo.sHtML

[Q89] 判断表是否存在
来源：http://wap.fanxiaobao.xyz/Article/details/gbdqqjcof.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.fanxiaobao.xyz/Article/details/gzjcwticv.sHtML

[Q90] 生成序号列
来源：http://mobile.fanxiaobao.xyz/Article/details/gpirzzuyr.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.fanxiaobao.xyz/Article/details/gyrrlvfcf.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gnlaszbhf.sHtML

R. Bash 专题
来源：http://blog.fanxiaobao.xyz/Article/details/gwngwuxag.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gljmrtcuz.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmtsfkfmb.sHtML

#!/usr/bin/env bash
来源：http://baike.fanxiaobao.xyz/Article/details/gaabcxbxa.sHtML

set -euo pipefail
来源：http://blog.fanxiaobao.xyz/Article/details/gjjcbjyni.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwdibbqfh.sHtML

name="Tom"; echo "$name"
来源：http://wap.fanxiaobao.xyz/Article/details/gadpzwvdm.sHtML

[R03] 只读变量
来源：http://mobile.fanxiaobao.xyz/Article/details/ghlzrhccx.sHtML

readonly PI=3.14
来源：http://wap.fanxiaobao.xyz/Article/details/gzregmwma.sHtML

[R04] 位置参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdhbvqtoq.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.fanxiaobao.xyz/Article/details/glxrejwrj.sHtML

[R05] 参数默认值
来源：http://wap.fanxiaobao.xyz/Article/details/gcfkznlqf.sHtML

name="${1:-default}"
来源：http://baike.fanxiaobao.xyz/Article/details/gvipyjptj.sHtML

[R06] 判断命令是否存在
来源：http://read.share.fanxiaobao.xyz/Article/details/gvajokalc.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.fanxiaobao.xyz/Article/details/gtjqebxta.sHtML

[R07] if 判断文件
来源：http://wap.fanxiaobao.xyz/Article/details/gvjigemds.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://baike.fanxiaobao.xyz/Article/details/gpfuwxjcv.sHtML

[R08] 数值比较
来源：http://wap.fanxiaobao.xyz/Article/details/gifzphnur.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.fanxiaobao.xyz/Article/details/gbmqcisrw.sHtML

[R09] 字符串比较
来源：http://www.share.fanxiaobao.xyz/Article/details/gqlqobied.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.fanxiaobao.xyz/Article/details/grwixytng.sHtML

[R10] 正则匹配
来源：http://wap.fanxiaobao.xyz/Article/details/ggnlpxsgb.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/gcthkjuex.sHtML

[R11] case 多分支
来源：http://wap.fanxiaobao.xyz/Article/details/gqoyhbvfo.sHtML

case "$1" in
来源：http://blog.fanxiaobao.xyz/Article/details/gspnmwxfw.sHtML

start) echo "启动" ;;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvgmgttvt.sHtML

stop)  echo "停止" ;;
来源：http://m.share.fanxiaobao.xyz/Article/details/goexkkslb.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzbrsndcc.sHtML

esac
来源：http://3g.fanxiaobao.xyz/Article/details/gbitiayah.sHtML

[R12] for 遍历文件
来源：http://www.share.fanxiaobao.xyz/Article/details/guidsdtcx.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaxkcrkeu.sHtML

[R13] for 计数循环
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcdmnfwdl.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gthnjnowm.sHtML

[R14] C 风格 for
来源：http://m.share.fanxiaobao.xyz/Article/details/gremcqojp.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gqklgjzaf.sHtML

[R15] while 逐行读文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gnnkjmxrj.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gsgjzjmgp.sHtML

[R16] until 等待条件
来源：http://wap.fanxiaobao.xyz/Article/details/gjojneuai.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.fanxiaobao.xyz/Article/details/gsqzgvcch.sHtML

[R17] 数组定义与取值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfyjavunx.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.fanxiaobao.xyz/Article/details/ghpqnkmdb.sHtML

[R18] 遍历数组
来源：http://baike.fanxiaobao.xyz/Article/details/gzkzclksu.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqpxpuqjq.sHtML

[R19] 数组长度
来源：http://baike.fanxiaobao.xyz/Article/details/gidpsfupo.sHtML

echo "${#arr[@]}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gwkuwpwtz.sHtML

[R20] 关联数组（字典）
来源：http://blog.fanxiaobao.xyz/Article/details/glyhwyqux.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.fanxiaobao.xyz/Article/details/gkkyyiawf.sHtML

[R21] 字符串长度
来源：http://3g.fanxiaobao.xyz/Article/details/gdkjryvsr.sHtML

echo "${#s}"
来源：http://wap.fanxiaobao.xyz/Article/details/gfjtzupus.sHtML

[R22] 截取子串
来源：http://mobile.fanxiaobao.xyz/Article/details/gytapejca.sHtML

echo "${s:0:5}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gtguarjcd.sHtML

[R23] 字符串替换
来源：http://baike.fanxiaobao.xyz/Article/details/ghwfxsdwg.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.fanxiaobao.xyz/Article/details/gbnakmzsj.sHtML

[R24] 大小写转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gybwirens.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaorderav.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.fanxiaobao.xyz/Article/details/gjqucxpnb.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.fanxiaobao.xyz/Article/details/giktazxap.sHtML

[R26] 命令替换
来源：http://www.share.fanxiaobao.xyz/Article/details/ggyxgyacd.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gngoqiyzs.sHtML

[R27] 算术展开
来源：http://m.share.fanxiaobao.xyz/Article/details/ghgunbkps.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.fanxiaobao.xyz/Article/details/gtroslnaq.sHtML

[R28] 浮点运算
来源：http://baike.fanxiaobao.xyz/Article/details/ghpgfzcxu.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.fanxiaobao.xyz/Article/details/gtnxqrfua.sHtML

[R29] 定义函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gbmlzojum.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gssdxortx.sHtML

[R30] 函数返回状态码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfnmrcxsu.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.fanxiaobao.xyz/Article/details/grgflczye.sHtML

[R31] 局部变量
来源：http://blog.fanxiaobao.xyz/Article/details/gudtxlxjm.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.fanxiaobao.xyz/Article/details/googadiqc.sHtML

[R32] 参数个数校验
来源：http://blog.fanxiaobao.xyz/Article/details/ggdpueigb.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.fanxiaobao.xyz/Article/details/gudxsdojj.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.fanxiaobao.xyz/Article/details/gahqfxqnq.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.fanxiaobao.xyz/Article/details/gkmvrbrum.sHtML

[R34] 退出时清理
来源：http://baike.fanxiaobao.xyz/Article/details/gnqxyfejk.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.fanxiaobao.xyz/Article/details/gbctfldwm.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grhresvmz.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.fanxiaobao.xyz/Article/details/ggzdxxrwv.sHtML

[R36] 并发执行多个任务
来源：http://m.share.fanxiaobao.xyz/Article/details/gkcxpqhxv.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gznfnetou.sHtML

[R37] 把输出赋给变量
来源：http://m.share.fanxiaobao.xyz/Article/details/goixydtpd.sHtML

files=$(ls -1)
来源：http://baike.fanxiaobao.xyz/Article/details/gybewtzhc.sHtML

[R38] 管道串联
来源：http://www.share.fanxiaobao.xyz/Article/details/gubmkslbs.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.fanxiaobao.xyz/Article/details/gxyrtzmbn.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.fanxiaobao.xyz/Article/details/gulrdxlbg.sHtML

cmd > out.log 2>&1
来源：http://baike.fanxiaobao.xyz/Article/details/gguyhzilw.sHtML

[R40] 追加写日志
来源：http://3g.fanxiaobao.xyz/Article/details/gsaqhkgac.sHtML

echo "log" >> out.log
来源：http://read.share.fanxiaobao.xyz/Article/details/geenvgwzu.sHtML

[R41] 丢弃输出
来源：http://m.share.fanxiaobao.xyz/Article/details/gczvbxlsf.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.fanxiaobao.xyz/Article/details/gvyfuzvim.sHtML

[R42] 输入重定向
来源：http://baike.fanxiaobao.xyz/Article/details/gbndkhdro.sHtML

wc -l < a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gsthumdnq.sHtML

[R43] 按名字查找文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/glpptsiaa.sHtML

find . -name "*.log" -type f
来源：http://read.share.fanxiaobao.xyz/Article/details/gbjrqxhts.sHtML

[R44] 按修改时间查找
来源：http://baike.fanxiaobao.xyz/Article/details/gdngdejir.sHtML

find . -mtime -7 -type f
来源：http://m.share.fanxiaobao.xyz/Article/details/gjtvkdykx.sHtML

[R45] 批量删除
来源：http://3g.fanxiaobao.xyz/Article/details/gqvujkrzv.sHtML

find . -name "*.tmp" -delete
来源：http://baike.fanxiaobao.xyz/Article/details/gklyivuzf.sHtML

[R46] 递归替换文件内容
来源：http://read.share.fanxiaobao.xyz/Article/details/glcuwzult.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grvjsgnvu.sHtML

[R47] sed 单行替换
来源：http://baike.fanxiaobao.xyz/Article/details/gzhaufsow.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/guopegpch.sHtML

[R48] awk 取指定列
来源：http://www.share.fanxiaobao.xyz/Article/details/gxxjncwxp.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/ggjpgprjp.sHtML

[R49] awk 带条件
来源：http://m.share.fanxiaobao.xyz/Article/details/gqtejqxpb.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfkpwwneg.sHtML

[R50] awk 求和
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gktrwoitl.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gllmffcsh.sHtML

[R51] 排序去重取前几
来源：http://www.share.fanxiaobao.xyz/Article/details/gdahvucrf.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.fanxiaobao.xyz/Article/details/gxxwrwxjy.sHtML

[R52] 统计行数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpqnzcsoc.sHtML

wc -l a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gzcnnteqv.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.fanxiaobao.xyz/Article/details/gayizoixr.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.fanxiaobao.xyz/Article/details/gdzvrgyxv.sHtML

[R54] 比较两个文件
来源：http://wap.fanxiaobao.xyz/Article/details/gendfckbz.sHtML

diff a.txt b.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gyqjcswnt.sHtML

[R55] 压缩与解压
来源：http://www.blog.fanxiaobao.xyz/Article/details/gofwdrltf.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.fanxiaobao.xyz/Article/details/gmbyqppzl.sHtML

[R56] 远程拷贝
来源：http://baike.fanxiaobao.xyz/Article/details/gmciqnpwe.sHtML

scp file user@host:/path/
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggnkejnvb.sHtML

[R57] 远程执行命令
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmcitxzgv.sHtML

ssh user@host 'uptime'
来源：http://www.share.fanxiaobao.xyz/Article/details/glfkjjaho.sHtML

[R58] 下载文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gofemomfx.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.fanxiaobao.xyz/Article/details/gksbdqmsx.sHtML

[R59] 发 POST JSON
来源：http://www.share.fanxiaobao.xyz/Article/details/gogzvnrdv.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxmsunyon.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.fanxiaobao.xyz/Article/details/ggectzoer.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.fanxiaobao.xyz/Article/details/ganoocffo.sHtML

[R61] 磁盘占用
来源：http://www.share.fanxiaobao.xyz/Article/details/gftidbzvx.sHtML

df -h;  du -sh *
来源：http://www.share.fanxiaobao.xyz/Article/details/gqolstnxh.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvhlxpvam.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.fanxiaobao.xyz/Article/details/guhpqflbl.sHtML

[R63] 内存与进程
来源：http://m.share.fanxiaobao.xyz/Article/details/gvzkisjlr.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvvdclcyg.sHtML

[R64] 结束进程
来源：http://read.share.fanxiaobao.xyz/Article/details/gscodizvz.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.fanxiaobao.xyz/Article/details/gabgpqifm.sHtML

[R65] 查看端口占用
来源：http://read.share.fanxiaobao.xyz/Article/details/gqhokjhqj.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.fanxiaobao.xyz/Article/details/gpwlnguxo.sHtML

[R66] 定时任务
来源：http://mobile.fanxiaobao.xyz/Article/details/gbhdiipie.sHtML

crontab -e;  crontab -l
来源：http://www.share.fanxiaobao.xyz/Article/details/gncpinbav.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.fanxiaobao.xyz/Article/details/gboiklnrm.sHtML

openssl rand -hex 16
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmluefbuv.sHtML

[R68] 计算文件校验值
来源：http://read.share.fanxiaobao.xyz/Article/details/gkpgsnbsq.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpupvcqoa.sHtML

[R69] 生成随机密码
来源：http://mobile.fanxiaobao.xyz/Article/details/gtpnwefno.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.fanxiaobao.xyz/Article/details/gcmxeqwxx.sHtML

[R70] 时间戳与互转
来源：http://read.share.fanxiaobao.xyz/Article/details/gvissnvgm.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkrteemdg.sHtML

[R71] 日期格式化
来源：http://m.share.fanxiaobao.xyz/Article/details/glzreyntd.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.fanxiaobao.xyz/Article/details/ghvfvdfpm.sHtML

[R72] 等待端口就绪
来源：http://read.share.fanxiaobao.xyz/Article/details/gkucrwxyn.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.fanxiaobao.xyz/Article/details/gmnvbjbhm.sHtML

[R73] 分割大日志
来源：http://m.share.fanxiaobao.xyz/Article/details/goeqjjjyg.sHtML

split -l 1000 big.log part_
来源：http://www.share.fanxiaobao.xyz/Article/details/gxgbhisws.sHtML

[R74] 批量重命名
来源：http://www.share.fanxiaobao.xyz/Article/details/ghqyiwhji.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gafjaizma.sHtML

[R75] 导出环境变量
来源：http://wap.fanxiaobao.xyz/Article/details/ghycjmkgg.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gngpcstqu.sHtML

[R76] 使用临时文件
来源：http://3g.fanxiaobao.xyz/Article/details/giklyafrv.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzdptqwpd.sHtML

[R77] 读取用户输入
来源：http://read.share.fanxiaobao.xyz/Article/details/gbufuzyvx.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gypdlskau.sHtML

[R78] 交互式菜单
来源：http://baike.fanxiaobao.xyz/Article/details/garmzyjff.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.fanxiaobao.xyz/Article/details/gitwztnah.sHtML

[R79] 解析命令行选项
来源：http://m.share.fanxiaobao.xyz/Article/details/gnobcxzkl.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.fanxiaobao.xyz/Article/details/gngbcmikn.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.fanxiaobao.xyz/Article/details/gjfwpuzfk.sHtML

time ./run.sh
来源：http://baike.fanxiaobao.xyz/Article/details/ghfleatdg.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gfotbospl.sHtML

S. C / C++ 专题
来源：http://wap.fanxiaobao.xyz/Article/details/gounfyaam.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbqcotkah.sHtML

[S01] C：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gboppsukl.sHtML

#include <stdio.h>
来源：http://www.blog.fanxiaobao.xyz/Article/details/gocpxylwu.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gsndbzjuo.sHtML

[S02] C：变量与格式化输出
来源：http://blog.fanxiaobao.xyz/Article/details/gbbexsatg.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.fanxiaobao.xyz/Article/details/gvimjlgll.sHtML

[S03] C：读入整数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjdqsqibi.sHtML

int x; scanf("%d", &x);
来源：http://baike.fanxiaobao.xyz/Article/details/geocgykhz.sHtML

[S04] C：字符串复制
来源：http://3g.fanxiaobao.xyz/Article/details/grbgglsdc.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.fanxiaobao.xyz/Article/details/gzioqaire.sHtML

[S05] C：字符串长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gzkhcyuot.sHtML

strlen(s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gygvgasel.sHtML

[S06] C：字符串比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gitjvthrp.sHtML

strcmp(a, b) == 0
来源：http://m.share.fanxiaobao.xyz/Article/details/gupdxmvyj.sHtML

[S07] C：数组遍历求和
来源：http://wap.fanxiaobao.xyz/Article/details/gpzfnwiyi.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.fanxiaobao.xyz/Article/details/gfyieiciz.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtjxpxsls.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.fanxiaobao.xyz/Article/details/gvgccrdgz.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.fanxiaobao.xyz/Article/details/gnjgngeqx.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gekxjqgpv.sHtML

[S10] C：指针与解引用
来源：http://m.share.fanxiaobao.xyz/Article/details/gtvfqigur.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.fanxiaobao.xyz/Article/details/guxfsreui.sHtML

[S11] C：逐行读文件
来源：http://wap.fanxiaobao.xyz/Article/details/ghgiioaeu.sHtML


<!-- 参考信息 -->