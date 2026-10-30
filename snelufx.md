代发 wailian999

[Q48] CTE 公用表表达式
来源：http://mobile.fanxiaobao.xyz/Article/details/gxfqvyete.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.fanxiaobao.xyz/Article/details/glzriupkx.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://3g.fanxiaobao.xyz/Article/details/gkusqlonj.sHtML

[Q49] 更新单行
来源：http://www.share.fanxiaobao.xyz/Article/details/gnuyfqwxl.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://3g.fanxiaobao.xyz/Article/details/ghfktpimf.sHtML

[Q50] 批量更新
来源：http://baike.fanxiaobao.xyz/Article/details/ggkcbikcn.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.fanxiaobao.xyz/Article/details/gwbfgqyhu.sHtML

[Q51] 用子查询更新
来源：http://blog.fanxiaobao.xyz/Article/details/gzpwtxhed.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/ghlnwrjvd.sHtML

[Q52] 删除指定行
来源：http://m.share.fanxiaobao.xyz/Article/details/gpopjuuff.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.fanxiaobao.xyz/Article/details/gxuagsrje.sHtML

[Q53] 按条件删除
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmtpzotmv.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://3g.fanxiaobao.xyz/Article/details/gjrndvpml.sHtML

[Q54] 清空表
来源：http://read.share.fanxiaobao.xyz/Article/details/guyveygii.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.fanxiaobao.xyz/Article/details/gpbzclbxa.sHtML

[Q55] 排名（并列占位）
来源：http://blog.fanxiaobao.xyz/Article/details/gjqgmtxpt.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.fanxiaobao.xyz/Article/details/glotooghz.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzqqjxtsc.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.fanxiaobao.xyz/Article/details/gknscgkec.sHtML

[Q57] 行号
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmkqhnkqs.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gcqrkrhkd.sHtML

[Q58] 累计求和
来源：http://blog.fanxiaobao.xyz/Article/details/gxccngerb.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/gmuixkhfp.sHtML

[Q59] 分组内累计
来源：http://3g.fanxiaobao.xyz/Article/details/ggtbvdmhv.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.fanxiaobao.xyz/Article/details/ghnyouejs.sHtML

[Q60] 取上一行 / 下一行
来源：http://wap.fanxiaobao.xyz/Article/details/gznahztfj.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://blog.fanxiaobao.xyz/Article/details/gscypmdgi.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.fanxiaobao.xyz/Article/details/gueqpyblw.sHtML

[Q61] 移动平均
来源：http://mobile.fanxiaobao.xyz/Article/details/gxmdggoea.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.fanxiaobao.xyz/Article/details/gdgtifovz.sHtML

[Q62] 分组占比
来源：http://m.share.fanxiaobao.xyz/Article/details/gumaerqaw.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.fanxiaobao.xyz/Article/details/grhncbicg.sHtML

[Q63] 开启事务
来源：http://blog.fanxiaobao.xyz/Article/details/gewfbkbjh.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://mobile.fanxiaobao.xyz/Article/details/galykhnhd.sHtML

[Q64] 提交事务
来源：http://www.share.fanxiaobao.xyz/Article/details/ggrqkqvzh.sHtML

COMMIT;
来源：http://read.share.fanxiaobao.xyz/Article/details/gjxqgfmss.sHtML

[Q65] 回滚事务
来源：http://blog.fanxiaobao.xyz/Article/details/gycxxpdna.sHtML

ROLLBACK;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggoxmxxmv.sHtML

[Q66] 行锁查询
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsiccihkn.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.fanxiaobao.xyz/Article/details/gzcewyhmd.sHtML

[Q67] 设置隔离级别
来源：http://mobile.fanxiaobao.xyz/Article/details/gynvdsytn.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzstynynb.sHtML

[Q68] 保存点
来源：http://www.share.fanxiaobao.xyz/Article/details/guwovelvp.sHtML

SAVEPOINT sp1;
来源：http://baike.fanxiaobao.xyz/Article/details/gbkcbfiid.sHtML

ROLLBACK TO sp1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gbfoybndm.sHtML

[Q69] 查看执行计划
来源：http://baike.fanxiaobao.xyz/Article/details/ggqextquk.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://m.share.fanxiaobao.xyz/Article/details/gwqcvxxuc.sHtML

