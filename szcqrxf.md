代发 wailian999

[Q44] IN 子查询
来源：http://mobile.fanxiaobao.xyz/Article/details/gfoxxxacd.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://m.share.fanxiaobao.xyz/Article/details/gvtnukksu.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.fanxiaobao.xyz/Article/details/gnxgpndvs.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/galqatzbt.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmkvvhdkj.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.fanxiaobao.xyz/Article/details/gpblsaqwq.sHtML

[Q47] 与平均值比较
来源：http://wap.fanxiaobao.xyz/Article/details/gxmigateb.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gadscqrbd.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmtffkwbb.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://baike.fanxiaobao.xyz/Article/details/gynwcszxz.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.fanxiaobao.xyz/Article/details/gshiutnse.sHtML

[Q49] 更新单行
来源：http://baike.fanxiaobao.xyz/Article/details/goauerxgu.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://3g.fanxiaobao.xyz/Article/details/gdutqrpes.sHtML

[Q50] 批量更新
来源：http://www.share.fanxiaobao.xyz/Article/details/gaxzxjopa.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.fanxiaobao.xyz/Article/details/gvruajvfx.sHtML

[Q51] 用子查询更新
来源：http://baike.fanxiaobao.xyz/Article/details/goslgcsff.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/ghygegeha.sHtML

[Q52] 删除指定行
来源：http://blog.fanxiaobao.xyz/Article/details/grxuydjvw.sHtML

DELETE FROM users WHERE id = 10;
来源：http://blog.fanxiaobao.xyz/Article/details/guzxxzofi.sHtML

[Q53] 按条件删除
来源：http://read.share.fanxiaobao.xyz/Article/details/gggblyhwe.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.fanxiaobao.xyz/Article/details/gpxjnqtnb.sHtML

[Q54] 清空表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghxinsuro.sHtML

TRUNCATE TABLE logs;
来源：http://baike.fanxiaobao.xyz/Article/details/gzmmrxyco.sHtML

[Q55] 排名（并列占位）
来源：http://www.share.fanxiaobao.xyz/Article/details/gmzzsmvfo.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.fanxiaobao.xyz/Article/details/gkhttvzjp.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnihnziao.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://baike.fanxiaobao.xyz/Article/details/gvbwxwqse.sHtML

[Q57] 行号
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnteioufv.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/goxgfnkvq.sHtML

[Q58] 累计求和
来源：http://mobile.fanxiaobao.xyz/Article/details/ggawchoie.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvnikasyh.sHtML

[Q59] 分组内累计
来源：http://www.share.fanxiaobao.xyz/Article/details/gzosgzuqx.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/ggxsgooop.sHtML

[Q60] 取上一行 / 下一行
来源：http://baike.fanxiaobao.xyz/Article/details/gzbzxcvjg.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghahjxmoy.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/gjagwcdfl.sHtML

[Q61] 移动平均
来源：http://blog.fanxiaobao.xyz/Article/details/gmxwcvpcr.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wap.fanxiaobao.xyz/Article/details/gynyzpnze.sHtML

[Q62] 分组占比
来源：http://m.share.fanxiaobao.xyz/Article/details/gbynepxxe.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxgbuicce.sHtML

[Q63] 开启事务
来源：http://blog.fanxiaobao.xyz/Article/details/gvdcnnish.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://wap.fanxiaobao.xyz/Article/details/gaejvorhj.sHtML

[Q64] 提交事务
来源：http://mobile.fanxiaobao.xyz/Article/details/gagkccpru.sHtML

COMMIT;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwbfqzivj.sHtML

[Q65] 回滚事务
来源：http://mobile.fanxiaobao.xyz/Article/details/gizhsriee.sHtML

ROLLBACK;
来源：http://wap.fanxiaobao.xyz/Article/details/gudwjirhk.sHtML

[Q66] 行锁查询
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghervddxt.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wap.fanxiaobao.xyz/Article/details/gmcykkzgy.sHtML

[Q67] 设置隔离级别
来源：http://blog.fanxiaobao.xyz/Article/details/gschmvhai.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wap.fanxiaobao.xyz/Article/details/gqdjtkuoi.sHtML

