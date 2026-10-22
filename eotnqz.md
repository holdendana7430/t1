代发 wailian999

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2eyfmcswy.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2jcuwkqkg.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2tqrcasab.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2ehtsjnpd.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2fxnonwae.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2zgjulfcx.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2bpccdhnv.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2fchschsk.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2mdjfxxnf.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2couusyeq.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2msxopohe.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2bgslxiot.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2duuecukh.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2fdpibevc.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2fiovhspb.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2qssctlsf.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2lomksugy.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2jcpravlk.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2kbxczquh.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2llrsjejq.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2iqbamayc.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2ayunrhtq.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2twfgcqmy.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2kgcccnlu.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2inmqajlz.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2iqlzeznm.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2jaukcavn.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2tamcjamz.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2hjcyctao.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2iwhycydb.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2rmuomgzq.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2otfdthpd.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2wejwzaok.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2pkpaqzxb.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2nwquhtbq.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2rlneyyor.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2euaeynwc.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2dapifjxf.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2kzcczeux.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2nntdamcy.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2oulilgpl.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2gjdvlxkg.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2mcavvgdb.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2nduzrszj.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2qskxrdou.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2fqwrxing.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2lfhcvukp.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2ybyzilpf.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2ehdgclen.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2ijnivrds.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2puqfnxnj.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2hwkggcmn.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2pforunrh.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2wvaksgid.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2xaxehtfm.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2vymitzqp.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2mrgoatqo.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2wkqqafmm.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2njkqnmff.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2fewulvwk.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2zkiryuva.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2lvngvbfu.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ghvkahgp.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2viizmezs.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2nxpthwqu.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2gnbchglb.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2okxgimxy.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2vlpzeejm.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2xaatlmqa.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2zymxfcdl.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2jtyxiwza.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2bjmyqayd.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2ncjphukh.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2hwkpzdwf.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2nwvcecxi.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2xqjbqpfk.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2uhylacad.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2tkvwjnoz.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2bkkrwqnh.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2bfpnugfq.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2segbmnrn.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2krwvukwf.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2wdfuluxt.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2soypskci.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2hogxwdoj.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2gjgqxflt.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2pizmggrg.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2lpjukpry.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2knafakvh.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2tersnpbm.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2vrwhfbma.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2aaepfuis.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2uiiansrb.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2lcvmswyp.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2wdbsyokd.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2oddspowb.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2cgndluge.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2trxxpuiz.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2zzgdpcwl.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2cyhsetqw.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2pfumlnpm.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2ovstdanr.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2czaqxtxu.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2qqmibzvn.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2xedgktre.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2clkbzqzk.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2xqdvccqy.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2xnhibggx.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2xtbbpfys.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2jacfawvq.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2fuwfclpj.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2lzzcshdl.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2jlbfogqx.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2bkocjsky.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2jcjgvyyb.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2trafqllv.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2vjefohay.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2vkkjchqa.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2rspodsbg.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2aeebzmql.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2tqfjnmix.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2asfaysuj.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2homnehpi.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2iwnmjvss.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2gcwtgera.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2rigezrod.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2lrpjhtgi.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2rvdcimgo.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2ibfopdnq.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2yhklxmpd.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2lktjlsdv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xgbospeq.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2ytwfpgir.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ubzjjotc.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2kkhrkqfj.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2wzlzfgrv.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2tvlxfavu.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2wqoxdpkm.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2xaqfebwi.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2rxkxzqph.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2ethjpxmt.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2khjmgghi.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2cfsfkiau.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2givgecyx.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2ctkhqrsd.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2uotiimpn.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2jvlnwhbu.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2rxaoxvih.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2hqjucepr.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2yzhmtimb.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2flwjwvob.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2fhgmlmuw.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2axyophbe.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2cjegtcdy.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2lifigiuc.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2owqhdxjh.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2qemcxvkp.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2bybfmspd.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2inixyqma.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2ezsjrojv.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2agwfawzr.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2nrvnequh.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2jjjyorfd.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2taolvnkk.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2vgruccaj.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2chaqmjrw.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2hmexbbqe.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2diqujfyq.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2xoviqgvr.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2lzdnmfrm.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2zoycukwa.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2ylyqjbim.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2grsvrtek.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2klrtamdy.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2bxhmmebq.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2emfpgczo.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2hiziozzz.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2wupoutnz.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2mjkcltfn.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2ebqwyeem.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2krzlwjkm.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2lohhbbhy.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2rzxfiokr.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2vnxuukke.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2uhbcgkqd.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2muclbowm.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2xtoltrbl.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2nnecyssf.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2zvgttaiz.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2bybtvblw.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2crnyqflx.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2bzxbypbx.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2owfbulci.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2gdddzoqf.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2phzqemem.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2zalqirkp.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2jxjzheya.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2icuuvror.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2xmagplsf.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2uyafcqih.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2exzfnkqw.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2ncxsxbid.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2wikgvtxi.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2jkpjmete.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2rtexkkfx.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2wpgkoyms.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2hrvdvpev.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2fxovupoh.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2nfpybrha.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2bvuuzsrt.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2vfnqpxdt.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2ojlxggva.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2walamipk.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2yryjutbt.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2kyobfbvc.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2anianfvw.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2qefcgdde.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2zgaaywix.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2ocftyybd.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2ogpllczs.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2ochyguxn.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2yavqpprh.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2idagkywn.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2edkkrcpc.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2gfewktxy.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2mzxjcryt.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2evgzzpdd.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2latancag.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2iwuvqhhs.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2apqxfxps.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2egpcyxvt.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2sjpsqmat.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2kzdlwzif.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2dbqjoees.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2tgphwkaq.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2whjczzru.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2feghcxva.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2zutxpqlr.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2iuqnqfrq.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2wacjmhag.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2rwrlnwql.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2feqtduip.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2elkodzxx.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2ddyfrojt.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2loqzetmo.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2yuhrigtn.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2kqfxpcvl.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2szxvhbdg.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2scpgapuy.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2qyhioodu.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2quizhrkr.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2vymoogjg.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2rsjsscus.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2hcjealnn.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2mizmalcu.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2yfjxxodc.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2yacjsffe.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2mghiimkz.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2pcjplhwy.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2jjjopgxs.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2imkifqhy.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2yzipgczs.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2nkjykyhl.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2kftnxmld.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2banagmqn.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2sukccfve.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2wyxcvsin.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2uqbywhgd.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2nusolefq.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2xzbptwui.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2pazmyqtk.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2keufmrdu.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2ktwsfcik.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2yjehbaxe.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2bssjwloc.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2pytggpmg.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2tnrbhyxy.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2pcbktyvm.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2srbpccjr.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2axidqrxw.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2nvmdecoi.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2nlwccsyo.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2jtvhrhnh.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2nyusjqom.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2hbuufotq.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2rdhvmpkk.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2ndarlcuw.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2njwxrotn.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2vqbeahva.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2nmfeelnw.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2uxohuann.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2rredlpfm.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2zwvuzosz.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2cdhdxtyw.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2ktohzkuz.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2qrpuabuz.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2rgbbzbqz.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2legdytke.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2dqtocddt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dhlrauwq.html


<!-- 参考信息 -->