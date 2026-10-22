代发 wailian999

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2rgdhoylj.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2qghwybki.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2mchxojav.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2yuurebhc.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2rpdajxbv.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2ugbjqrjc.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2axkciurw.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2jrmphdhb.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2aupwmqnl.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2uqiwltpz.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2fjiwvkxl.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2ltolbzgk.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2gtvpvqss.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2mgvaxmem.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2jxqoflux.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2hxggosmu.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2hnvvguhz.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2entusiiy.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2holcphkc.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2sgbedjcq.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2sxzmiuya.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2aenuaxre.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2gnqpyhlr.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2nohadurv.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2brpdorkm.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2oedpflvk.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2apufhdcr.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2scbvvnuk.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2vbxwglwi.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2erbbtbeq.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2lscvdfja.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2fvefdloe.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2rrgtyziu.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2aftglpcl.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2mquqqygs.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2fhgaievq.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2fiiatgpf.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2crcjahpo.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2uehzvbyk.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2hrekustb.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2xanpugsl.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2iyheisil.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2sueiukxs.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2nucpedar.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2odifhcku.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2dapxwtkh.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2grhxoxya.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2sqaouvun.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2elnayted.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2ohzvuquc.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2qbqactow.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2jzfsuims.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2hjcxmqro.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2vosyqzlx.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2kjkrryiz.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2zghrwtnx.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2liyemabd.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2npxjgzgg.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2uobzicke.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2dfykeuop.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2ejxabttd.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2thgwryqj.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2hbbesxhu.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2wwxejmpg.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2eowqdcon.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2ktxfucif.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2oucygtff.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2mhdqdpio.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2gtiweijl.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2qaktlkbk.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2hrhrpyhh.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2gcykeduw.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2uwixjgkm.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2brziohxu.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2fbldmrcv.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2wlqltkdl.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2addbousw.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2kghrqisz.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2vbvaoydi.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2zrredhro.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2etgnpstb.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2jbmelfnq.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2spwtlekn.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2hqrsepuq.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2egvevsds.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2dwbtkomd.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2xohkwtem.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2mwontwsb.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2tgfbsogc.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2pcearvhg.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2nusuldcg.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2ekhstyjj.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2jsfiqvuc.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2lrecferw.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2ctgywwro.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cwrtnwsr.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2hfbgbwfx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2layhfqrs.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2oohhhzqi.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2gcxwrmrb.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2zkkinbku.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2xwqjibmc.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2oiamyjlp.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2fzirvrww.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2xmmmuzop.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2mmqwnlil.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2yosbqdsf.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2ojerpcjq.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2obbwfxte.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2fsywmyqz.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2oiejetde.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2cxrehzpm.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2dplfjwkd.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2mkdjujeg.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2notvnnew.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2kykfaebs.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2nvcuyndn.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2akvtoklc.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2jcvhtrql.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2aqgffdgn.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2iwfakwmu.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2hpveaysz.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2vfwmqaev.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2ffgbyphv.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2dckzuvdc.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2irnnxbux.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2odwmpvag.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2jyfvytuq.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2ycuxbnly.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2waixdvud.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2wyltrdcz.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2gzgkerpa.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2oawgmkle.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2tcilzvgm.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2cukgfgdl.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2kcwbtcgz.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2xkjeswby.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2tszzklit.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2rkkkerqi.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2ldivxcct.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2wpllsdnx.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2ipnuvbvj.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2lyozurtq.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2rgyesfjo.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2cduycbln.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2mprbgdgu.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2kqhrgsft.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2xtrtvudk.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2brelcvjh.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2nyndrckh.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2qmuqcwfb.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2pqmpzrgs.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2gnqowtqg.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2nosokirf.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2otuevwkq.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2todaelmx.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2kjbyoovd.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2ysuhtadj.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2nhpjbiex.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2bvodfxjg.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2xzyerfan.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2lbvpkhog.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2mlhhnlqy.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2smwikhai.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2ndgqhkkv.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2jeutsotf.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2rbsogpst.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2kbekddbf.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2eaifvvce.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2xijxpjra.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2bufrsfct.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2avoerdys.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2wmeqblnu.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2wbjbfsxg.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2ykpriokr.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2vpnzwcok.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2xrjpzkbd.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2gfqynjnn.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2anbuiegv.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2ukaujnia.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2gphuwtxv.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2dgpwueme.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2mwlxijib.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2rclqlxvm.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2hrfkeqsb.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2evcetpmn.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2wrpwzzhb.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2gxnpivpw.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2hwzfoczg.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2mibvxrif.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2tfjsgmln.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2whhbzemj.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2tgccikih.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2vuohndjk.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2vjubfzyy.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2mpqawiyt.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2fccsqczh.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2oekvrnpq.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2erhxvhen.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2etkrlvgy.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2gudlowyf.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2rkqcexiw.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2hvzddldc.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2fuetmbit.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2ghyrodyu.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2qiiwfwfp.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2qlfcgqmm.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2htwzeqkj.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2iahucgov.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2hnwduffb.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ukdzalcz.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2sdqjiajz.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2rianzykg.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2rsftpajs.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2kqspwswh.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2yncmpqxm.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2xnrbzkor.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2ahdtnybw.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2nyvvbewp.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2qiwkvjkp.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2shobsbcg.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2jwosrxfa.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2jiwgqxht.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2pcplejeq.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2cgtkdvlc.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2cslvbxoj.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2gkrkilzl.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2hqrsbvst.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2zfhhthus.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2tvqpulqm.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2rirxtiop.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2gztwmxvi.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2yofqdmsr.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2oplixhjj.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2orqoxrby.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2qfxzyqwi.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2snkzqocp.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2iaapwiij.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2wzeeqzai.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2tifknfyj.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2svafikfm.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2vuknludc.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2jjxflbsk.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2lkqohgox.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2pxmyyamr.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2klelneaq.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2tpksibxi.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2imnmhzbz.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2sjszxjij.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2pihhyaad.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2wjjvvzfo.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2mjkahafm.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2daszravq.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2zgzpujtx.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2iypcohho.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2bglsddhn.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2xrutjwvz.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2knhycire.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2olyobhnj.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2tzskeuwb.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2xztuajmi.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2qlmuossh.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2bcxlxpls.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ukdyuifd.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2yewzonbo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ymmpfaji.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ayknklsu.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2enheleto.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2xwvoscje.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2ypvqinti.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2lydlsnze.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2jeoywsbg.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2kcmygnph.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2bopngwsg.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2gbklkzpb.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2hnwndwxj.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2glrnllca.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2drilosja.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2gnjxvfro.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2rxetqkjq.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2sgvxgvnb.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2ztpgqkrj.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2ghefzjoe.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2iucavwso.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2obrxuixg.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2eiutuehq.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2zrmaoafl.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2gcurfgsm.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2ajbclqhx.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2bmxecbfv.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2wepfmrup.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2bmdeglag.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2ldypmzeh.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2jmgodipb.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2bzukwutq.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2komltstb.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2limplcmv.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2icopxhqj.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2exbtmmsp.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2ecoygnkw.html


<!-- 参考信息 -->