[Q68] 保存点
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gekwylrcf.sHtML

SAVEPOINT sp1;
来源：http://baike.fanxiaobao.xyz/Article/details/gawakchfc.sHtML

ROLLBACK TO sp1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gxbgllwaz.sHtML

[Q69] 查看执行计划
来源：http://read.share.fanxiaobao.xyz/Article/details/gmyyjsrts.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.fanxiaobao.xyz/Article/details/gznniywhw.sHtML

[Q70] 更新统计信息
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjerbhfpc.sHtML

ANALYZE TABLE users;
来源：http://baike.fanxiaobao.xyz/Article/details/gyzflkqcx.sHtML

[Q71] 查看建表语句
来源：http://mobile.fanxiaobao.xyz/Article/details/gzkadqdae.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.fanxiaobao.xyz/Article/details/gtgncuttr.sHtML

[Q72] 查看索引
来源：http://blog.fanxiaobao.xyz/Article/details/gwgnewytt.sHtML

SHOW INDEX FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gjblwnbjc.sHtML

[Q73] 查看表状态
来源：http://baike.fanxiaobao.xyz/Article/details/geeusajau.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://wap.fanxiaobao.xyz/Article/details/gjwbayszl.sHtML

[Q74] 强制使用索引
来源：http://read.share.fanxiaobao.xyz/Article/details/gyqvbcahq.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.fanxiaobao.xyz/Article/details/gurdradkb.sHtML

[Q75] 日期格式化
来源：http://www.share.fanxiaobao.xyz/Article/details/gbjnnyrff.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gljqktggz.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.fanxiaobao.xyz/Article/details/giincrawb.sHtML

[Q76] 按天统计
来源：http://wap.fanxiaobao.xyz/Article/details/gceeofetq.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gengvahes.sHtML

[Q77] 时间加减
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghkvcpdil.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvsivsnqa.sHtML

[Q78] 当前时间
来源：http://wap.fanxiaobao.xyz/Article/details/gvvnsdcxt.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.fanxiaobao.xyz/Article/details/ggiubawky.sHtML

[Q79] 字符串拼接
来源：http://baike.fanxiaobao.xyz/Article/details/gqnppjoth.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.fanxiaobao.xyz/Article/details/gucfzoqgq.sHtML

[Q80] 字符串截取
来源：http://blog.fanxiaobao.xyz/Article/details/gbbtrfpbo.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gfusvpmgc.sHtML

[Q81] 字符串替换
来源：http://mobile.fanxiaobao.xyz/Article/details/ggjdyykfu.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gnentiwca.sHtML

[Q82] 字符长度与字节长度
来源：http://mobile.fanxiaobao.xyz/Article/details/gijsqvmta.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmpcmqgbp.sHtML

[Q83] 大小写转换
来源：http://wap.fanxiaobao.xyz/Article/details/ghfccxnqx.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/giibupbst.sHtML

[Q84] 去除首尾空格
来源：http://3g.fanxiaobao.xyz/Article/details/gwrbcxrpp.sHtML

SELECT TRIM(name) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gnertqvkw.sHtML

[Q85] 数值取整
来源：http://m.share.fanxiaobao.xyz/Article/details/gwglefvri.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gomlxfanv.sHtML

[Q86] 读取 JSON 字段
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gddrnwvjg.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.fanxiaobao.xyz/Article/details/ghncszmqt.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.fanxiaobao.xyz/Article/details/giwbqkyqu.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.fanxiaobao.xyz/Article/details/gpvodidap.sHtML

[Q88] 行转列（条件聚合）
来源：http://m.share.fanxiaobao.xyz/Article/details/giqctdeon.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.fanxiaobao.xyz/Article/details/gxobuqdxi.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gkywhnkfi.sHtML

[Q89] 判断表是否存在
来源：http://3g.fanxiaobao.xyz/Article/details/grlbrqvld.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mobile.fanxiaobao.xyz/Article/details/gdmtpjprj.sHtML

[Q90] 生成序号列
来源：http://blog.fanxiaobao.xyz/Article/details/gnwalgbkg.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.fanxiaobao.xyz/Article/details/giqkdjmma.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gptubujto.sHtML

