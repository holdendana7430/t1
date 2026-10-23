代发 wailian999

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3aoylgfxt.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3qpvwfjlc.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3wfzuecqk.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3drkozbwh.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3emwhoxcw.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3dnnxpgut.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3vajrrtda.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3rsgpynoa.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3ofjfsngc.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3qfinsvzv.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3hqcmwdgb.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3gaqamrqp.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3hlfvhnrw.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3dzlvprbs.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3yrfcvouj.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3lcwcrwlt.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3movgyfhe.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3dvimnueq.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3urqzanuj.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3uajbzfrg.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3zadqldwz.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3musodalk.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3uuifguuu.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3cdnnumhx.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3vfhwzabi.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3zrlssfbf.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3izncqwoa.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3rlglesbp.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3dupefpde.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3rdnlimew.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3dscwiozd.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3fmukxvvb.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ntyiydtm.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3etvyfcyo.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3pxsjqetk.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3cknvhdob.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3uepwlxgg.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3frrejwtg.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3kdtuluni.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3hviyfnmi.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3bjilctav.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3sjufujwr.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3rcgetzto.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3bhhynpfd.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3clfukryh.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3mxivoxfb.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3uvlyefup.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3prlqbykl.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3lbfghpqu.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3uljeshwn.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3cencyqpy.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3fobmxdjf.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3zgogxckc.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3wvdzfeia.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3wblntokb.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3bucqdkin.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3qnwoaivz.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3eerdxwrf.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3iuuesbkh.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3tsytyyca.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3uxwaxipo.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3ixrapmzn.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3mddpsfgq.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3teryccqb.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3cqagigsj.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3ecdyhcew.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3nwftijse.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3mawivpgq.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3xjwxvfoc.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3cnddrzhw.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3kwyubaru.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3orlocbln.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3qizxfass.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3sdfagogq.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3bmuodjvi.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3dzmigavu.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3vconchlb.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3grhpnbjc.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3qwacxooo.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ydgurpeo.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3ptzsqgsu.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3lznnsntl.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3kmbwkigi.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3xewptvbr.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3mblhcsus.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3rfqeyiye.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3hrhupkoq.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3ewtzstjt.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3tgurkcaa.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3ukhyjbfl.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3txdkgqek.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3jnuuvbrj.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3woqfigsr.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3pdofrisp.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3irshnqpl.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3caykpccu.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3bmzscrqk.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3xemptlbv.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3ulusbuai.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cctmthmn.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3dqccbvaf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sjqnspfp.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3mxpgtggt.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3pkkytogv.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3vtrsgboc.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3sycqcrho.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3gywibeya.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3gycncsmc.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3iaaghdbz.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3iqnxdjvt.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3wnqoupax.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3bwrbifnr.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3uygkflpq.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3jvpflirm.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3yvguquaw.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3jnbcjafo.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3lfekrstn.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3ajkmpzjz.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3qrxlefjk.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3kheasivw.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3tiuqcrvc.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3pxabpxwe.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3qkrfjzau.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3ashrjces.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3anijadpk.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3wbrhknbn.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3pkazjade.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3dtpnrofi.html

esac
来源：http://www.52xcode.cn/Article/details/gt3lmtrltyd.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3ipdnyhdp.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3sscjguvo.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3gewwwgop.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3obudwplx.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3czqmjjef.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3hdfmxiju.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3bwqmdhlk.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3gesgkffb.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3ykyjhofw.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3gqepltyj.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3wxvlrwti.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3bhfksilw.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3xwbrohvv.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3ffdiyean.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3qydthvmq.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3iwnsjwap.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3tmcbhuqa.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3soswvgoe.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3qgysxvox.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3kofqomao.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3zgehlyyx.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3iqqchqud.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3vrgupgpk.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3xiaplgtr.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3ljkxxsts.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3fivzxcjd.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3ieymxrpk.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3whmsfqwu.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3aimxybuu.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3qvchapfm.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3ggzogufb.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3nhrzucsk.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3kycbukkx.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3enodcqik.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3lxdfyswm.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3myugmybv.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3sipbggty.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3rbfdubyp.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3dquhiqcc.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ijyqglob.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3mxtsqkmd.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3yslqjhqm.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3agbrmlxv.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3tkzchnsr.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3pkoqtiyc.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3xopwcaqu.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3lbzxwjcy.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3pofznaef.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3yfomnnvl.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3kqpqmeiq.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3ixltffhl.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3qeqgazhj.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3okspiwnu.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3qvuptukn.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3kzmuhour.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3fznsitoz.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3admozdyo.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3rajplyew.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3hdsoktaa.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3mdzfkgzh.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3faqkxyah.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3cgibnwpk.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3wfbrhtkb.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3eunioawe.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3xzzuwclg.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3ttlkctao.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3qfqfocnb.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3ovkrojkw.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3kihgppkp.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3ytvivpso.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3uwdsslqb.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3lchqdwbq.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3dpkjqcwz.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3yoqcrwuv.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3nwvjpcry.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3ibyspzly.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3ifqngouo.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3tzcyyoac.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3lpuhhqtd.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3gxwgmvcl.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3sahhxpgt.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3waunewxb.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3hzqmbqdl.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3bqwpolpy.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3jabizagl.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3gagyjfxg.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3pppalqov.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3kbfxiqbk.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3ipwddkkd.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3vrjohcwc.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3cjqumivl.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3jsiubvwk.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3mtgzybjx.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3hjthyzpy.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3wbtykalh.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3swnfcohk.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3ywkkurwg.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3pvphdzwn.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3nwkugnyj.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3dovrubkr.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3xbewhsdu.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3eqtvjikl.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3repmdupb.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3vmqcfajd.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3qxydcdtw.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3hwqfgstk.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3filoossa.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3lxxyscgo.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3rnjspkdu.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3imdorxcv.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3cmxvlvph.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3drzkpvwz.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3bjxysvjk.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3fntemgoa.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3pzeurjuq.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3huinxicf.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3xzwtgcvq.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3emmripma.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3uqqaxbkr.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3yxveohwp.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3vazfniir.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3gofqiaie.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3jygrsxbd.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3bbamhbeo.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3djqlkvon.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3sikjirkn.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3atbpylnk.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3deolidej.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3yffejuzf.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3ntspwybz.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3mibbmnzp.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3ehamfrwz.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3umuxvomo.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3jftifuum.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3xvbdhmbw.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3kanfumqg.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3uefrzvcb.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3ukxcgsag.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dumdyumw.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3tlfapdzw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gxsrgrfr.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3mhaoolqy.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3lzvhvnvg.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3rtnwpbrl.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3jgnebhjo.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3bdnxvljf.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3jkpzddgr.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3sfvgkxyt.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3lpssedsc.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3rvvtpffp.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3pipyocpd.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ajxbrcgw.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3dqlfajlh.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3sqehvevt.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3dxqyshws.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3jptkuixs.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3tjmpteva.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3arhzvcgn.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3ccdkogzr.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3nvsgehdo.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3yatpzfxt.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3nbqxhlhh.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3yzxhlibi.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3lqefqrly.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3dorqaeru.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3seiffwsb.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3wkdsbxvy.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3ffwscbbt.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3ewecocsx.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3axejrqsb.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3cyvqktgy.html


<!-- 参考信息 -->