[Q70] 更新统计信息
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtmultrqk.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqxjdolki.sHtML

[Q71] 查看建表语句
来源：http://3g.fanxiaobao.xyz/Article/details/gunnvfrlp.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wap.fanxiaobao.xyz/Article/details/gyakdorvh.sHtML

[Q72] 查看索引
来源：http://m.share.fanxiaobao.xyz/Article/details/gkvrqzsyi.sHtML

SHOW INDEX FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/galvmhhme.sHtML

[Q73] 查看表状态
来源：http://read.share.fanxiaobao.xyz/Article/details/gkzhbpwul.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://read.share.fanxiaobao.xyz/Article/details/glyepbppb.sHtML

[Q74] 强制使用索引
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfyvabuwy.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.fanxiaobao.xyz/Article/details/ggxjtmrkj.sHtML

[Q75] 日期格式化
来源：http://mobile.fanxiaobao.xyz/Article/details/gzkkipbpw.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.fanxiaobao.xyz/Article/details/gehdvlcxb.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mobile.fanxiaobao.xyz/Article/details/glabssfjb.sHtML

[Q76] 按天统计
来源：http://3g.fanxiaobao.xyz/Article/details/gheyhapzj.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wap.fanxiaobao.xyz/Article/details/gmvfexehl.sHtML

[Q77] 时间加减
来源：http://baike.fanxiaobao.xyz/Article/details/glysdcewd.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.fanxiaobao.xyz/Article/details/gcysevzxl.sHtML

[Q78] 当前时间
来源：http://3g.fanxiaobao.xyz/Article/details/gvxhkbeat.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.fanxiaobao.xyz/Article/details/gfplbcags.sHtML

[Q79] 字符串拼接
来源：http://m.share.fanxiaobao.xyz/Article/details/gesgmfgog.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.fanxiaobao.xyz/Article/details/gonqyrnyz.sHtML

[Q80] 字符串截取
来源：http://mobile.fanxiaobao.xyz/Article/details/gnanmizho.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gbxwqxzji.sHtML

[Q81] 字符串替换
来源：http://blog.fanxiaobao.xyz/Article/details/gfslqfzbk.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gjwpazpoq.sHtML

[Q82] 字符长度与字节长度
来源：http://blog.fanxiaobao.xyz/Article/details/gfunodlxb.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gopcenxty.sHtML

[Q83] 大小写转换
来源：http://wap.fanxiaobao.xyz/Article/details/gtflxuquu.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gjpqeyrlr.sHtML

[Q84] 去除首尾空格
来源：http://www.share.fanxiaobao.xyz/Article/details/gtxjoborv.sHtML

SELECT TRIM(name) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/ggxpckydq.sHtML

[Q85] 数值取整
来源：http://baike.fanxiaobao.xyz/Article/details/gophwlxfm.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdfmpleqb.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.fanxiaobao.xyz/Article/details/grxqedcds.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnrthxrpb.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gczsaaxzd.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glqwypmwt.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.fanxiaobao.xyz/Article/details/geqlwotru.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnlixcdii.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gjelloeay.sHtML

[Q89] 判断表是否存在
来源：http://baike.fanxiaobao.xyz/Article/details/gwkqvavhn.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsigbmwdf.sHtML

[Q90] 生成序号列
来源：http://www.share.fanxiaobao.xyz/Article/details/gpjstziie.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggfhjgdhu.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gcjfdkxxf.sHtML

R. Bash 专题
来源：http://read.share.fanxiaobao.xyz/Article/details/gzxhfpufg.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gopzvmgwv.sHtML

[R01] shebang 与严格模式
来源：http://wap.fanxiaobao.xyz/Article/details/glbrpvbmj.sHtML

#!/usr/bin/env bash
来源：http://blog.fanxiaobao.xyz/Article/details/godjyghvs.sHtML

set -euo pipefail
来源：http://blog.fanxiaobao.xyz/Article/details/gxvbltkag.sHtML

[R02] 变量赋值与使用
来源：http://3g.fanxiaobao.xyz/Article/details/gftzcshbr.sHtML

name="Tom"; echo "$name"
来源：http://read.share.fanxiaobao.xyz/Article/details/gcvnihsfe.sHtML

[R03] 只读变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggrffkpmd.sHtML