R. Bash 专题
来源：http://m.share.fanxiaobao.xyz/Article/details/gaunvumwz.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grgagcous.sHtML

[R01] shebang 与严格模式
来源：http://wap.fanxiaobao.xyz/Article/details/gtnzklhtd.sHtML

#!/usr/bin/env bash
来源：http://blog.fanxiaobao.xyz/Article/details/gjmzgkgia.sHtML

set -euo pipefail
来源：http://3g.fanxiaobao.xyz/Article/details/gtijxsaox.sHtML

[R02] 变量赋值与使用
来源：http://baike.fanxiaobao.xyz/Article/details/gjzzqfjfd.sHtML

name="Tom"; echo "$name"
来源：http://blog.fanxiaobao.xyz/Article/details/gjmvnadje.sHtML

[R03] 只读变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfmyrmmzt.sHtML

readonly PI=3.14
来源：http://blog.fanxiaobao.xyz/Article/details/gpyxuhdmm.sHtML

[R04] 位置参数
来源：http://3g.fanxiaobao.xyz/Article/details/gtmibqoiv.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.fanxiaobao.xyz/Article/details/gkhqdfnnt.sHtML

[R05] 参数默认值
来源：http://www.share.fanxiaobao.xyz/Article/details/gmolrzauu.sHtML

name="${1:-default}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggaaszvqi.sHtML

[R06] 判断命令是否存在
来源：http://mobile.fanxiaobao.xyz/Article/details/gkdmfchlf.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.fanxiaobao.xyz/Article/details/guvbvjjge.sHtML

[R07] if 判断文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gtzhatchw.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/gbxvedkdv.sHtML

[R08] 数值比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/guykkltli.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/gckvtmmep.sHtML

[R09] 字符串比较
来源：http://baike.fanxiaobao.xyz/Article/details/greepvxxf.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.fanxiaobao.xyz/Article/details/gkvfgjgxg.sHtML

[R10] 正则匹配
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzoaeyzyi.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.fanxiaobao.xyz/Article/details/gcusqwfow.sHtML

[R11] case 多分支
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghyrttziw.sHtML

case "$1" in
来源：http://www.m.share.fanxiaobao.xyz/Article/details/garbivsgg.sHtML

start) echo "启动" ;;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxqsymaon.sHtML

stop)  echo "停止" ;;
来源：http://3g.fanxiaobao.xyz/Article/details/gzhxymeax.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.fanxiaobao.xyz/Article/details/gacykueyj.sHtML

esac
来源：http://3g.fanxiaobao.xyz/Article/details/gzjfqdzse.sHtML

[R12] for 遍历文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gdjbovbkv.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gbbxnkavn.sHtML

[R13] for 计数循环
来源：http://wap.fanxiaobao.xyz/Article/details/gvnuvbtqb.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gwqbdzkna.sHtML

[R14] C 风格 for
来源：http://wap.fanxiaobao.xyz/Article/details/gskhqtywu.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gnxocilyi.sHtML

[R15] while 逐行读文件
来源：http://wap.fanxiaobao.xyz/Article/details/gztpvixsr.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gmzjisjzk.sHtML

[R16] until 等待条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gacwociqe.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwkuxcfou.sHtML

[R17] 数组定义与取值
来源：http://baike.fanxiaobao.xyz/Article/details/gnvgpjvha.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.fanxiaobao.xyz/Article/details/gyfloxzhk.sHtML

[R18] 遍历数组
来源：http://baike.fanxiaobao.xyz/Article/details/gnleedgji.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gzhdjceac.sHtML

[R19] 数组长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqfkcinxz.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grjxkftwp.sHtML

[R20] 关联数组（字典）
来源：http://mobile.fanxiaobao.xyz/Article/details/gxjinccuw.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.fanxiaobao.xyz/Article/details/gvochyejp.sHtML

[R21] 字符串长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glrqcsxyp.sHtML

echo "${#s}"
来源：http://baike.fanxiaobao.xyz/Article/details/gypbyfmzm.sHtML

[R22] 截取子串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gusjwbekc.sHtML

echo "${s:0:5}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goiizhqov.sHtML

