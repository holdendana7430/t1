代发 wailian999

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2ccphxvei.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2tyqbiprg.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2egthklft.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2oczrpway.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2vayfrmrn.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2hadoamvm.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2chadpzlc.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2gxekiglb.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2ajpeevax.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2lpbfpoek.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2qwcxtzgq.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2ccxxwzbd.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2houinxtj.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2rhqbnsev.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2caynkghl.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2vtqjwopy.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2qltkukxh.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2kqjzhjzp.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2eobmpcnl.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2xarhepqa.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2leqzurov.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2aoelgtna.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2xxayapqc.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2urybaeuj.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2vuctjtxn.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2mjpjnlap.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2hlxnianz.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2ulolsjdo.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2trmwrltk.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2axifnffv.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2lxcxiyry.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2csberyho.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2gepfqvfy.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2kisjtsst.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2hvvxjgrh.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2idpiixdq.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2njzqxfcm.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2ptdehsjl.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2eqorsdeo.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2mnczihor.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2nppzcjqi.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2nxxwcvpc.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2igsmdjcz.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2eaewlnmd.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2pkmkxejj.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2athvxksq.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2cgeakgsy.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2uzmohwfw.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2kfotopgw.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2uuyjokqq.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2egqzgbsm.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2ivpgecpx.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2bjkxlsfq.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2ohitghwl.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2ixqaixnn.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2jtefdoew.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2hkxrmqya.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2oillriqt.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2ipsqdbgn.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2kbxadylj.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2uxgilwzi.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2jihzapzc.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2hmhrzatm.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2yntvdpam.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2jlopovzb.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2kzejkqov.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2fpqhysmp.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2jctnmmde.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2zjggkkic.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2tubcdufk.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2qxaikglf.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2uivoxrkt.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2ebditjyr.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2brrdrdts.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2nfapjjwi.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2rsyeshtt.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2unafqqpa.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2pxtqprrf.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2qeulrwjj.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2yigdocie.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2nwhvkxtv.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2fsvwkpdu.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2gtmwyjjh.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2twrmxlyt.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2ufvszebl.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2yaolmcye.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2utqoergx.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2ojjgaago.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2rdjoxoyw.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2vbfxyfso.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2tujhshdy.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2rimanzcj.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2zkutenfu.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2lsfwdgjq.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2wslddglp.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2czesypuv.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2kyzghxft.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2rusojoho.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2xzragapf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2glnnfjgf.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2ssrcvbez.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2syqismvc.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2mxpcvkxq.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2esgiltyp.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2yuafribv.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2bghvbvrg.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2rfwyoebs.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2cttmjhqa.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2axiuqoxi.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2mztfbkjp.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2bdwthmzd.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2unwaxqrd.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2pvecexal.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2sqiqkhef.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2dyzgtxez.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2wxhhqtus.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2umsztsuy.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2tyqyvpxu.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2fbtikqwt.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2dwfathzz.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2yrnkxzpb.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2btojmmlu.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2rrzvboya.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2opvhwkwf.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2znsgcmyo.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2pecoegen.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2fhmkoxae.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2efiqswnn.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2pgyjaoxv.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2znmgphsm.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2ddrabeig.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2xtvesers.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2oumohzrg.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2texwtohr.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2mzbmbahe.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2btssmhyt.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2cfvupqsl.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2tbqeojmq.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2dfyxurgc.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2zjftusiu.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2ibvqzzku.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2cnthkixe.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2cikmuouy.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2vinqirfl.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2bdntnfur.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2xbedoaka.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2opdmwxcd.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2cpfjqxby.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2joevwboa.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2vxdzinbu.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2kebpivob.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2dnihawfx.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2tmkieqzj.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2qqawriup.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2xswrjnfx.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2vwvszccd.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2khtntxmi.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2stqufbce.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2etpedieg.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2strmkerv.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2pqbvjsoh.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2xuubvdwz.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2peoxlanw.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2wdlzvozl.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2lgzvmjgv.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2rqqjqkvp.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2zgynmmta.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2wpwxawfx.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2wlvuxqop.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2auubopju.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2eleybnkm.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2kbgvqqkh.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2qgzunvtj.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2zopanldf.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2qgwvhmnp.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2kiyectuo.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2bxmwgeiu.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2yxmzrnsv.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2evwuohok.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2uxsotabc.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2idfwnfew.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2ybocjlfs.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2owrwuafo.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2ffeaykwj.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2nizubrzq.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2uwdepccb.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2sfolpuan.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2tmfhbonr.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2avblojxz.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2pkjxojjw.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2apjenatx.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2rqjqrigb.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2zkfqecoy.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2xugnoacs.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2rcykxtbl.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2njzbudhi.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2theborgl.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2ekyusfcn.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2zvtahqwi.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2blpnsyki.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2aargpzgl.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2jvjftdms.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2dgsjhowr.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2pqoesrxm.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2xjbmumqi.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2shlkxavd.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2becozshe.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2mslgykbw.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2juahxaod.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2mhewceke.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2rpblyvsn.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2enaadrww.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2ezyannwd.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2ciijkext.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2xufgmvdi.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2mgwfzuoz.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2kbpkcuax.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2zhgrnari.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2epktolgv.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2wigmzjjk.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2qnwrzuuu.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2aduucdjb.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2lqnwdrqv.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2xcuzlsfq.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2lfsldfyk.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2xakgutie.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2hbxqqinp.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2pxyydjsy.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2mznkwsif.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2bvtharay.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2naifnlgg.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2cnizygcu.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2ljntszpw.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2bjztfcoj.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2usxsvuzc.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2xhpmnpxt.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2tluyvfyk.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2bfshgrvl.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2jgamscba.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2tekpztqc.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2ylnlvfoo.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2llblfhqb.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2rqnqhtrc.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2davsdtvu.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2xmqlahoo.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2txfobpck.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2rbtwkfza.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2ieamhqjh.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2rnthvwmr.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2bcsjlhyq.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2ovqljgtk.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2bjixjpns.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2ddsumdgy.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2urlkamts.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2iykkjkvf.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2uckjnitt.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2dvkffruq.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2yhubqakv.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2mdrfocau.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2ahlwfoav.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2kvthwtaf.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2sbxvxorc.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2hqpmnfaw.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2nutdcwsj.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2jxaqjkqt.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2clkddhgf.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2gxsnwfdi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qpdetuna.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2vmuueyhv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rrtxsiii.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2abbcqifo.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2lnvvgzun.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2kbccjszp.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2exnuirnq.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2egrushrd.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2jreauehd.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2gbsvlyup.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2ftquawwu.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2yrhmokbq.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2foekeezo.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2yllustqh.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2vfjpzzia.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2nmbxgqxe.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2cnpclbwh.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2xkfwiund.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2mwwebxrt.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2pqipszez.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2bfxfjdzv.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2lryqtvcb.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2apccujhd.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2fssdryyu.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2sqtbqvrn.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2dupwdsla.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2fuzokbfu.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2dszdxwas.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2wkpxjfyc.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2sqgsffag.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2nzactlfd.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2tnahggqs.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2enghwjqr.html


<!-- 参考信息 -->