readonly PI=3.14
来源：http://read.share.fanxiaobao.xyz/Article/details/gjxnjaezc.sHtML

[R04] 位置参数
来源：http://blog.fanxiaobao.xyz/Article/details/gnsgmajah.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.fanxiaobao.xyz/Article/details/gfyrwxmwl.sHtML

[R05] 参数默认值
来源：http://www.share.fanxiaobao.xyz/Article/details/gmhegimjg.sHtML

name="${1:-default}"
来源：http://3g.fanxiaobao.xyz/Article/details/gdrnbktzd.sHtML

[R06] 判断命令是否存在
来源：http://www.share.fanxiaobao.xyz/Article/details/gjogbniau.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gdfifbcpm.sHtML

[R07] if 判断文件
来源：http://baike.fanxiaobao.xyz/Article/details/gpvgwpvgw.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.fanxiaobao.xyz/Article/details/gbotffdhx.sHtML

[R08] 数值比较
来源：http://blog.fanxiaobao.xyz/Article/details/gwzltalzm.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.fanxiaobao.xyz/Article/details/gvickvwid.sHtML

[R09] 字符串比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkacoakjg.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnpkvzkqy.sHtML

[R10] 正则匹配
来源：http://blog.fanxiaobao.xyz/Article/details/gunobvcnv.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.fanxiaobao.xyz/Article/details/gkzfltcdo.sHtML

[R11] case 多分支
来源：http://m.share.fanxiaobao.xyz/Article/details/gmblmfquw.sHtML

case "$1" in
来源：http://baike.fanxiaobao.xyz/Article/details/guhrpslkd.sHtML

start) echo "启动" ;;
来源：http://blog.fanxiaobao.xyz/Article/details/gxhxyijfc.sHtML

stop)  echo "停止" ;;
来源：http://read.share.fanxiaobao.xyz/Article/details/gcqwquohf.sHtML

*)     echo "未知命令" ;;
来源：http://blog.fanxiaobao.xyz/Article/details/gfibcwdge.sHtML

esac
来源：http://mobile.fanxiaobao.xyz/Article/details/gwjnicjat.sHtML

[R12] for 遍历文件
来源：http://blog.fanxiaobao.xyz/Article/details/gecjmhgof.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gnuxncjpv.sHtML

[R13] for 计数循环
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmztoompb.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geytaryda.sHtML

[R14] C 风格 for
来源：http://www.blog.fanxiaobao.xyz/Article/details/glhacrxyg.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzfegract.sHtML

[R15] while 逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gnkktkegk.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gezuuxogh.sHtML

[R16] until 等待条件
来源：http://mobile.fanxiaobao.xyz/Article/details/gxfkoqcjy.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.fanxiaobao.xyz/Article/details/glnucncnh.sHtML

[R17] 数组定义与取值
来源：http://www.share.fanxiaobao.xyz/Article/details/gqeabsock.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gmurazdst.sHtML

[R18] 遍历数组
来源：http://m.share.fanxiaobao.xyz/Article/details/gybekfrgt.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gpnrwmwhk.sHtML

[R19] 数组长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gagcykqny.sHtML

echo "${#arr[@]}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gdidgujbx.sHtML

[R20] 关联数组（字典）
来源：http://baike.fanxiaobao.xyz/Article/details/gmuvhuuve.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.fanxiaobao.xyz/Article/details/gxsjqqitg.sHtML

[R21] 字符串长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/gddmxenqw.sHtML

echo "${#s}"
来源：http://blog.fanxiaobao.xyz/Article/details/gfqtlrqyo.sHtML

[R22] 截取子串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdyhnwmql.sHtML

echo "${s:0:5}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gnilycqey.sHtML

[R23] 字符串替换
来源：http://baike.fanxiaobao.xyz/Article/details/gsgwesspn.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gwvjehtza.sHtML

[R24] 大小写转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gagslzjsv.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gxkbgnnmj.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqlbdqaxa.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.fanxiaobao.xyz/Article/details/gbbozgsnh.sHtML

[R26] 命令替换
来源：http://3g.fanxiaobao.xyz/Article/details/gxqaqgstp.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.fanxiaobao.xyz/Article/details/gsokeqpzj.sHtML

[R27] 算术展开
来源：http://read.share.fanxiaobao.xyz/Article/details/ggpakydzw.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.fanxiaobao.xyz/Article/details/guzyjoxpi.sHtML