[R23] 字符串替换
来源：http://blog.fanxiaobao.xyz/Article/details/gaemteusf.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gheaxhbkw.sHtML

[R24] 大小写转换
来源：http://wap.fanxiaobao.xyz/Article/details/guhgbssff.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gdjgyhshm.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcihvzmyg.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gyfgryily.sHtML

[R26] 命令替换
来源：http://blog.fanxiaobao.xyz/Article/details/gyqoigflq.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.fanxiaobao.xyz/Article/details/gaqhovqpz.sHtML

[R27] 算术展开
来源：http://read.share.fanxiaobao.xyz/Article/details/ghuyxvjdp.sHtML

echo $((1 + 2 * 3))
来源：http://3g.fanxiaobao.xyz/Article/details/gydoffazl.sHtML

[R28] 浮点运算
来源：http://3g.fanxiaobao.xyz/Article/details/gcqljpzmf.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnkaammyy.sHtML

[R29] 定义函数
来源：http://3g.fanxiaobao.xyz/Article/details/glhzvtfpj.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.fanxiaobao.xyz/Article/details/gkowtppbo.sHtML

[R30] 函数返回状态码
来源：http://wap.fanxiaobao.xyz/Article/details/gipqtsyvo.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.fanxiaobao.xyz/Article/details/gurexjqtl.sHtML

[R31] 局部变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gkghgcuid.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.fanxiaobao.xyz/Article/details/giuzcyees.sHtML

[R32] 参数个数校验
来源：http://blog.fanxiaobao.xyz/Article/details/gmmpxqcpl.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gyshfadmv.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.fanxiaobao.xyz/Article/details/ghajdwkva.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.fanxiaobao.xyz/Article/details/gqvvktnxr.sHtML

[R34] 退出时清理
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqcflokwv.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fanxiaobao.xyz/Article/details/gmefdhuab.sHtML

[R35] 后台执行并等待
来源：http://read.share.fanxiaobao.xyz/Article/details/gynvcrkpx.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxxfdopoz.sHtML

[R36] 并发执行多个任务
来源：http://www.share.fanxiaobao.xyz/Article/details/gyfrswygg.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.fanxiaobao.xyz/Article/details/geeeqjnfq.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghazyydxr.sHtML

files=$(ls -1)
来源：http://wap.fanxiaobao.xyz/Article/details/gycutljrg.sHtML

[R38] 管道串联
来源：http://baike.fanxiaobao.xyz/Article/details/gmuqmqmof.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.fanxiaobao.xyz/Article/details/gzesliuke.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.fanxiaobao.xyz/Article/details/ghjyvjfow.sHtML

cmd > out.log 2>&1
来源：http://blog.fanxiaobao.xyz/Article/details/gjsnzgmez.sHtML

[R40] 追加写日志
来源：http://baike.fanxiaobao.xyz/Article/details/gaqwwsqkx.sHtML

echo "log" >> out.log
来源：http://www.blog.fanxiaobao.xyz/Article/details/guugifdby.sHtML

[R41] 丢弃输出
来源：http://read.share.fanxiaobao.xyz/Article/details/goahgnowq.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.fanxiaobao.xyz/Article/details/grcezfnrs.sHtML

[R42] 输入重定向
来源：http://baike.fanxiaobao.xyz/Article/details/grkkbqgyd.sHtML

wc -l < a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gbtxidprl.sHtML

[R43] 按名字查找文件
来源：http://baike.fanxiaobao.xyz/Article/details/gktuqznfm.sHtML

find . -name "*.log" -type f
来源：http://www.blog.fanxiaobao.xyz/Article/details/gempgntmq.sHtML

[R44] 按修改时间查找
来源：http://www.share.fanxiaobao.xyz/Article/details/gjbqycyjs.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaqvjepff.sHtML

[R45] 批量删除
来源：http://blog.fanxiaobao.xyz/Article/details/gzxqecbel.sHtML

find . -name "*.tmp" -delete
来源：http://3g.fanxiaobao.xyz/Article/details/gaunwzxtu.sHtML

