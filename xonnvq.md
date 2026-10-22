代发 wailian999

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2zcygthwj.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2ekkcgmys.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2ryxeudbb.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2gqgypvwh.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2nymognsu.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2mycszewy.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2qovauscu.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2ilizzvjo.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2lhaaihhf.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2hbondntw.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2euolvqxu.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2alrzghaw.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2iwopihfn.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2varmdgye.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2jcsbjrlr.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2mjfjrrka.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2itwrhbsn.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2wzjztomp.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2vytgiocf.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2gsolrzrv.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2bokkxmhm.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2jqnlxbxj.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2lnmynlke.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2icpzxaxm.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2qewcjtfr.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2jtokvdri.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2kblgrrgd.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2kujlrizc.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2pfrecdqo.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2einvulmj.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2nytvscdh.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2iuucvkvc.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2llyweoef.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2kpzeomsl.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2hsxullxs.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2qzsqxaeu.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2ifdbglcx.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2eotfiaqi.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2azmelehs.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2wcpkudfr.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2casvdixk.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2jvymjtmr.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2uruwiimj.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2bckjdgiq.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2tajtwhlo.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2xsimwhxk.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2tjelmiad.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2pcowuhhk.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2jbdzwxuu.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2ldgfacic.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2umjpjvoq.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2ehwxipje.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2jyuwhykt.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2xbnmieya.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2begsagmu.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2txibflpk.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2yisktgyu.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2tmcnmvln.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2lykvcqkt.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2oqvpqqwz.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2hmhxhdds.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2tebirgns.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2tubusvgl.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2sjncfnuy.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2ofbreuci.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2unvdwqcw.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2ettfzsro.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2puxlbxpq.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2lpkqkjrc.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2valuarbq.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2qmvpnmgq.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2audbtxvv.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2znrtqpww.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2zvrywzyt.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2mxgosjoz.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ldpxoswm.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2wjnxheij.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2rcrfwcch.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2tfnfalak.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2qgmcuior.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2qlobvqdq.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2kkviublv.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2dnbjcbsw.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2ljfqppqb.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2vgnysfsk.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2inntzepq.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2huzoxqfg.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2ucjnqznv.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2zhyoiiks.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2mwjlqxdh.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2euaamvly.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nfrbqxbl.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2fqggidac.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2skfzagaw.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2ngvslzur.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2ulhsllne.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2szlavugm.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2bprchbsb.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2hllyswdb.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2xnmhpexv.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2astntfyf.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2wpaxntrz.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2aaqkxsrm.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2dwefnupr.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2wntnftrw.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2hiaivlfp.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2yjhfszts.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2jgxrbxqx.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2vhjxcjbf.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2lmsbvtru.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2pezepynf.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2mvfizmnp.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2vvukcfxu.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2gxcsfmdj.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2iizunsdl.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2sqvgnwky.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2ygspwelz.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2vuaowdef.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2cjigfefp.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2feioyqjc.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2uszlxjrp.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2bjjjswob.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2duhjcfxb.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2xgxmefjy.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2mwkwwojw.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2yswrdirt.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2pnrvegcx.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2lxxeuuom.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ywommsfb.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2ezbgkdbq.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2xmbnyhhw.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2aohkchyd.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2xucyiuyo.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2cqwefgbm.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2imdhezkv.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2jnlmwirs.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2nkcqsktp.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2eucsxfaa.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2akwbgbyt.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2ohycuhkh.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2mdaitava.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2ztfpqxik.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2pulnqktw.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2irmxuwrf.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2iuooxncq.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2lnimudxp.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2olgrjodg.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2diuucmeh.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2zoocikpu.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2ysqyexlv.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2cciqkich.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2wnaopfwo.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2pizdetrk.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2hzvyqmrq.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2ekfkhgya.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2zbevkyjb.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2wyqzpiax.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2dxquafmn.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2palabpie.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2tzuxlnxt.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2kgiocpeb.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2bvstyvdt.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2ljqqcajc.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2oepgqkyw.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2pwtswuob.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2zmqzpmym.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2fovgpzch.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2rqthllbz.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2yqkmonqz.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2iaicvabf.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2hajsbnyd.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2mwixsvhp.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2gzyeosjh.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2udjdmujx.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2zepyqxod.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2ckfcyghl.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2guweamag.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2mqkevfhy.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2prkldkub.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2dmrhttvy.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2hcblaiko.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2dtrconjg.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2whiqnzox.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2rxjetjge.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2mguvsogv.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2plucrpxx.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2chwxxzjy.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2nghphpmn.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2bknbzicq.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2mcedsfha.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2iknseqbq.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2kadwibyb.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2vjcaldup.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2ycnrgfoh.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2hahhjtai.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2nbuirjff.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2hmwdcxfa.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2fyvzxgqu.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2paqhqspb.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2sjckmejk.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2ohjyglxf.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2ngvqmaqi.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2ezcieodw.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2vlyqehfa.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2atqcnehg.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2nlnubveh.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2pvltmopp.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2iovabvus.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2shoanphy.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2snsowsgn.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2tnckweal.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2oevfazkh.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2yxttxkgu.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2httlhonz.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2vvlhgibo.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2evnadqxz.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2hultlrtz.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2gkpvzskl.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2jmekzari.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2nmzafnsg.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2zoqhjbxb.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2cpiygddz.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2cqaldvjh.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2ikymkwfh.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2govofxip.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2rqpmwppz.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2hmyqnlkg.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2proxixir.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2ccggqrfz.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2aryzarxo.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2tvuhgfic.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2vbuyvkmr.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2iwqvktpg.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2yaegxxhi.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2pzxzltze.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2ilutftdn.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2ntiqblhc.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2xiexpytd.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2vcohsrut.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2yjzwgerg.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2wpngnapd.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2pwrhpwwp.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2cfhdkhft.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2xjhilmzj.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2zcqkjwrs.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2lwyvyylm.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2ajiwldpk.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2lqavqjaf.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2qahtyxbp.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2pdrpxqet.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2swnocbdo.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2xsczjwim.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2kxjikgnv.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2ukgalqag.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2pdmpwnsn.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2aaexuxtj.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2cvrawdrv.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2ipqgafbq.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2ruaurbns.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2opdwucnt.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2sjyyhomo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2muoooqbs.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2qfyxnlay.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2klssiaiu.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2kjcylohp.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2zkvemmag.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2aubyvbrr.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2mhiaolxy.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2gpqavjzq.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2yjxyihbg.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2jvqdnzqr.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2oiacqhfv.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2qdgbcsoe.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2nvthxaqa.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2jbjhrypw.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2qvieedsv.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2osubxage.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2kbrgnrbz.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2uzqbefij.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2sbwpkbjb.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2hnxbawfh.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2jjkkmmqi.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2jrrpdohv.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2abnxpdlt.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2krpopeft.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2vicqjaeh.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2gyzekotu.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2hsyauqwk.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2ooagaggg.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2vpiwvrrf.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2tmbezalk.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2asdueiof.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2rufaoqwv.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2zqgminae.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2ervqptlo.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2jnxjomfw.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2pwumffpf.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2pmtvsmow.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2bfiwkikl.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2xwrocvab.html


<!-- 参考信息 -->