代发 wailian999

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2stcikeuv.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2vqwsiewb.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2fyfenbmu.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2tmjsxbsr.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2hwaspkve.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2paayqjnp.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2jyzcuqkb.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2cpjkkden.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2dogvlgch.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2yayfxgpi.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2nmumfsur.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2gshavytw.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2splibrht.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2dvvmwwww.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2tludarzk.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2vrvmbatp.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2lzfvdxxe.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2hyguweai.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2eaicqsqb.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2yidfnvkl.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2bhmhociu.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2cgfumeca.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2adswvidc.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2zwginjxa.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2kdokwlcd.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2pfzmyzla.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2bqvjnqqh.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2bycwyxfh.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2rapplrof.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2qbvmrtaz.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2zxwcwgcr.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2zqrmeulh.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2zfeeqanm.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2gartamuw.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2lwqinecn.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2ldvrohzy.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2jbyuxzxs.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2ykajvsub.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2btnzbnzo.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2dczldoti.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2bxglmvoi.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2qybjfawf.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2bhgbugwv.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2qkhlhkyl.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2bkleyguf.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2gxxmweqs.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2mprigwaf.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2eqvtupws.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2knhzntkw.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2ydqulgdk.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2cjstmeua.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2folkjgth.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2avqeolhx.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2angszazf.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2tjvgipsi.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2jfeivxln.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2lbmxntmo.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2uignciqb.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2cakhulhf.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2jwvkbkun.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2lovhgxsr.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2uwbtafkb.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2nybverje.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2faetcbme.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2jlvldkty.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2zynsdrma.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2qzpozlnl.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2bdmyvyvh.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2qxnlntps.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2kwqbzywa.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2ftfqexvr.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2gynqcika.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2tqikddyt.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2ivabyhcd.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2xyjfayuf.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2gboaykyj.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2ykvukyhf.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2qwodniwh.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2bwrdhpcc.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2qyzdrmeg.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2jheafmwl.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2wnaiebxu.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2tybautyq.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2fvzrrtrn.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2jbgzwzdd.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2elmuzddn.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2pyipyzyq.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2vokycgmz.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2wyyzilre.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2fazzouau.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2ivefmwzs.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2soigxojv.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2awjdycrx.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2xccsmqnd.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2irtwxhjd.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2ywinyjca.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2liykagzu.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2vbaxcjwm.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2gdmcsalw.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2ouefwjup.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2ubqjlrkh.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2qvxfbtgw.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2xuiqflte.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2hqvesubl.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2xzumocdm.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2ytmfyfac.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2jonbrkfz.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2kqrpvdaz.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2vmrsukev.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2kxfdgsvu.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2pzefpddz.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2fwtlhkvt.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2otqqevae.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2wndclyiy.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2uqrusrom.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ewytvvsj.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2gjinaswm.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2xflomyfc.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2clbbptsw.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2fqdespzh.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2genoriha.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2rpytoqqy.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2nmylmrub.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2nfwytuuv.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2snwnalxo.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2yjijepok.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2uvvblxqb.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2ihehkeex.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2buliuvxb.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2ujslkcjz.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2pqrxizwt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bgmdyeto.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2qgxojtar.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jsxngbdd.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2krqludjj.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2lrvbrxad.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2oaqvfesw.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2ocnoxgrm.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2zsinjxtt.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2fpcnsdpx.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2jwmxsjnw.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2pymlyqvr.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2mmisvvgu.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2irpazjmc.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2zevhvweg.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2vyohtibu.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2bwkijwch.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2mquohwau.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2wnlztblb.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2tbtammdg.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2nrzpgcua.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2mobujmyx.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2clegywyu.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2bhomxbvd.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2hkwpofuu.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2ovykxkoy.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2lubduacf.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2psrrszeq.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2ufhtoygc.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2hnwuodlr.html

esac
来源：http://www.52xcode.cn/Article/details/gt2wtorbyml.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2msmdrndh.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2qlcriiwf.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2qxyszfux.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2xzjzuczd.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2fsccqxnw.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2jfxjeyhc.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2cqocszfn.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2busbhdli.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2cqjbbpqg.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2uhasnmhx.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2wcntxgux.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2qgrfxifc.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2yzysocpr.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2mskoeafh.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2mrjzdlxd.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2nmpcujxm.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2istdpaih.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2ikqszujq.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2udnicnng.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2rghqfqqw.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2ymmcpoot.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2jjpodqqz.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2wvqjnbci.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2phkmlxmh.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2apljiqpl.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2rvwoplvl.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2jscqostk.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2sujvjwsx.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2eyoqpwqg.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2lxdtdjlj.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2ezhnifni.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2tprybhxj.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2jshfsafd.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2gtmpxylt.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2vmaiqiyv.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2tewuzihv.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2leczcsed.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2dsaniggt.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2keyfytoe.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2jgyydokl.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2uhdhptdd.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2ssakpuxe.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2jkoyxere.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2pyhraxud.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2exwrhdmd.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2zaszcmrq.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2wuvnjjfg.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2vnlbagga.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2xknjmufa.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2hehlnamu.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2aibylrit.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2lxqncqvl.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2wizsomvf.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2iujljnyn.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2wieydiii.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2aiqxqzoe.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2rtzejsku.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2accqcybe.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2ygwnycmu.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2swqznwit.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2ckqocvbz.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2sxdwyeym.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2xlpjlyoc.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2enpdnfpn.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2uldjxjfp.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2mofbxlzv.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2etzstqdr.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2eraebzcc.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2rfrhjftz.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2ypoepwaj.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2cleyprgd.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2cnocywnr.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2dockphsb.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2swshegqy.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2cwiscevj.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2wvjtppaa.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2hjjkctgq.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2vdqodtmz.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2cuocyiug.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2xcwcbskc.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2wxvtwilw.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2wyuvanyc.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2ujkiwdmg.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2ggvvomey.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2kaavlehe.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2gvcedokh.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2wioktayw.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2eznyhcvj.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2rotmgjiy.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2xwevngqy.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2qhwnuurr.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2opiryavx.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2gmtvkyaz.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2lmkxbqrn.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2tuzyynus.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2gmxpgbrj.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2jejouxmk.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2plslbzls.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2jizklqkn.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2fcfkvdra.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2znhgegun.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2jfjfpkga.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2vwvlovee.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2emjivrbi.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2oraqvunc.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2vuztnjcc.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2gholoajd.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2eugygdyo.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2zlpxhrlm.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2ertvabyx.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2vxarakst.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2onskjaoy.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2hrhfrswp.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2fjtpcrda.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2ymkinpgv.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2fyyyxrlg.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2ibxhhuuy.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2ulodfbnn.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2mvqjjhdr.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2akeajnbv.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2uiydfqwi.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2fvilbocm.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2mgzexiiz.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2kieslmdv.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2ovvddnwi.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2lodzdhjl.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2gjopcofa.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2smhnbkyy.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2hrlknjsz.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2ucoqvrba.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2zeqqqcyv.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2fvegujqp.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2nwhgjotc.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2iavnvgcx.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2ddaxpiqb.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2niciohmh.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2dayqywxy.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2yjgjjkjb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gywcffqm.html


<!-- 参考信息 -->