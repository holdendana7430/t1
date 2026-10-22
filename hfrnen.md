代发 wailian999

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2ojpducfp.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2eyeyrzne.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2npmcxxwo.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2eezzmzkl.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2pacwuiwy.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2uxkqpcyx.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2zvfowibt.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2vfepdwie.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2jvqaysqp.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2uiqvpfzt.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2lpnvxchu.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2qfjraeat.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2zukyzbcv.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2wnszudbi.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2bsxxunkw.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2chyasjkf.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2axpsddpd.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2ghuscdto.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2enchymcq.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2difuakja.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2rmzxgwoo.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2tlhrvebz.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2njzablnn.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2kpreedkf.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2gzqcgoko.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2msxxxstp.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2mqborgxv.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2uszyyvmv.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2ljguozpw.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2wezhfgbf.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2cjjhjllz.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2nzpcdzav.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ovmsrbkk.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2urkooini.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2oppvpmwf.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2qqgzofez.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2rheebeez.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2nidrkwpq.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2qmhwvlsk.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2mxdsxuwc.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2vkrelcgw.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2snuwzhsn.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2hotnzzvm.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2cyssjasg.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2vcmgfyzh.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2xicfowqf.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2dvejwcul.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2dsqclgpw.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2cbvgebgd.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2maujtqsd.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2knptytls.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2blsgdtti.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2gcsesecd.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2ztmuaztq.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2cjrikwvf.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2pgpeqowp.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2ughrasdy.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2silrswbn.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2ozusyrqh.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2yzridwpz.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2xjkohbbh.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2pdjkwcdn.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2xnizeaer.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2tfvhvsid.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2oxtroqaw.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2diebmuae.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2anjxqwmk.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2eeuktbop.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2zpcrtdqd.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2bwwejxet.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2wyqyyaxt.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2gnhoegws.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2awovwusk.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2wqvhcyuu.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2xoxugofb.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2mmarrnvy.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2ngahkxfl.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2helqqwfc.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2ehzqzxgl.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2jabzlbrj.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2quxnlaac.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ihnegswh.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2eamyzdza.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2vpuhmdog.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2ownqhcpi.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2cwvdglfr.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2tprxubiq.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2uurzlscc.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2gbqzaqck.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2gapvrmxt.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2dueqbztp.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2yyvudgyz.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2parzecpl.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2myoqaark.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2xhqyryvm.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2nvgonjyn.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2nfmxwibk.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2uttlcywi.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2lbtgizmj.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2qcssgzpy.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2nwheqsou.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2gzdxblxk.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2ncxxjpdc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vbhjznih.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2zpvguhgx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qqxcjmdm.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2thewyzmq.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2hgneygst.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2gfiivatd.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2xrgiaoav.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2cwjxcdpc.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2qhjnzrgt.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2wkvqvfkw.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2puiqrvlg.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2puuzjmmt.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2fnvfbsyp.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2nsbvrtyd.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2dyatsnpn.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2noehqsqi.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2ipqbhzxf.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2zabtcoug.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2puzhkori.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2ksnbzfwg.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2rnoekkad.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2djrkxwrr.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2itnlsjff.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2tappqqmu.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2hbdnauwr.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2smwmwwxy.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2wytrfjei.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2pneczdqf.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2jzajeqdi.html

esac
来源：http://www.52xcode.cn/Article/details/gt2juefeffa.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2jowhzshi.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2tweykvxi.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2nrvsrkme.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2shlrjrck.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2rftyoefk.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2riwdvhdw.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2tplyzpzs.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2eoaniuuv.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2hztjjoxp.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2obumhuuq.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2oshykrlu.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2yllcfrcb.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2xrjkrvep.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2ngacpepv.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2oxetywgo.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2tdqjmiaj.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2ubnpmldo.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2zavfqgnu.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2dqoaiphg.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2ypaaxogq.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2ggdgggbt.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2tbifsrdk.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2yafzylnm.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2yyjqssvn.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2hwpqkjmh.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2vznkfaia.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2uxvqpsqi.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2ysavvtjz.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2scmawxew.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2cpgimgou.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2aabjulim.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2knuegdxn.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2evdufkwx.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2vbcdcuqt.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2pooymnyt.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2zjvsebge.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2mwbpjmxg.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2twctnrmt.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2imqoykpz.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2zyqfchan.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2ztlnqbqr.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2rxyyztcp.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2hjsippdk.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2fsmyzuox.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2cvpnpfym.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2hkucmcqg.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2hmpdvebn.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2isulfzuu.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2hiajgjae.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2vnnatcqx.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2vxlgvbfs.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2wwfuruuu.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2btzgucdo.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2xlhmerte.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2vquzfrsq.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2uvayldpu.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2ryyzkswd.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2monqiarh.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2mcgdtavp.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2kiehutkt.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2inoowcrl.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2abypzjvx.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2zahsoqzo.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2ucvebwhn.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2xcsqzgtr.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2lgfjuaqh.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2abjoabhm.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2mcymklbm.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2cxhhsexm.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2dolmyhvv.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2nvkipclz.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2vjdwigll.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2cksxvsms.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2evhasckk.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2rfewnccd.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2czqfompn.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2nkzatnal.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2ocbozyvq.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2veekopux.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2xtpdknea.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2cyvsjoqp.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2lpvuxuyt.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2rtcacgqv.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2eutrftbb.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2dezqpvue.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2iarpguse.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2xtksjinr.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2bpnpxgrx.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2mwxyxaij.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2pdyqlxhy.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2kthiwvay.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2mnzapvjo.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2bsromwkh.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2azvmmppq.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2voabrmaq.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2ixcnkmkt.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2gaukrvyc.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2czplnely.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2ktydnrix.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2lovfvnuc.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2glabmsbc.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2izqpljcq.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2qmukcabz.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2dhmvukun.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2gbabmsxy.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2lbjwhpdz.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2gatzkrwc.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2zejttwth.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2inkrupeo.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2rscndedc.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2syamkokk.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2yffxemvx.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2nlebgofs.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2oakvxues.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2zagqqsmr.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2ijurczho.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2bpigbhsv.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2vtcdzbds.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2hyximqtl.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2azjvjxbp.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2rbzhadtc.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2dughgebf.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2gllvvlpy.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2apizxwtf.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2fkjkromj.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2apqoyusg.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2kymttjgq.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2vycwehev.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2ugbpvqlz.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2zyvjobqv.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2hnpbjsby.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2jgsilvjd.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2lgapvayp.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2gccjxzyx.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2rmntemsr.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2lzlvnaeg.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2xwtzttrh.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2dansdmae.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pordzbkp.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2xwbltrbp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ibeqxhcn.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2mikzyydw.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2xtkihysf.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2hvsxdumm.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2lukmpfyv.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2holtigeb.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2jewahukv.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2edebsxjz.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2xtjififk.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2ujtwmpty.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2fkksryiv.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2yzysuizc.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2uomslafr.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2duwvxdjx.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2uwxaavfh.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2lamkrfgl.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2onwajeje.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2tltctwyp.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2sghixkhc.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2rwpknsca.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2yayvilyo.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2analgwcd.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2ukeyqdxk.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2hovejyrf.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2jcidemwf.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2yzoywioo.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2rjgclrwd.html


<!-- 参考信息 -->