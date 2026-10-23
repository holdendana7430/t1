代发 wailian999

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3lrtuiszs.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3bgjlkssm.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3jhwhzoed.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3tvwpqbhx.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3bdiumcrc.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3shrymqwb.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3kyueuqlw.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3nlktgvvz.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3tlrrbcew.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3whrfrdhk.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3fgvydznm.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3swisbvjn.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3yvgxkhuq.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3hgvgkluj.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3khfncpvu.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3ynxtrecq.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3biimqlaq.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3uokeouqx.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3hjrrkwku.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3kmtnhejz.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3yljepodr.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3zgldzyyv.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3iahkveww.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3khswpdau.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3umvuzkij.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3pgqmqipn.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3uaxmrwdy.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3yzojhgin.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3zdnqendq.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3vchpsvas.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3divowmrn.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3iavvblqv.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3qqtchpfs.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3zbyehzhb.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3qejsdxzz.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3cygqcldi.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3gtptioum.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3vrpukwgj.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3crtyottg.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3cmdzwsiy.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3drjpifax.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3bvvwijnh.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3vdbxiwfd.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3kqmegifl.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3fyacbgkt.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3lxaqsboc.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3zjgizsou.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3vluaqvdo.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3jzapskyf.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3oxutxinp.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3qrdhjlqf.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3pzdjgbwh.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3caswetjs.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3uikntels.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3lvlylwbi.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3xpuzwgyb.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3bodjbuku.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3kwwizzlu.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3cvjbiymd.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3pmuixzti.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3pmjyanru.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3aweowryp.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3rduaaaoz.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3qkvcyssa.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3vykszyjz.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3xxryvxqd.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3mmsnnuot.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3hfxranjb.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3wrcdnpmy.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3lhlydqxh.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3eezptnpu.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3diknlgeq.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3msaiqmln.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3mpnyzvqy.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3udgignxs.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3bznoierr.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3faenoibf.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3uwdlfybq.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3kniwexrj.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3qfvslsva.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3xzrkyvnu.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3jntzzkkz.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3pjqrdnpo.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3xjsnaark.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3tfexnaks.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3libalajz.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3umjyfskw.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3invzdfvk.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3lueczmed.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3waqbzxzk.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3iapasrwb.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3nijedmze.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3voeciegv.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3muxgynht.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3ucbkguoj.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3yikxqenl.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3limawask.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3wmfagrnh.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3nbppkiyk.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3htqahtnj.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3fusagaea.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3twsvmhdn.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3vunajbgt.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3jektcpnk.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3uctpltiw.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3qjjclxrh.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3udxhbkly.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3imwyoajg.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3xqpbdduw.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3pfwtvxmz.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3oueuaoxz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3aocjkmhr.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3gfbhrhbd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3whphwlrj.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3izikgfag.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3pbpcooun.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3jguudumg.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3yhwtbpvh.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3fuxzbpng.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3pqegqitw.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3lhivexkm.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3yexeklup.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3xhwadwwb.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3xypabhot.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3rkbaaolb.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3ynnbmmxk.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3ksaukume.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3oiygmetg.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3vqaneiji.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3dlwxvqwv.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3hsuoafcx.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3qwbaajcs.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3hakxajow.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3xusipoah.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3rebtwixb.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3kbbhtjkn.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3ieojpnfe.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3qiaiyttl.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3qkbvmppp.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3bfcddyub.html

esac
来源：http://www.52xcode.cn/Article/details/gt3vhnipkui.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3oowryjlu.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3penjatlr.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3hyqdnkto.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3yqqergcw.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3pqscejru.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3wrticxot.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3uvbjahdi.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3navmzdve.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3adlxxkcc.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3baqockxy.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3xbnnfnxp.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3qozpmisg.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3xwhzfrra.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3bsbmcqxc.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3pwcslhvm.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3xdrpcknl.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3oyxekcew.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3owrhnnqd.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3mndwruvf.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3ybzvbxoq.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3yepiuals.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3zoysqjhr.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3lwamkcwx.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3yqhwjbur.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3rsrrpdgz.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3msonbvls.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3xqubezvs.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3qxvplqrb.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3thwliscu.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3yxoolpjf.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3hdevqwuy.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3dwjfcqnf.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3psxwussx.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3ngybyztp.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3hzljkpaw.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3qnmfwcps.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3bnjpeucd.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3rhewlufg.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3pyjnpbru.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3lfqqjphi.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3kdblvkzt.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3zmnpfnkh.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3abakjhvl.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3ojbontxy.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3wbnhwdkz.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3kgehicqi.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3kqsztqir.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3keugjvsd.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3suupmqpi.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3zvdmxgsq.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3hlbvshyo.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3ipnnazxj.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3hbjkwjvm.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3raydptcu.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3lsybaqtx.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3qgjaztgs.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3ajpxhyiw.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3hpkfbhvy.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3vgoblpuh.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3cwoorjws.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3pniqbwid.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3lmzeyjdo.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3rsmkvtyf.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3eyhahrzw.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3fljfhlvp.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3kcelbswe.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3csaapdis.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3bsnryozx.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3icngssvj.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3hylisinc.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3qvthfgyo.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3lrbxlbal.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3xtqulryg.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3lrtpklwo.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3ehuqkbxd.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3uzfzhauu.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3owxxmuqk.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3lqwoazcr.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3surggnfa.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3ijwsufms.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3fawtmixz.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3wfnhxnnc.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3vjqvlyqm.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3yqhwkrab.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3ofgypjkl.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3ssynvouv.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3oddmslbl.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3djwpmxxp.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3xwwyuurv.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3kqppuhmq.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3pvriryxe.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3txjypnoe.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3wpnejnci.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3zrvkgbgr.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3mfdialie.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3hphpwrbg.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3kezxicmv.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3spqwgedd.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3vjixzepn.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3leqzotrf.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3vygamwsy.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3suzspwro.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3yuuvaryb.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3xpzzirgl.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3eyubeqzm.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3qbxxqyxs.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3tieookhu.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3namqupyv.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3jrmgmoak.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3ephslehf.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3yoijpvzo.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3ngobgurs.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3lwwvqmiz.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3nqapmhhc.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3mxjchbil.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3wptkcnwz.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3extprrgh.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3sjcbrnjm.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3mvpfxoci.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3wfvkhchb.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3nonoyawo.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3doacpaij.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3pkvttnwh.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3nxlbfzwp.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3ncrustfl.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3dqsvglvb.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3aovbqdla.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3nuhxnshn.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3baubhoss.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3bphpehrr.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3tptfgngh.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3vuersiud.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3ideexaac.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3jlejwole.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3kacnaqlv.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3fbqupvxg.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3vrbqxvog.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3qccosiyw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yermchpb.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3lrlurwam.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jcjhjefu.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3dunykipl.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3drvdmdpn.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3bdjgkpee.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3clkszuan.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3bsqtxott.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3eykigqxe.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3vekyipnq.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3ctymbkdb.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3jzmegvyw.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3frawddwi.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3eyhtvykx.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3sveejobg.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3nujttxrs.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3ufpkqoza.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3lfbfrxui.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3bkskfnnb.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3dfzoijsl.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3yorsxjew.html


<!-- 参考信息 -->