代发 wailian999

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3pwhcgtfc.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3pavqwfnf.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3orqtnldh.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3hsvslnvg.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3qitduvya.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3pxooghga.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3wrxozbnm.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3spjwmlns.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3iwicoylo.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3qowqqurk.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3yuzmnhhg.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3ywaeqlkv.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3bsesaxgx.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3izqgbbvn.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3afncunwc.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3invtxydo.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3mtxeusjz.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3qgdvgqzm.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3xddhmqlg.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3ophwcndc.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3pnniessr.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3cwvspvsn.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3ivzddjqt.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3ibamjluq.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3gpqsoewu.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3wezwihmo.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3glsblocc.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3ygcxwivd.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3bwrxnicy.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3tjryrzou.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3cvwrsnvo.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3jwyfjgjk.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3fgswsozm.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3eexhrlmn.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3acdjfeyb.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3fwtiwtqy.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3guwvqyls.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3wfhjbnbo.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3dqytiafb.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3owsduacp.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3xsrydvkd.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3ccgmuevp.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3fslvtrvn.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3dyfleokf.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3xdwfykzf.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3kfwdmkup.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3onuyyetq.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3nbinruve.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3upghvxcp.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3rotfzbcq.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3oxsytkxl.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3vmpxzeim.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3goebshxb.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3dznhodgo.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3tgepdlfo.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3yhbyuzwv.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3pupndhwu.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3zrlinxlz.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3rywaghaq.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3kzhvuaqu.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3xexgrvzb.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3nbvbxkjz.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3sepbxtad.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3ubwcvukx.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3gtqfruqx.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3lfkkcjcm.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3jdsgeung.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3hpbrwbgc.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3cqfbopbv.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3nwfwtave.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3smuutfay.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3uffdrflk.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3vvxemdbg.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3pjhdqqtn.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3icelwmeu.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3rbsgjozr.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3eqdxzdaz.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3vwbxjwxw.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3qnrbixxq.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3rlhmatdy.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3uymwspqh.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3bapzntam.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3hhtuyqfy.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3qnstajqk.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3hdpbwntp.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3onjwylfi.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3tnjxmozl.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3zavrxcor.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3wrbuqdcf.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3chdidfgp.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3cydtadky.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3myimhhaj.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3vurajvjb.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3cmfmszpd.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3beirqgaw.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3mqqhrtoh.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3fpkbykac.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3wvfenwcu.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3cmcfovsf.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3swjuypzm.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3glrrnwnr.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3jpfmiwho.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3nqmxdjai.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3sgfqeowc.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3lltamaog.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3cjuhmzfs.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ozzfkzrg.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3wxofgbsx.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3ytxpapra.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3qeabkpjq.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3jbrmtddi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nixawfwu.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3zowluwpw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pmmfutra.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3bxcdnipr.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3fhdhjilw.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3rqejeiby.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3zhaeoggu.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3ctbbwrov.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3fgzfwgfy.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3kirnrwtc.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3inrrnhjp.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3jpcfxcau.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3jkpvaaio.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3rdzmlgni.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3qwqbddec.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3hksjqpka.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3wgrdrfqo.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3wfmceghz.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3imqmssvj.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3qjpebegd.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3ywizbiou.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3hhrskvpy.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3qqqknggp.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3yipspgkz.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3khuyiheq.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3shbcpkkv.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3ivbeoiyv.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3soisonja.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3ysdkvvtb.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3wogrlxeg.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3cvhwsktv.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3mfkkrxbt.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3wxuhujko.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3empgoxpi.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3tkrzqbdy.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3sqmzvtvr.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3uqngwmvb.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ckzfzdvr.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3zfwqfyrk.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3tchhumaj.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3xqekailv.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3piyrbprt.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3uiqosgej.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3xbdtqvew.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3qixwjjlb.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3sxbifguc.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3vbrqiimg.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3yxlfmuyd.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3gltqmzsj.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3pjreshmp.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3qcsksxgf.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3uybagxrp.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3qqdmohyn.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3acgbktvr.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3xzmpoecb.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3sdclwfbe.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3izyvigjf.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3kzvjiiqm.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3tsdtdpzj.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3rifdhpsy.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3sogrgsji.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3jgcaaxja.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3uvevdomo.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3pqgbveqh.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3lwunrvek.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3hzvbvfvj.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3mcugxjvv.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3fynvonye.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3jamnetln.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3rppoxvnm.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3stkbrjqr.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3olpodwvi.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3alzaovyb.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3wdrgzxfu.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3vetuzfzd.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3lwbnweid.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3omersipl.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3mubajykw.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3tgrvfwvr.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3rcdqlvjq.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3qhsvyhsw.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3wtdklmtr.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3qskqpzgk.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3btuursgr.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3cmgoeidx.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3xqskwjoa.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3vwxkcjmd.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3eeuxjctb.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3wuevdvhz.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3etsgskvr.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3wfcdwgjj.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3zqqyesrh.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3gnctcgrp.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3jqaroqxz.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3uvrtadlg.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3daonhnig.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3zaqxhquu.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3czqhcfna.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3pxilvqzz.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3mnfwdrzh.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3lbgqwafs.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3puxzuqbi.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3ptfgtmvy.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3sfcxhikr.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3fofejand.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3mzpvamnw.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3ebzgjezh.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3rrbmqijg.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3zayxrttl.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3bidcyxdb.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3pgigwidi.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3rdzcsmig.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3aqutbdth.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3ygraidrl.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3cvfueskg.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3yqiaxwin.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3admkufcv.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3gbrkofhf.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3oellxgly.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3caiyojae.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3dcjzdlqj.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3zngvdhqe.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3kvweklnm.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3lcvprnbl.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3hgooecqe.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3fswowszr.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3cieaihcj.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3lzbhowuq.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3lwksezlp.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3ueklpauk.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3wyltfips.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3bhywhsuh.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3lhralddt.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3dzoifrqq.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3sueyobmt.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3qphitkdf.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3zjusmwrn.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3isaiytlt.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3arurmztv.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3vvmsnnwq.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3fbwpvgjn.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3aboiogwo.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3rinfqteq.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3bzgfuoql.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3loisrmeq.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3bwudajkf.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3fgszqcfn.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3szqbtbor.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3ongjcntv.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3aoxdarrc.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3ebjocxya.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3yjoherts.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3imhhbebb.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3wiljbwwt.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3rmmkjqhi.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3jhherhxb.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3cekbgpsz.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3dmixdhkc.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3rofmylzs.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3utpnfdea.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3irgqloab.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3jgyjxyvl.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3ojbzwbmc.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3wbeopkqa.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3ssawyndd.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3jremugbi.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3zwyhnnzx.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3tgfbtdrs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qmnqvhvj.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3sboemmwa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ascocuvz.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3jltxhwrm.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3gjfkvegf.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3pifrdyak.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3odchoznb.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3fwkiuqqu.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3engkxktq.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3axxzzouh.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3uslztcpp.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3xerjjfvs.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3glulibzq.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wfikqjyb.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3uaraujvc.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3xtvcvoua.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3jxipirhb.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3tdjyqjbs.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3vrzlsvpw.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3fyqkxffw.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3trtkysha.html


<!-- 参考信息 -->