[R46] 递归替换文件内容
来源：http://wap.fanxiaobao.xyz/Article/details/gpfojtjzc.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.fanxiaobao.xyz/Article/details/gorvwlpda.sHtML

[R47] sed 单行替换
来源：http://wap.fanxiaobao.xyz/Article/details/gqmqmatzf.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gewjyxqxe.sHtML

[R48] awk 取指定列
来源：http://wap.fanxiaobao.xyz/Article/details/giwpiwipz.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gmficuzpx.sHtML

[R49] awk 带条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdpiztuea.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.fanxiaobao.xyz/Article/details/gztskeyga.sHtML

[R50] awk 求和
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghikwotix.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gwkraxpnv.sHtML

[R51] 排序去重取前几
来源：http://3g.fanxiaobao.xyz/Article/details/gidtjfcqa.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.fanxiaobao.xyz/Article/details/gisjitgif.sHtML

[R52] 统计行数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcoaklcil.sHtML

wc -l a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gzfpelgnk.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giapdivri.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.fanxiaobao.xyz/Article/details/gtqjhrzaf.sHtML

[R54] 比较两个文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gyuyfnyjz.sHtML

diff a.txt b.txt
来源：http://3g.fanxiaobao.xyz/Article/details/goxaklorn.sHtML

[R55] 压缩与解压
来源：http://mobile.fanxiaobao.xyz/Article/details/gqhkmpeee.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.fanxiaobao.xyz/Article/details/gbudubutu.sHtML

[R56] 远程拷贝
来源：http://www.share.fanxiaobao.xyz/Article/details/gofppcehe.sHtML

scp file user@host:/path/
来源：http://read.share.fanxiaobao.xyz/Article/details/gfjyudrig.sHtML

[R57] 远程执行命令
来源：http://wap.fanxiaobao.xyz/Article/details/gsoutdnnn.sHtML

ssh user@host 'uptime'
来源：http://blog.fanxiaobao.xyz/Article/details/gkxydguye.sHtML

[R58] 下载文件
来源：http://read.share.fanxiaobao.xyz/Article/details/ghogdlxgb.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.fanxiaobao.xyz/Article/details/gjyktgppp.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gibmfrrgu.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.fanxiaobao.xyz/Article/details/gcvgvmfrx.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkzbjpwuj.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.fanxiaobao.xyz/Article/details/gxmisperz.sHtML

[R61] 磁盘占用
来源：http://3g.fanxiaobao.xyz/Article/details/gwspwdopr.sHtML

df -h;  du -sh *
来源：http://3g.fanxiaobao.xyz/Article/details/gdccmktuy.sHtML

[R62] 找最占空间的文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gzmwnqfmz.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.fanxiaobao.xyz/Article/details/geiqbgugb.sHtML

[R63] 内存与进程
来源：http://blog.fanxiaobao.xyz/Article/details/gioubalml.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.fanxiaobao.xyz/Article/details/gcdeugimg.sHtML

[R64] 结束进程
来源：http://www.blog.fanxiaobao.xyz/Article/details/grnrinuro.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.fanxiaobao.xyz/Article/details/grtizrslp.sHtML

[R65] 查看端口占用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpjcwofxq.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.fanxiaobao.xyz/Article/details/gfcpejgaj.sHtML

[R66] 定时任务
来源：http://baike.fanxiaobao.xyz/Article/details/gabjbepgw.sHtML

crontab -e;  crontab -l
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnqiensbu.sHtML

[R67] 生成随机十六进制串
来源：http://blog.fanxiaobao.xyz/Article/details/gwfuoxbvi.sHtML

openssl rand -hex 16
来源：http://wap.fanxiaobao.xyz/Article/details/gslbqmzyc.sHtML

[R68] 计算文件校验值
来源：http://baike.fanxiaobao.xyz/Article/details/gtwfjfirb.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gjtokriir.sHtML

[R69] 生成随机密码
来源：http://blog.fanxiaobao.xyz/Article/details/gpzhstwjf.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.fanxiaobao.xyz/Article/details/gsfgpmgix.sHtML

[R70] 时间戳与互转
来源：http://3g.fanxiaobao.xyz/Article/details/gkqdgwvat.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.fanxiaobao.xyz/Article/details/gpgveagwj.sHtML

