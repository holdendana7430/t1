代发 wailian999

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3qaabjfuj.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3lgcxatwh.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3ykxqffuj.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3dksdipvc.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3sqozgouk.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3pslmqfrt.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3poivfqvf.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3padbrbas.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3pokelakc.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3kidihfid.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3duqwgmmu.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3dxfareju.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3wuhdcqrf.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3megkznjy.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3yhoagooy.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3jwqtlmwc.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3ezclwfzk.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3przkwwip.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3votzedip.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3xxmkhvnk.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3ooybtiyj.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3pafsnxer.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3hkmrapeu.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3koydsbam.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3pcialpvs.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3tcxvlvev.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3pmhkqjze.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3ezlqjbon.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3lqtghulx.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3dgmntjaf.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3ijkezsbq.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3ksjjhyrc.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3rhzwwvfi.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3fpdhlkdo.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3usawpmoj.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3xuiajcab.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3qofteemo.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3jekbiznh.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3isuhwrsm.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3zhjpcfjv.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3zzzjmmus.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3npjnbkdu.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3qtkdcfps.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3tixbdfau.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3xsxzeqhh.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3sxusrsab.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3kunftrkk.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3dhfqystv.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3mvbqbafw.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3gbccyfmp.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3qletzkoa.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3yijtuqdm.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3lhywgkvb.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3jmjvxkwv.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3dwleitow.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3zxjovfmr.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3nyrhaoqx.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3xjljqhba.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3lgerswvy.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3mpvohaxv.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3nnmyscnk.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3wrylpnfh.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3cwytcypj.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3gkgimdui.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3lmjsxcsl.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3onbekopp.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3udqzhxpa.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3wafmjauo.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3mwzwexdq.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3bdewwqmh.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3hhyziynr.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3qwrjdfpe.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3ibxnglfu.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3psrxdoqf.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3ccyhlqku.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3gyknzwqb.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3jbkxfxpk.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3syevgrpk.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3zvlmaihn.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3dsrgzbux.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3ijtvrpiq.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3ajeaasob.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3kyqbeuaq.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3jpdgktou.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3kxkxlzzj.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3lqjbyfsv.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3vnvrqkdf.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3ukpcufdz.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3tyfijynr.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3qnpoamcm.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3okpcqypo.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3biovewws.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3pxptmzgo.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3hfgyojbf.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3hynsdabs.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3ameqkdqy.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3rvozyhqw.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3kfouqcek.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3qjofprag.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3gquofbwk.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3ktmioonp.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3jyqydtsy.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3iujygclk.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3urocegzr.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3jruqnbux.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3opkyalgi.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3wrwtnhla.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3zmiqwqwr.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3iqlvqvqf.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3qjxeggon.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3bbmjfbye.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3kwcyrqal.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3baqixgcl.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3equawbaa.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3hxxyxkxu.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3pmidvehh.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3jxlnqptu.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3hzpqtotb.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3hwcncqov.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3laryyxof.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3vmzclakn.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3bpwzqsey.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3rdkrdnti.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3faffsajd.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3fqsbqiam.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3mvysvbsu.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3vlwljlck.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3cqvxwjob.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3xyyaykpc.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3wtpiztxd.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3etdypdaf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rvatztcv.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3wgwpampu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3saeddqej.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3gvtpuaxt.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3ueswyvtj.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3udihxtzj.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3tenoazmb.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3pwbyxsbz.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3guibtugh.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3yvvjquoe.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3zepdwpfa.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3xidpdwri.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3dtlcauqc.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3ctiqmzvy.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3fesfuliu.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3pztqrzck.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3vadnzxup.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3yobjtdxf.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3xirqzzxj.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3kuzbfsoo.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3ttujrcmg.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3bntqgxxt.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3pcxikhdc.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3hxkruisl.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3uctrvkpy.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3xhkrnjku.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3itbcgciv.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3mvfpkwez.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3tuivjbty.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3oaflhats.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3yfvfrhxz.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3cwxbmicp.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3kwiejrwz.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3umypokdp.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3vpxxnhdn.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3dhstbxwx.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3abzdvlrx.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ssnwubyy.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3gybqamex.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3hglnpogc.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3wxyhqqec.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3vbwefotp.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3rlcndtun.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3ndmlbapq.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3fdyyyhgf.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3ijlxngsa.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3txouhngp.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3jisehexc.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3fbkbvxry.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3rlhnzwtv.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3tpnmdsdq.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3vhribsrb.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3dfttidpx.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3xaonmcqm.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3ahbqngsu.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3xlndnaaz.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3hmjmrdbw.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3lsyusybz.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3lbmbksjn.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3vcxvpyul.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3wzjsajem.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3owrrrcwk.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3yjlwfzho.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3gqclrtxe.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3jydyppqm.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3wdwkioru.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3oegyazlu.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3toujfmcl.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3jwwyjqxq.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3miqraoxe.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3wduvnzom.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3ceothjgw.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3mxdqtwif.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3allquvgs.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3oethauep.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3tzgnnezy.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3qqxlrosy.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3lbdicoqg.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3urgpqeyy.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3hughepvp.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3kplcjbpf.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3jrxsjeom.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3aurjppyb.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3aevjnqti.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3ecpfkupb.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3wlnwopwr.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3wvzidadj.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3izgvujxd.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3ywgkdqxu.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3vsqpkzzv.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3siohjiwy.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3qwiqbcyu.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3lssfpxrw.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3hzlakmjf.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3orxetzie.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3dtxtodwu.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3wmjjmizh.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3pgodkfvd.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3zfhdvkbh.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3zayfykrv.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3efvipaxo.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3gtyauaoi.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3ctoxymnp.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3buwohdiw.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3gjtltgjj.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3fvjuavqg.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3lphmkgoi.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3iwtwocha.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3jhsnuawx.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3pybbndth.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3pxegyrlk.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3fjrdqgzl.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3kewiwona.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3kxuggqim.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3yghoaeol.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3xjiaidpq.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3mqqoogat.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3ewolzzhr.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3woiddeso.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3evatllhy.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3ukzfhbjq.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3pzmkxuvy.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3oudemwft.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3tsjtqpnx.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3qdkwfebm.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3zmokyiuj.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3bcmtydsn.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3hnufeoyl.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3nxdyymct.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3wwavibth.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3tpwppsfs.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3agidixob.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3zzijzwwd.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3kfdgsscx.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3bcvmdsco.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3mtjnmfif.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3zwwonbtb.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3pmotljjs.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3nabqddqa.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3cdxhoyuw.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3bgiejuhi.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3izewjoap.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3sdnuikgq.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3godvobol.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3gtrtbvlm.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3dntpeppz.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3lqkdwofm.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3rpgdsxky.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3kcpzahvm.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3wbixwgua.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3xchtcccg.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3rudpkjzi.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3mzpbcrdo.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3jjicejow.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3mboqbbhp.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3gjcptvbd.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3rtgnxsjs.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3ppcbncjq.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3fewwrpyj.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3bwktkgrh.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3wdtltcme.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3gqftvwps.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3ahcmnfzy.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3rhvugblz.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3ilgfxxty.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3oybbmlgy.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3hcgmtnsi.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3ytgikhic.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jbfbptpg.html


<!-- 参考信息 -->