[R28] 浮点运算
来源：http://www.share.fanxiaobao.xyz/Article/details/gmiwwefvj.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gspwnfgnl.sHtML

[R29] 定义函数
来源：http://baike.fanxiaobao.xyz/Article/details/gvqmikvkd.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goouxnryq.sHtML

[R30] 函数返回状态码
来源：http://read.share.fanxiaobao.xyz/Article/details/gucllekdr.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.fanxiaobao.xyz/Article/details/gjjbhmxqs.sHtML

[R31] 局部变量
来源：http://baike.fanxiaobao.xyz/Article/details/guukvpwks.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gxwfrwdsr.sHtML

[R32] 参数个数校验
来源：http://mobile.fanxiaobao.xyz/Article/details/gwntktxfu.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gdmbcffqm.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.fanxiaobao.xyz/Article/details/gewigksxo.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.fanxiaobao.xyz/Article/details/guzlwuptr.sHtML

[R34] 退出时清理
来源：http://baike.fanxiaobao.xyz/Article/details/guqpgyyrz.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.fanxiaobao.xyz/Article/details/gngnwwyme.sHtML

[R35] 后台执行并等待
来源：http://3g.fanxiaobao.xyz/Article/details/gtfpboraq.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.fanxiaobao.xyz/Article/details/gjvuiiobp.sHtML

[R36] 并发执行多个任务
来源：http://m.share.fanxiaobao.xyz/Article/details/gqeexdszc.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.fanxiaobao.xyz/Article/details/giqsrurtn.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggdjustbd.sHtML

files=$(ls -1)
来源：http://blog.fanxiaobao.xyz/Article/details/gborjbfby.sHtML

[R38] 管道串联
来源：http://3g.fanxiaobao.xyz/Article/details/gngbjeeck.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.fanxiaobao.xyz/Article/details/gxzwynseh.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.fanxiaobao.xyz/Article/details/gfnzkxayg.sHtML

cmd > out.log 2>&1
来源：http://www.share.fanxiaobao.xyz/Article/details/gfporsuns.sHtML

[R40] 追加写日志
来源：http://blog.fanxiaobao.xyz/Article/details/ghlrletox.sHtML

echo "log" >> out.log
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwikuoqsb.sHtML

[R41] 丢弃输出
来源：http://baike.fanxiaobao.xyz/Article/details/glnpzazxp.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.fanxiaobao.xyz/Article/details/gaiqipbiq.sHtML

[R42] 输入重定向
来源：http://baike.fanxiaobao.xyz/Article/details/giqqobhaa.sHtML

wc -l < a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gseemxwrc.sHtML

[R43] 按名字查找文件
来源：http://baike.fanxiaobao.xyz/Article/details/gzgkxazbc.sHtML

find . -name "*.log" -type f
来源：http://3g.fanxiaobao.xyz/Article/details/gvgpgfhjs.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grnwmbrdn.sHtML

find . -mtime -7 -type f
来源：http://blog.fanxiaobao.xyz/Article/details/gpibzcnfr.sHtML

[R45] 批量删除
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guxlfqzoj.sHtML

find . -name "*.tmp" -delete
来源：http://3g.fanxiaobao.xyz/Article/details/gamzkvsls.sHtML

[R46] 递归替换文件内容
来源：http://wap.fanxiaobao.xyz/Article/details/gzakrbvni.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.fanxiaobao.xyz/Article/details/ginxfzxyw.sHtML

[R47] sed 单行替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gemnmiaks.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gihakfyau.sHtML

[R48] awk 取指定列
来源：http://wap.fanxiaobao.xyz/Article/details/gpplalefk.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gssnpklko.sHtML

[R49] awk 带条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghmitgczn.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.fanxiaobao.xyz/Article/details/gptkkrhaj.sHtML

[R50] awk 求和
来源：http://baike.fanxiaobao.xyz/Article/details/gmvodmoqo.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gfcsafuyw.sHtML

[R51] 排序去重取前几
来源：http://www.share.fanxiaobao.xyz/Article/details/gkfsutnwx.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.fanxiaobao.xyz/Article/details/gfrnwoiva.sHtML

