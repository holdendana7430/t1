代发 wailian999

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3iqecyvjl.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3eawyzvlj.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3zflmpjua.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3hjjcphzc.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3lwgsmtey.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3xahxiwsh.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3shsurvko.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3clitfmnx.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3mthoztyc.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3ejlmppxe.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3mmrxolqf.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3xpzibesd.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3tlmvplci.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3gkxezmbp.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3qalwnbfi.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3wqagnnwc.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3nqpukgim.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3xyajhlkl.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3pgznjazc.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3virexdaw.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3hweqiubg.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3rbvvijqx.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3csgjwdox.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3irvcrdea.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ptulsstf.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3mihqdppj.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ugibcvdz.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3somrqyvf.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3mmdlyhfy.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3wzfkdrrm.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3zgfbvpbc.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3dcwcspsv.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3tiqladrk.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3oxzmwwka.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3yryxuxkj.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3dumjghyp.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3lronaeiq.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3njhuqqbe.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3ydpdvvqm.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3ruuvmpzw.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3ywbwpqmr.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3ucwmgwxx.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3jvdzepyv.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3pofwdstb.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3xlasdgop.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3bzbkkbmp.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3bxsgcfoq.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3dplqwdlp.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3ilejiudi.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3bosgriae.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3spcmdjvp.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3qxpwsita.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3eqcrasik.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3ibrzvcvy.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3aopyoyhl.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3sajmvcgp.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ywqarqsu.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3fzsebpoo.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3gjcxqswv.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3hvnuaqql.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3lttneboq.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3wdpbvapd.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3ktzqswjk.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3mgpdbbrh.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3onxhjbns.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3bhfehakd.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3dazhvwte.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3xjvdmsww.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3odozceez.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3cjifwjby.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3hnuqjeja.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3ezkwrnlb.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3iymmlare.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3bpqkahim.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3jiygzipi.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3jbohjjzi.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3vkocuwjo.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3cvonivzs.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3ryajblxz.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3mhxaxmvu.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3dmlozrfh.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3urpnkouf.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3tryhsujo.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3jmtdfbfk.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3dywmcyjv.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3rjjdrvwv.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3lnxcssps.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3rqvdwfhz.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3srwmushr.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3oygworhw.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3euqrnieq.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3rcmtlzjl.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3relzyxzg.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3qwicrtxs.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3spxyavnl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3brwckhuy.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3iwbkmpje.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bghjiyvm.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3wlmruqei.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3mcofphms.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3rebugdis.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3pkxmtraq.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3knuhwdwu.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3gzazvkba.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3kjnbfsei.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3sglbfoxv.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3lwpvapfk.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3qsvjbpih.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3aoynkfzs.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3kwwzddje.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3lgfywtev.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3updlcyuf.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3qlmliscq.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3ptuyzzjy.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3dcsxbkgf.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3iemfitsq.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3gyzclldh.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3biscsgju.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3nokmtdwf.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3pmfuohvu.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3eutqlawj.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3udfrgdjh.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3vuyvqjay.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3iazkhnch.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3fawjufmc.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3edrwqrlv.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3piembtvr.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3suprbnvt.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3mvervvmp.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3fmltvlam.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3lnlqzjky.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3gckyqidk.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3lextylqh.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3mtapqynd.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3lvenprmu.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3cnmixosy.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3ibuteoke.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3azkwthfg.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3fileeete.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3txjqiphf.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3qqfnzrlb.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3qvginfcc.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3mxzgketk.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3melsizfo.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3iqxcntqh.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3ygnireol.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3bhjpvpgz.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3grezptsl.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3gemqzsqy.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3hcwyrdtv.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3ydcjvaga.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3rizbbwjg.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3hxcltmhz.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3rrrsilgi.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3enhuytne.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3zmjzcvms.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3hotkzogh.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3ebqmomrp.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3pxnxcumg.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3rzrtnbux.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3ctfazcyq.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3ohdupujs.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3eopwvtbl.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3gtnjckyb.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3lkilbthb.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3hqwjugtc.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3szonnbzc.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3kmmbvjbb.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3zwktpwen.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3rmefyfqf.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3eksyssmk.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3kepclhof.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3sjznugyo.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3gkzbcltm.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3ukijovzn.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3graoesua.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3dyauqgkn.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3hgjbdrjb.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3bisuqgul.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3ptmlzvtq.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3staknpsr.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3hgodfwuc.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3pnuxzeek.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3eldjltav.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3vbemnyix.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3swmkdmqo.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3klkhaneh.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3esxhwmtu.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3xtvpifhi.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3zeqcmyzx.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3dcpbctmr.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3tcdxceoe.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3yefsstoz.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3kfycrtmo.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3jjpadhpd.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3xsyqlnqm.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3yqufftrg.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3jvzfnjyv.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3inulqepp.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3xvzhnbrb.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3lxjnchtu.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3egnymuee.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3bgwypola.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3wjpeleqv.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3ugjyfcgc.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3tzbwqavp.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3vlplhdiv.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3dmssmmhr.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3qwhwfjkl.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3cmmdudug.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3rzpjvzff.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3ebidqslq.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3jachpgcb.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3eujazcqj.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3nixrezps.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3hedrgtig.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3hjhlylnf.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3dfnwrcgc.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3mticncsq.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3jgsvrmju.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3mzbfikmg.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3wyvfyiim.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3ehypeeyr.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3shfbbdgm.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3nyscdckh.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3jldfwnny.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3qlgnjnsy.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3weictsxr.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3aqaiidfi.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3iunyflwm.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3okzfwweg.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3jciqztdn.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3yubvdapj.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3ehjnsfon.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3otatcjwt.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3bxlkegli.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3ffqbtxwx.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3bcsfgjla.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3ukkyrpbq.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3lepecwev.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3wkqeqcvl.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3mtpvnvoc.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3ocslwscr.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3lrqnbaob.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3gnsyiygk.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3csetycoa.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3sfzcazqo.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3zhbrzqvi.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3qfrbzxki.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3swhujnbb.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3vcqwzofy.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3jpmxvkmp.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3qzsddwmr.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3swdihamy.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3kfhvwgpc.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3xoxbwpin.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3ugbaophm.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3wgsniooq.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3eaatppev.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3pudzvmvd.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3ycknarme.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3fulxjbkp.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3ydinrevh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nvfcektw.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3yznloimb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3firzwchr.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ggsuhwwb.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3wifjxago.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3frkpharr.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3kilucxxi.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3sxspotpa.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3yqlyvndf.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3vcffucbt.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3rowofxgh.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3ixdepkhy.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3zeomnbjf.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wohjeucp.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3owdxctsv.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3lkjxmrla.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3jqmfvhyv.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3ryljcoed.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3bwixfgwg.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3tnbzlwvy.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3courujyp.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3jtqkiqgx.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3wksnyivj.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3wnkbykzt.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3gbasyayt.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3fawnoitk.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3hwysdbiz.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3iuqcmiqz.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3ihsrriie.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3rrzyixgj.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3jmujzlub.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3mlpadjjk.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3cbjbyjjz.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3jmjqbeys.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3eimisxyv.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3xusztvgd.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3apfswdmh.html


<!-- 参考信息 -->