[R71] 日期格式化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gumtjnycu.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.fanxiaobao.xyz/Article/details/gaefkiddh.sHtML

[R72] 等待端口就绪
来源：http://mobile.fanxiaobao.xyz/Article/details/gaxtqpsfr.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glhucknpj.sHtML

[R73] 分割大日志
来源：http://mobile.fanxiaobao.xyz/Article/details/gbfvppvdd.sHtML

split -l 1000 big.log part_
来源：http://baike.fanxiaobao.xyz/Article/details/gpjuhbcty.sHtML

[R74] 批量重命名
来源：http://www.share.fanxiaobao.xyz/Article/details/gmttbzxmp.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gubmiitwl.sHtML

[R75] 导出环境变量
来源：http://3g.fanxiaobao.xyz/Article/details/gzgcaxili.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.fanxiaobao.xyz/Article/details/gteuiygin.sHtML

[R76] 使用临时文件
来源：http://baike.fanxiaobao.xyz/Article/details/gvfkxhyjj.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwhagzisf.sHtML

[R77] 读取用户输入
来源：http://baike.fanxiaobao.xyz/Article/details/guulccdse.sHtML

read -rp "请输入: " ans
来源：http://blog.fanxiaobao.xyz/Article/details/gpmefpypg.sHtML

[R78] 交互式菜单
来源：http://m.share.fanxiaobao.xyz/Article/details/gzvxbnphw.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gpzjxuppb.sHtML

[R79] 解析命令行选项
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggpxlxymv.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gakicjryk.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.fanxiaobao.xyz/Article/details/gejxsjoyd.sHtML

time ./run.sh
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxjofkxcu.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gxaztounk.sHtML

S. C / C++ 专题
来源：http://m.share.fanxiaobao.xyz/Article/details/gamvsqhkn.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/ghiinauuz.sHtML

[S01] C：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gsluzlyji.sHtML

#include <stdio.h>
来源：http://m.share.fanxiaobao.xyz/Article/details/gvxnasuox.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gbvpxylhd.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.fanxiaobao.xyz/Article/details/gdcyvnaek.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggzthzpnj.sHtML

[S03] C：读入整数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdsqnqojs.sHtML

int x; scanf("%d", &x);
来源：http://3g.fanxiaobao.xyz/Article/details/griecpflc.sHtML

[S04] C：字符串复制
来源：http://blog.fanxiaobao.xyz/Article/details/gnqysipah.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.fanxiaobao.xyz/Article/details/gcgffchha.sHtML

[S05] C：字符串长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpuiptxsl.sHtML

strlen(s)
来源：http://m.share.fanxiaobao.xyz/Article/details/gnivuxrtp.sHtML

[S06] C：字符串比较
来源：http://read.share.fanxiaobao.xyz/Article/details/guodffqyh.sHtML

strcmp(a, b) == 0
来源：http://mobile.fanxiaobao.xyz/Article/details/goxskvjom.sHtML

[S07] C：数组遍历求和
来源：http://baike.fanxiaobao.xyz/Article/details/gapphocgz.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.fanxiaobao.xyz/Article/details/gnxmvvioh.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.fanxiaobao.xyz/Article/details/gycqqytbb.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.fanxiaobao.xyz/Article/details/guroysmcq.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.fanxiaobao.xyz/Article/details/gendnjlll.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.fanxiaobao.xyz/Article/details/giuwmqnse.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gavxynfce.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.fanxiaobao.xyz/Article/details/gwwpnlsgw.sHtML

[S11] C：逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/guyyrfbir.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvjnrgsdl.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.fanxiaobao.xyz/Article/details/gggdkreki.sHtML

fclose(f);
来源：http://wap.fanxiaobao.xyz/Article/details/gjlrnpcbn.sHtML

[S12] C：写文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gvypxtfzl.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.fanxiaobao.xyz/Article/details/gpzeqqdjg.sHtML

[S13] C：宏定义
来源：http://www.share.fanxiaobao.xyz/Article/details/gkidlgucg.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/garwiqgpf.sHtML

[S14] C：枚举
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqexabenk.sHtML


<!-- 参考信息 -->