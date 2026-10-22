代发 wailian999

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2yystpakl.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2qggfeinv.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2emoigkem.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2nzxchyzw.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2ahzqcodn.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2fbgawboo.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2elvxtsxg.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2tptzmxgm.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2egmmlpwz.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2omajiamb.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2olhrhbfl.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2enbwudoi.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2aardoohb.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2tpbybcjd.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2vacfumxa.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2aqnohibb.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2pavqdhbc.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2zdxxhrzr.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2chonipqn.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2ykbvevcs.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2kvdxhkhf.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2dsulnokg.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2mrmsowhs.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2uipdursw.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2kvllmhon.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2qbnwtkts.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2zzshmnmw.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2psegsyxq.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ovwxpure.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2tuwooiqt.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2vgarjnni.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2kujlxmxh.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2pmsjvzws.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2rygqhptz.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2iyfkrzez.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2loamtrvd.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2tdmvhvca.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2tsopyasp.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2jjqmxfdh.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2byeykozx.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2okgyvjcg.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2bhggrsyd.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2ekavtpoo.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2dqqyltku.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2iwgtykfy.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2nvrexipn.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2huqfxqyc.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2uywjvocx.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2gvuksmqg.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2nodtwctq.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2sryszfmh.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2fiyayhgq.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2btvzvqfh.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2bwwpzllg.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2ftttszca.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2jfrzjpgo.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ekbmygnq.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2tdvolbdk.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2bwaiejqp.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2gimzjnqa.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2ofsvxhai.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2qqswqbvr.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2btrbrvpj.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2blykwrju.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2lvfcgepv.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2ehhicpnv.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2virvnqvs.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2lyzjcrtz.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2uulbmctt.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2rpuhfrak.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2tcmkahtc.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2lpwuurdy.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2kqyjbioa.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2awuwtkjh.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2vadvjvzw.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2jheuigzl.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2rceypsvv.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2tbkiomzg.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2kdkyngsr.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2fytndwjb.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2wxeopicb.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2pvgnrzej.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2cvtoapne.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2yndiveuv.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2adktannr.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2vurdznie.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2qvqlnadx.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2lusuyyya.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2jdurwrcy.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2fxwbypkz.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2wcessahp.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2klxmyjzy.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2bzuanmem.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2dyqonyjj.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2syzwvkba.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dgrdegqo.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2udhwtvgz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2srbuqkuv.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2oyaswovf.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2mgcuddeq.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2zpvdytah.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2gwbehblf.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2vzxhmvoc.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2yvtjmark.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2zowvbdpi.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2eoakdfuw.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2krrzqnvg.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2rmyybsxp.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2ldmqglpd.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2wehcihox.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2faxnqpwh.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2zyjwcbcy.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2agtpyiwb.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2rkpvrose.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2xmodzqgp.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2etaqyyar.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2dczwdmux.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2chxrzhqu.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2glblwvoi.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2dvawggwb.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2gyzslmer.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2ovudjytb.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2kqxysmck.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2rhgyawtl.html

esac
来源：http://www.52xcode.cn/Article/details/gt2cthpjnjf.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2wycgbrag.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2ailmiqkf.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2wwwtxwhv.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2tdpguvwe.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2qahtzgog.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2iaasflkv.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2valincyv.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2frifbvue.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2bsobjyzs.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2ybogqnbt.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2nfufvpvm.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2nftadgxo.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2ulzpprsi.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2mjcbfqyn.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2eolyhghy.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2ymzfvwvc.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2uggpkaer.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2qfaozwip.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2muxtixkf.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2igunpzfc.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2pebjmlmi.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2akhsyftm.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2ivgciqov.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2gskrohek.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2iicbilki.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2jqrazvxc.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2igtxutwl.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2hryoizst.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2gsaziasa.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2yjbxiygy.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2tqovgpyk.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2vacfydgk.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2lcgufkoz.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2mtunbxoi.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2usheuwaf.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2lnjwzgxk.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2ujyrmpcq.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2dzlguwcw.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2iybpqbmw.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2vwegbnbe.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2qkcvgdip.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2njzguxmx.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2uowrkelf.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2evxqbbrc.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2kitikuwn.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2cdloradm.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2fshbuntr.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2innancvu.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2gtlgsfcy.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2cwmbfgkm.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2bqdxesmx.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2mhqvzoyn.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2khscytbo.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2wbivqnce.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2xclnngsk.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2gjdnmrrx.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2uahiqlnx.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2xnbjkuyf.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2meygkqje.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2prbguzug.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2pefgsonr.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2dfqpfnsj.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2sxzhqahw.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2foibyoos.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2bqjwrspd.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2bpjcxnmb.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2nlraxdjo.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2neolnpds.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2gsjqktgr.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2kfnawurv.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2ugsmaykb.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2gxpjfegc.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2llcwkffb.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ombiebjw.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2vwjmktrr.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2kktgifgg.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2zbvovcbx.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2rlebbyrq.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2mieykzhw.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2qpvwdatf.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2mrlsxjeq.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2zhxlztnm.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2jzsjaduw.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2quzvgpat.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2ecfbdqsb.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ipinktli.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2rrbihnhc.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2tajzrbgp.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2japzgqxu.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2drqmpxmq.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2oktrkxdh.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2oncyleoc.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2rssdknwb.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2bqihdjyp.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2butqaemv.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2svruhitl.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2ammmtlnt.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2losmgkyo.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2njapyavn.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2hymlvdse.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2ikirpxkk.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2wgailqnc.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2ggzdqilp.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2frfngsmb.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2zrbwxees.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2gugwimix.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2ljlpozqu.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2yeiafqln.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2chkgfbbj.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2jholfrjr.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2iclykmlb.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2lztmsgwa.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2fdjeimvb.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2qiolsydd.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2oceovvuo.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2vqlemsen.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2rwwzkrql.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2dfxqdbjn.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2qjptswar.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2yapqumoy.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2mblxubfd.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2vbeinbxw.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2ofirrcdt.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2acmdnnbr.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2qxqzquwl.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2sizdthkz.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2qienwzqo.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2dtmdqbky.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2abejvptu.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2epblqiiw.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2grcpmkng.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2jedotzxz.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2qlaflpzm.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2yuqgfyka.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2rzzycurn.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2tbizfwqe.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2wmontsqv.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2fgysjafh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gtzlfnvp.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2gzbegfdq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dsyjmxdg.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2iulncgoo.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2rjrxndap.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2ejseyiqk.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2afuovlbq.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2wvnkorgn.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2dymmuktr.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2yhomgqow.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2ehdvlvvo.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2eduhccdc.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2qqirdnty.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2bvpircus.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2wykolpea.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2nrnpcjdl.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2wbfpsypo.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2netaaxkv.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2xihptxod.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2vpbynimd.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2mtvxunfp.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2apjdwrly.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2ioquyzbk.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2kwfobhpo.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2gltwmtye.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2fybeechm.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2rrxpdkmg.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2hskgwmev.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2fdexhbxr.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2hjyarxcn.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2gmqxbmaa.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2hdhujgla.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2vuosrtkq.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2lrjaqbxp.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2kdilmsie.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2ticdyski.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2rxnjbfob.html


<!-- 参考信息 -->