[R52] 统计行数
来源：http://3g.fanxiaobao.xyz/Article/details/gttozvyfq.sHtML

wc -l a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gcdnvjrbc.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.fanxiaobao.xyz/Article/details/gtacvvsmo.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.fanxiaobao.xyz/Article/details/gablcruzr.sHtML

[R54] 比较两个文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtcqseavu.sHtML

diff a.txt b.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gdkftgqjf.sHtML

[R55] 压缩与解压
来源：http://baike.fanxiaobao.xyz/Article/details/gxmsdufog.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghdhuhpbl.sHtML

[R56] 远程拷贝
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdsbafotp.sHtML

scp file user@host:/path/
来源：http://read.share.fanxiaobao.xyz/Article/details/gxazamtwa.sHtML

[R57] 远程执行命令
来源：http://blog.fanxiaobao.xyz/Article/details/gjjzloafj.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwwluhgkt.sHtML

[R58] 下载文件
来源：http://m.share.fanxiaobao.xyz/Article/details/grbvqpchm.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkqsaglwl.sHtML

[R59] 发 POST JSON
来源：http://wap.fanxiaobao.xyz/Article/details/gsnswnokf.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.fanxiaobao.xyz/Article/details/gdnzbugwt.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghmzmuied.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.fanxiaobao.xyz/Article/details/gsqucvcri.sHtML

[R61] 磁盘占用
来源：http://blog.fanxiaobao.xyz/Article/details/grhdrselc.sHtML

df -h;  du -sh *
来源：http://mobile.fanxiaobao.xyz/Article/details/gircmytke.sHtML

[R62] 找最占空间的文件
来源：http://read.share.fanxiaobao.xyz/Article/details/guiwihbdy.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.fanxiaobao.xyz/Article/details/gunqqmgqr.sHtML

[R63] 内存与进程
来源：http://baike.fanxiaobao.xyz/Article/details/gcnfwaola.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glbsupaey.sHtML

[R64] 结束进程
来源：http://read.share.fanxiaobao.xyz/Article/details/guvhbiyxu.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.fanxiaobao.xyz/Article/details/gfkuwghvo.sHtML

[R65] 查看端口占用
来源：http://www.share.fanxiaobao.xyz/Article/details/gomaawzgz.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.fanxiaobao.xyz/Article/details/gvmywvdro.sHtML

[R66] 定时任务
来源：http://mobile.fanxiaobao.xyz/Article/details/gtshxqqyz.sHtML

crontab -e;  crontab -l
来源：http://blog.fanxiaobao.xyz/Article/details/gkfkiqgkm.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.fanxiaobao.xyz/Article/details/gmcqkrgpw.sHtML

openssl rand -hex 16
来源：http://read.share.fanxiaobao.xyz/Article/details/gxwtoorsg.sHtML

[R68] 计算文件校验值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxbgztipz.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/getbldfuj.sHtML

[R69] 生成随机密码
来源：http://m.share.fanxiaobao.xyz/Article/details/gqpstvgpm.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.fanxiaobao.xyz/Article/details/gyfyrxcmm.sHtML

[R70] 时间戳与互转
来源：http://www.blog.fanxiaobao.xyz/Article/details/gywpessrr.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghgxrxvge.sHtML

[R71] 日期格式化
来源：http://www.share.fanxiaobao.xyz/Article/details/gpsstbonx.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.fanxiaobao.xyz/Article/details/gpokfmakz.sHtML

[R72] 等待端口就绪
来源：http://baike.fanxiaobao.xyz/Article/details/gnjlqpubu.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/grgmnlzsx.sHtML

[R73] 分割大日志
来源：http://blog.fanxiaobao.xyz/Article/details/ghmynncyw.sHtML

split -l 1000 big.log part_
来源：http://blog.fanxiaobao.xyz/Article/details/gpceluzrk.sHtML

[R74] 批量重命名
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdihbvwkm.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gkuikiizn.sHtML

[R75] 导出环境变量
来源：http://blog.fanxiaobao.xyz/Article/details/guccocwmo.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.fanxiaobao.xyz/Article/details/gklolhbym.sHtML

[R76] 使用临时文件
来源：http://3g.fanxiaobao.xyz/Article/details/gpgipirmj.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.fanxiaobao.xyz/Article/details/gqdwieibm.sHtML

