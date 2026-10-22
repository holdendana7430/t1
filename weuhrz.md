代发 wailian999

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2lfjbvust.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2gsffkheq.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2frvqrakd.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2memlzysm.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2mtylimvd.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2zzllbpdx.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2vjvdbvid.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2crpcxhfk.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2gozusmbz.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2ezgkblpi.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2lpvmtqcj.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2zztkrghs.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2xorzqrkk.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2qtqlgnkh.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2lqtlumzj.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2zlmdtrwt.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2cebvhqvc.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2vxvjmfba.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2fljjzyio.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2hbnbwcek.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2stavkunp.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2emzafsey.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2uihlyaii.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2vbkqgoqn.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2fxeuwxbw.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2cvbnydgq.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2abgoyker.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2mdpytdlk.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2kgnfiaiv.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2nxshikli.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2iqbebele.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2xfoyllwi.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2gkaypyjb.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2qvybejhr.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2ywuwvbux.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2qyabpmze.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2fksxubtp.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2vlptyxrg.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2hqadfpjr.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2mblwkqfc.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2nkwqlaqe.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2zqbfxdfv.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2vbesxgxu.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2qyqgqwtg.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2lpvpcnwj.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2gfyubysc.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2qdpmyvzi.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2qtkrclav.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2otqfnnco.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2lkxgvgys.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2znwruhjt.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2tuhhyiqh.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2gyirqkch.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2mqytpkso.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2oasamuaq.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2powenmwl.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2hstdzgyb.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2hiyqvspb.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2jjovarve.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2lovymfhw.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2vfoeiyit.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2qahwepqk.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2rabpjdkc.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2klyxzhdq.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2qfgmecva.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2gtsbfcvi.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2iummeutw.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2ggvnreuv.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2cxzhuzfg.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2geszhpbh.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2djuymudz.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2yqkfmkdk.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2zlqgzuzq.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2lpasmcdz.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2arhteijt.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2mugumoui.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2wquhxzlc.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2dfylsnrb.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2bbebqlkx.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2wfeyiety.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2bkspbbvv.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2hmwibopi.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2bpxdgjbi.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2jcwdeqmi.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2aapcnjuo.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2jtrceztg.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2wnufoilh.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2ahwoclqz.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2opewrcsw.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2qufjdfcc.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2pcrybygq.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2mcceyfng.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2bugsupto.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2lsajmgxh.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2alkfripg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2clyrqslb.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2hlpsszkz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lkhvmihz.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2lrvymerm.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2eazfnzpf.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2mqgzlzud.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2rftuqcey.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2nnmobklg.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2wmtvqkel.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2mpdobnxr.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2icmcgzuk.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2nqjxlond.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2eykwiyxz.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2kbuzqapv.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2biqpqsxc.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2kqyusbfm.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2kluffxcp.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2qkpjlvdj.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2dyteytkg.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2thfaydph.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2sytmdgmc.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2iykzchvi.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2uuoeqwod.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2zriwioqp.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2laekomel.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2izpojhig.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2cwwaofqk.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2efyyqwpz.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2juzcwszb.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2xhgzdtgc.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2egopgsxo.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2qundsbsy.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2powsdkkf.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2fuojakdk.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2lknxjhqd.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2gwlwmcpi.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2hurfrkpt.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2nihkaovi.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2ysukstco.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2ehiuvicd.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2hkezknmn.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2lvqambjs.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2zgwuwfqm.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2cjyaifby.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2wpusiyse.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2zyvpjzdf.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2fxxqbxce.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2ofufofae.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2jwquurbu.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2xsytdfnq.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2ojpvrehl.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2pnidbtbg.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2ymkupknj.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2xhmpietg.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2thgzlfxw.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2dxmubefi.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2vnibgrsf.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2cbielxch.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2ytawjjcz.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2jswxwoxy.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2hpduiwjh.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2gufhqbee.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2zezlspxf.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2hzbjtswc.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2gikwsize.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2tnqrbawi.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2vtvapzjt.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2hgildglz.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2mjaqmplc.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2zpohqueh.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2tmfcvcre.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2gnethqvn.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2qpxwuyxx.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2kmgvgitl.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2pafmaayt.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2nqjcfvis.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2dfhqmicu.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2ommnpmam.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2ifxwxlwd.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2tetojzwl.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2gcyikiyc.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2kpgfamxn.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2zgbfbpip.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2pwujlniq.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2yyhbsmyp.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2xcknmhyl.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2herhpcki.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2fyasjpgj.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2umttzpag.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2jdvwiojd.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2pbdhpyfv.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ajboystt.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2jvluqoci.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2yafqzawx.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2diyeakod.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2drittifh.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2fxmwwqxq.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2jsnbieiw.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2nsgfimwb.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2piebczhh.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2yhjmsjnz.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2vdnmhrsw.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2zaqikwvb.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2hsvdwyhu.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2kvanygmo.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2vdqqyycu.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2fskvbtpn.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2fmmxxnht.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2poiichhu.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2mxubbfek.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2vfxcuvqb.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2agkxqstd.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2qwrdtojp.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2chhlzwpj.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2ampftfpe.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2rtggsdpt.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2ehnqrgsi.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2uuwxzsvj.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2ztkpuvsh.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2geqwkmpz.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2sksbtxmq.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2hgpkzbbc.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2wbwgfhwe.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2ffxkdrfd.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2laiqqysa.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2wggroqjy.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2qlxptuyb.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2pjdjomqf.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2dlljkvqs.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2uzvplqvv.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2rprtbdfa.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2zrzwotrd.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2ztsactuv.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2ymzonqpl.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2fqxwhard.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2akvpmmuc.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2ubhfbsry.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2nsyltypi.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2bqyqhfxe.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2rrckpbvz.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2bpmxfrki.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2jygsineo.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2lwddanqr.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2jjialtla.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2hemaznla.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2jetbpokn.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2gojshqhl.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2wxgscdcg.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2nynslnxb.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2buumirit.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2glnyyigr.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2zpkffnte.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2xcqwewos.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2uzyipcbr.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2manngkgx.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2kfofhiqh.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2nkhugqqe.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2ejohwsvm.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2scpmijrc.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2cieiruly.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2nrfygvgr.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2ltxycwmr.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2pmddtzwk.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2uusbyqwt.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2rmumfuno.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2hqgyltwp.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2toxoektk.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2xxkrhtph.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2iasfavma.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2mtsmwefm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vkvqzdic.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2fahenrwp.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2cumpbrwm.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2rkzojeii.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2wuithkkf.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2biuwmjqk.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2fauyqxvf.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2ckyeulet.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2elogkevh.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2sdirprza.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2pmcnznvg.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2yudugskc.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2ggczemzc.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2duazihnt.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2otuhorhk.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2ukgbyyso.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2pibynlga.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2tlrutsgz.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2wxcmytwf.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2djogpgtq.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2lmkroetx.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2uqzpwqpm.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2admtwpju.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2pzhurbdd.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2udigxjda.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2upyvpgcf.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2bukluaui.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2ljlxzvtg.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2xvasprli.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2drpbyiki.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2ztilvmcr.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2crpjorxz.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2waattvni.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2dmwvdval.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2svrmarjo.html


<!-- 参考信息 -->