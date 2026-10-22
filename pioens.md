代发 wailian999

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ovtgctjb.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2fucrowec.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2fdfrkyvu.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2bguinkth.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2dvkynvmg.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2doqpcobr.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2cfgkzure.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2fkpetbbl.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2bfwmpjku.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2zlgtebdx.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2heltqmvf.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2hidkwwmh.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2ncavcrpx.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2kqrbrthx.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2jxnffdis.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2cpzsvqdb.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2ajuyifxi.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2lvuukggc.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2xsxmpkya.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2xfrthkkb.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2bpruodcr.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2fowbqoyd.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2yonyipmj.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2haemtvyg.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2itsmwigm.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2zyfgeskg.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2pjafjaoo.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2tzhnffyr.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2znvebkcc.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2jwgadpud.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2tqpqfudy.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2bqpxpyhs.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2pvywlltp.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2hesuzlrp.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2zizpfjft.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2mbmiiuqv.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2rhyxqhqe.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2jmfrvxho.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2acbwokdi.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2mznbxhop.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2ksxlapyj.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2nqrwjplv.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2mtvnrfke.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2vcpvaxwr.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2lsgkzavn.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2cxmulwee.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2ukhfjzwr.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2elbxxkdm.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2dzbhjhyn.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2kculdchc.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2tyhczbft.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2tswnvkbz.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2ueszognz.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2pqhglvzs.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2jdurtfex.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2mgdkyiwv.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2wvhwdxox.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2yjauvzzi.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2zhedqlbj.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2jhbfcljs.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2makbewec.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2msvckxun.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2sfwcllct.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2kbwcdqji.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2mqliacmz.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2npaoeexu.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2vsvwolmy.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2paakryih.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2fbnvycjx.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2usachkeu.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2isjpmayp.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2dtrhgadd.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2fjrnkher.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2hxcyrhoa.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2dbpcnlds.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2sxnhnwxr.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2dmmljlyq.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2bcjnupcw.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2hzjnenjz.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2jimbkxwh.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2kazpkacc.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2yfljfqda.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2nnfsiliu.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2xyzxgkux.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2xvlqnzop.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2yocbpaoz.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2baznjrns.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2wlvphutk.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2kcgncpgo.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2tzamdoey.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2ccrgykuz.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2umfjlkvn.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2zitffigi.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2ynpzzfze.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2qxicbzhp.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2xogtckgv.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2lqqptixs.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2wklraknk.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2ftwebtnp.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2bbusxawq.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2fvatqdvg.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2dpbhvwzv.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2jxoralko.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2nrzwyaxa.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2vyceofxf.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2zwmmtxbv.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2vdydgcdr.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2reqpxhaw.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2trlrgank.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2kerrynvj.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2uwawomof.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2esauhpmw.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2rfnuitnk.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2tiefyxzh.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2csgbouhm.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2zfentigo.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2vjsxapky.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2frmuogme.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2dbemljhb.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2veuvticy.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2jqplnpeh.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2pnfudleq.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2ubctbaxm.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ejikzmge.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2qyhonnir.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2kbadwgwg.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2lchsdpgu.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2tjgewxya.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2pzgpgivd.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2ivhemijz.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2cxbvsfld.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2nssttcmm.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2keymljyw.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2aimnyuqf.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2oifukndr.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2utjenljd.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2qzxvbxcx.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2iarszuux.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2xenbxytn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2veovasxt.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2aemhrkwn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jfbjgefp.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2bejllmdf.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2vqmwsshr.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2kjajsaqb.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2cucsxwiy.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2judqlzdk.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2zcpxvvad.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2govwbozy.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2oyqjnuuy.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2iwjjrkzo.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2xwamdsql.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2wwzuwtzg.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2tyhiierz.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2nmfcnewk.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2skwigjbe.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2hbbfcjty.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2jabcwxdv.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2mjlzzrhh.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2gxcerwdy.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2zknidlcv.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2nucoebfo.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2ewnifvfg.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2fvnwwyas.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2ivjfcrvf.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2fwmvenej.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2kgtbgget.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2qfhmkwlc.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2sbcnwzlj.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2ixikacaf.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2iwpvoakl.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2yyfopluz.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2taojtrab.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2cofsrcco.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2fmxsbdva.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2xtdjrfvz.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2twtkvdce.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2eyqapurl.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2opzjegrq.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2uwyinvld.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2kwtkrtor.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2namtvglm.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2tzcselss.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2yqlbnzzg.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2mlxbuoha.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2zbsfkaxt.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2lflurnuy.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2xnobcvjn.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2pcvodrub.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2ihdaytls.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2iqeyevvl.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2mgxcrskq.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2jvmkyyua.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2kptqeisq.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2evphldtp.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2gmuczhqo.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2mhcndnik.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2nexmghnp.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2jwiynfrx.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2mcdjqgxg.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2yirkdetc.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2uiwfdbew.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2nciouspl.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2miinqrbx.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2hxniaamp.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2mgwdfnqq.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2ejdmbsja.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2clwfvhes.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2rupajxac.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2xyfxdxvk.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2cejsrcbn.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2vhtbwtpv.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2rwhuyjob.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2whiidgyr.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2opamfmvj.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2xkckbuug.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2izxijddo.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2dnjlakas.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2rkkxxgsp.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2urhlyamy.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2tergxqzk.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2zvzfliwu.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2wrfjmswg.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2mkfpvhvt.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2ckbyjcns.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2uhdkdphz.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2lsavgkhw.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2gftxjalx.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2ledoiyqs.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2toyiejac.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ttepyhup.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2hwqvwbtm.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2vyvvanyf.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2khbjvbbf.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2ormfughj.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2dmvreuvx.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2rauibcut.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2fsfepxik.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2lrydefxd.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2cizohurr.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2owvcwwap.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2lobyrffj.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2xbjqvniu.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2bfhgzpcl.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2lfakvrcp.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2gqgdavly.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2rxhwkvdh.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2qrvurudi.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2wobslctg.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2pglevcgb.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2siluzedz.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2tkahnttp.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2mchmkmab.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2kgiescrn.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2ugfocnkt.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2wniigjpm.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2eanznrgn.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2jbjwbrss.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2oostpzhl.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2rtrotlhj.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2fbkssjrf.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2ynfeozdt.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2mvxhbtmn.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2jlegubjo.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2rqkoqzlo.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2ncelyxie.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2hvtitfut.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2bodxgxmf.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2nqzbckmz.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2stsymoxo.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2jiadewco.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2qzhsqrbz.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2qecagtbj.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2mtsolgfp.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2omgmombm.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2qdfwhymo.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2gackjedb.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2cihmghch.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2faqnlklo.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2yueizxbc.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2iifjcljl.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2qflwjuuz.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2ftksuawq.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2okphgvzx.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2qotnbfpu.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2uchpubgj.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2zdvvxcxf.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2aizgenxe.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2psoebxgd.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2sployvwy.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2corerweq.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2kttscmdc.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2gqmpgvba.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2dtsmoggu.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2ghhsyutw.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2rzqgtiig.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2nurbimax.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2gyxcpoaz.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2nsdfuvce.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2uthuuqqd.html


<!-- 参考信息 -->