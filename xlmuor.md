代发 wailian999

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3smdcnnvj.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3vvfkmqqj.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3sqruxajw.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3dmsqgqik.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3peahiqsa.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3wbfctqqr.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3izqugpnx.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3awcetcur.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3hxmtqdab.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3fucogvbb.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3hmutiyau.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3ybcqsijp.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3mccrmaif.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3ffdoromn.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3ulbxrxyw.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3zjbuylmv.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3fuynfphx.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3ccwqlmct.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3zyvwihwy.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3ruukzgxq.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3vezwskyv.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3qbewxfdt.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3vpknqjhh.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3txajiiou.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3phrnpbuz.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3loyechmx.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3kplxyilt.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3jeamxaer.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3qxmhuyvc.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3gfqsbezt.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3kbkqenvg.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3yibuzfkd.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3lgtxbyjv.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3ivjfarnb.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3aqsiebhd.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3sgmcwjwx.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3hhzuzddi.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3wxleanol.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3spkqouxg.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3sljfrasn.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3quychzvt.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3inqxmwmn.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3zgdxuajb.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3rdvrvsgp.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3ksofuiyd.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3ccssewhm.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3yjftitrt.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3pfrezchh.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3gotojpnc.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3werxqctl.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3wwizgusq.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3golvddbl.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3zeffekyh.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3rnvsgons.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3npbavwxz.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3vucppncs.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3diycvkzb.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3sszgvkex.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3saugutzf.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3bqtldpar.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3bnzpbpib.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3hsebvydn.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3qwcmcvoi.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3zjjapqzq.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3pqtsomil.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3kquuqrcf.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3bxenjdir.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3dktofyxd.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3vesdevdi.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3lbhgrtri.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3atpbkjke.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3lanvlawd.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3zwxeglwm.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3fdwbhdhx.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3zgvykypr.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3zbtjkrnk.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3dftbqvgf.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3tdkhhfki.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3ljdyhnqs.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3pzrgdkve.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3uoimwsnf.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ajcinndh.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3srxsygqi.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ymzksnnj.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3ncuhjqgv.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3kridjysp.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3ywbjqfga.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3egarmuye.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3wanaarsc.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ftkotgim.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3xziialtb.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3ainngdqk.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3htqvsrzu.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3etqzzbgh.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3thpzyjff.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3ikbafwhz.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3otphawtp.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3pmpbdqaz.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ectovlhw.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3vuradudh.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3kvcnoqau.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3zsivgwnn.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3dyemroqk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qubmpxgv.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3cwuegmqe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3baoncewv.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3xxkmdeqz.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3yzccqlon.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3hgeunddc.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3pzdcsmjt.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3xzpeybko.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3wonekrgv.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3gxoqcfnn.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3ozvilhsb.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3yifvtzyf.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3tbeepfnb.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3uvitkvom.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3uhxifksq.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3oagixzgj.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3newpwhgm.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3kmdbtmfk.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3niiafbyt.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3lkqwpcaj.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3naqkxlvz.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3jjhphawl.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3yjjhnszz.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3vsewgtsd.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3pzortqkx.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3tgenhdqc.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3fzvhcfvu.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3btvufnpt.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3pzemdrms.html

esac
来源：http://www.52xcode.cn/Article/details/gt3ccqgjivs.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3jyzmarde.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3wtkczyuw.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3sgprbgqo.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3cubddzyu.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3znhlmeri.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3jphymayt.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3dthnilsa.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3dcpzypyi.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3ncdcghqo.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3oewngbsn.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3cbmkyjwv.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3ggzbqgga.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3kknaccpa.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3sfxsozqo.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3oikrtmbi.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3obeyweqz.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3glthizov.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3xacrbdjx.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3bynpodas.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3cmoxjbhg.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3fbhixbjk.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3eoaowksw.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3boogwucd.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3ysatqxup.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3qixpdpcu.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3usvldhkt.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3yzrzyqvt.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3fkpqxctj.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3tntbqhoi.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3efonachd.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3adefyqbv.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3dbafsmrs.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3typydsyt.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3wkplbcnt.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3olphkeeu.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3gjjqdsyt.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3yygntvos.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3kackoktd.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3tlczaonk.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3zvplybam.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3jebtzdyg.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3idylairg.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3qphjvmoh.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3fbjbcprb.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3ncalqnfu.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3kxtazrtb.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3rjbefiur.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3dvlyldzq.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3zdbhjcxu.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3pptgvmaz.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3nkobjjoe.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3hcjlkzco.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3xluumbqd.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3ayqilvnu.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3qyzmnhkf.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3ronwpaqn.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3mzwbmeme.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3wfuraxij.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3siknokgx.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3puwbwndl.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3qofkigbp.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3vxppdbcw.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3jytppila.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3vbtyqymu.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3plsaysug.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3gkntirhd.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3hrctovsm.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3utiwtshd.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3gaafmurt.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3jactzues.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3jxbunpkf.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3dsevnwcn.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3oicaoldk.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3pwlhopvv.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3jnkzzhjb.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3ahpibooj.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3kzxhbvxw.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3jyxrhlzy.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3xppqfzgb.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3fjohukjp.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3hnklqhot.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3xasvhzfd.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3oxpajdpu.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3twgqqtkf.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3rucnftgb.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3ejqjnnpb.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3gywiilvb.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3arommkbp.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3oyinzxsn.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3rbpevnnb.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3atkwoqac.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3abscwyrt.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3zausqlid.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3aoytlrur.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3qvhqpvlx.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3lmraxwwj.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3falgjlia.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3otjculip.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3ncwvppib.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3cnihjutx.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3avaxxryc.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3kqebbgby.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3rgszbhos.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3rvckdjfj.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3vwqdsomr.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3exstoqnn.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3lhbxqnfw.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3jddhnzkx.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3iefupouc.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3vjygpnpo.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3bvlybtwl.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3vzynkdef.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3ehsemuqp.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ooegdtqh.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3zapfzgpm.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3swcwotse.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3xwtrihhz.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3ptarlklz.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3jqgsiodh.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3xgoroeyq.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3mwdalmzo.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3ykplhapt.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3oaobxieo.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3sceixzvc.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3rzkldigp.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3elvolljp.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3vfvltpmn.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3rdvnhwup.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3hpmlqcys.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3egwhnurv.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3tcqlmfez.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3tymaerjl.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3fvfjbyzd.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3glvluisa.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3yqxwxhpk.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3fyrnhsje.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3zxuxdoxx.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3zqnzxxmd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wlpiwdju.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3sawanoav.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3idczpgir.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3wcyqstgx.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3lbvvkvzw.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3lgizojes.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3hddkxlmk.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3jgynifzl.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3cvewwiux.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3hgzgpfwf.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3syogdkqq.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3fghzvkoh.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3bjkqggwy.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3kzsrabpc.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3zdcadfsn.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3qfumrhlb.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3icepcnlm.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3payobqsf.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3fhpwylbj.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3rbyxzkzn.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3tghjqgks.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3dfkximai.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3qkbpquqs.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3jnpvoxtb.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3vzmkavco.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3jepbrwdo.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3uckogdbb.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3uqrgrcyr.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3xshfexph.html


<!-- 参考信息 -->