[R77] 读取用户输入
来源：http://read.share.fanxiaobao.xyz/Article/details/goamztszr.sHtML

read -rp "请输入: " ans
来源：http://mobile.fanxiaobao.xyz/Article/details/gjnjuvkor.sHtML

[R78] 交互式菜单
来源：http://mobile.fanxiaobao.xyz/Article/details/gqsvesecx.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gipwhkdrk.sHtML

[R79] 解析命令行选项
来源：http://m.share.fanxiaobao.xyz/Article/details/gcspfylvr.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gkyeshviq.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.fanxiaobao.xyz/Article/details/gcreoaund.sHtML

time ./run.sh
来源：http://m.share.fanxiaobao.xyz/Article/details/gydbejacf.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gyoonxkhc.sHtML

S. C / C++ 专题
来源：http://read.share.fanxiaobao.xyz/Article/details/gaxhwjfct.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/grtjyvjxx.sHtML

[S01] C：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gxulwkfyh.sHtML

#include <stdio.h>
来源：http://www.share.fanxiaobao.xyz/Article/details/gwjsqbnvh.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyvnsyqjv.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.fanxiaobao.xyz/Article/details/guwatbbfp.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.fanxiaobao.xyz/Article/details/gjtbnieqb.sHtML

[S03] C：读入整数
来源：http://blog.fanxiaobao.xyz/Article/details/gforgahar.sHtML

int x; scanf("%d", &x);
来源：http://baike.fanxiaobao.xyz/Article/details/gerhgavjk.sHtML

[S04] C：字符串复制
来源：http://3g.fanxiaobao.xyz/Article/details/giyppzkyn.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.fanxiaobao.xyz/Article/details/ghbspdssn.sHtML

[S05] C：字符串长度
来源：http://baike.fanxiaobao.xyz/Article/details/gpdkwktus.sHtML

strlen(s)
来源：http://m.share.fanxiaobao.xyz/Article/details/gitqnbthe.sHtML

[S06] C：字符串比较
来源：http://mobile.fanxiaobao.xyz/Article/details/gvcjbebmx.sHtML

strcmp(a, b) == 0
来源：http://m.share.fanxiaobao.xyz/Article/details/gzexlrrzx.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbogkpacd.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvzcrwfnz.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.fanxiaobao.xyz/Article/details/gkphozziz.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzahqbjhi.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.fanxiaobao.xyz/Article/details/gmtsttakf.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.fanxiaobao.xyz/Article/details/gnwbfefef.sHtML

[S10] C：指针与解引用
来源：http://blog.fanxiaobao.xyz/Article/details/gzeuhwbor.sHtML

int *p = &a;  *p = 5;
来源：http://baike.fanxiaobao.xyz/Article/details/gznrbcjrq.sHtML

[S11] C：逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/gllnqowaa.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.fanxiaobao.xyz/Article/details/gttglajsj.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.fanxiaobao.xyz/Article/details/gaddqekrd.sHtML

fclose(f);
来源：http://wap.fanxiaobao.xyz/Article/details/ggexknfok.sHtML

[S12] C：写文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gnppqhgqo.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gncuorkiw.sHtML

[S13] C：宏定义
来源：http://blog.fanxiaobao.xyz/Article/details/glanrmnkj.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.fanxiaobao.xyz/Article/details/grdwsjwen.sHtML

[S14] C：枚举
来源：http://wap.fanxiaobao.xyz/Article/details/gvzhjfvpk.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.fanxiaobao.xyz/Article/details/gjlvexttn.sHtML

[S15] C：类型转换
来源：http://baike.fanxiaobao.xyz/Article/details/gckbaolza.sHtML

(double) a / b
来源：http://m.share.fanxiaobao.xyz/Article/details/gzrnecrau.sHtML

[S16] C：位操作置位
来源：http://mobile.fanxiaobao.xyz/Article/details/genlctotp.sHtML

x |= (1 << 3);
来源：http://blog.fanxiaobao.xyz/Article/details/gkqwrgcxx.sHtML

[S17] C：安全拼接字符串
来源：http://wap.fanxiaobao.xyz/Article/details/gzyboevau.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.fanxiaobao.xyz/Article/details/gwwrllcmc.sHtML

[S18] C：命令行参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmkrqpmua.sHtML


<!-- 参考信息 -->