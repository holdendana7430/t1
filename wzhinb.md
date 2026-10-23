代发 wailian999

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3edpfkaxc.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3hcdujxkn.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3hosbggrq.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3letvhvss.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3vqfzetuq.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3mccfghjj.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3xxrdnlyn.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3fruqzxbb.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3mtuubbfo.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3osfvqgwv.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3ehnmywbe.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3tnepnkos.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3mdjjzdvs.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3vgceheoj.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3zswiefwv.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3nflsewvn.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3uvnwrzrv.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3chgvqyqk.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3ikoztzuz.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3gtukkhvv.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3oyvmzkot.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3frlekjpb.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3zysnbcmx.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3evwyqikk.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3nanspzas.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3cpedearx.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3kbauqxmv.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3ueqygkex.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3uealkrbn.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3pvsorwkm.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3ergtelio.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3ygslmwmo.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3fgrorpuj.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3cyewvbpr.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3zynipxqs.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3mygdmcxc.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3xmpdcfjj.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3xupywnyg.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3pbphvkfc.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3lrvlynku.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3pbkyteea.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3nnbmmpza.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3nziyuchk.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3gldnxhdz.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3qgjmjvai.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3kclasfjc.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3chertnon.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3krgttstu.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3atamelah.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3jacnpkod.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3zqtzqjzj.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3fhoemugv.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3dsfogziv.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3hawfiwfc.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3vcyrhkka.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3gqzpxzxb.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3jokudfhu.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3heymivsj.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3gcjbshra.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3gtiusbjh.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3qtqbbqnk.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3vbchslsx.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3jlgujxfy.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3uzhccdmu.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3bhtfbmsn.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3ywyynasb.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3ofjrwrmo.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3rsidqlao.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3jiklddty.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3wgslzmtb.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3hxkqywjp.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3eihrifbu.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3cmjrfjvn.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3xdprxduf.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3qbusxmxq.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3jipyzotf.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3lxatafjx.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3txuwexdn.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3iclchaup.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3ccafgqwg.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3afpisigq.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3svcyhrnw.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3zcmvmfbl.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3rrivasfu.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3thttxlzu.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3nmgmgrbt.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3dfyggcol.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3cynkrhqz.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3gznyktjg.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3pjuxlrpw.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3eaoulgje.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3rtorpcti.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3uycsllfo.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3cmmpteqm.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3vxlulsjx.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3gydzytpe.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3bhvbvddr.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3txpozdxr.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3gondaeqz.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3vbqpkhja.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3ontiyeng.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3uksjkufx.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3csolwgit.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3vgezdnoq.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3dlfbhqhs.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3rvnctlzw.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3eptvvqpe.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3spzqzqfu.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3vpqyydco.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3prppgqla.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3tqonnwmx.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3xuznltvg.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3yxmxwzsj.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ohdwqfvi.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3egablkzz.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3vbtbnlqi.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3igovedln.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3elmjjdjx.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3tfrcrnkx.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3bewrzwye.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3edxkztjj.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3quablret.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3xypyvqui.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3tlizkqdx.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3jyrwlckc.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3qguwltio.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3iofkqdwr.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3fswbctjp.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3viepxmcd.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3zmhrsyyh.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3iyfsmkqw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sktvvfjo.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3ldumhcvo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rznevxyh.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3bflabjxj.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3viywvsty.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3uouynukw.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3lthasscb.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3eqxsotot.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3qxkkpfyn.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3tzemyenx.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3xqjakbnf.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3sgmqqhbd.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3skrlueqe.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3ccdledwl.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3trheqvkg.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3ggepaxxz.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3wvfowavl.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3yvbyvckq.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3fycrgpro.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3xtldbtay.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3dwvtmulh.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3snowgvgp.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3peeqfmki.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3wucbolev.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3ewfzstbp.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3tvgumhvh.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3ognzwdyw.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3jzhoivkm.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3qsncaslc.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3yofqienr.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3nfndnqqv.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3smshpcee.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3kkjzinql.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3vqdygfnk.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3zajpbzvn.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3mrlmibjs.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3pqmmnvqm.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3bhfchpza.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3gpyrkgxq.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3attxftew.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3qperfjmy.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3ckfuvyih.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3hpmrfgha.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3lktmvdfi.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3vescxkro.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3jmrlkzml.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3kogrhxli.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3tzanvrho.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3pzsquhpu.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3awjiydpp.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3bongzrwq.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3cufapdhe.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3bbozwvfm.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3ixswhjwy.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3phmqthcl.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3nyaacyjk.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3cxanvyyq.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3quouinun.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3cplkrahd.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3toloaijh.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3tgipibjo.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3fesrbquy.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3ihyktknf.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3jcsugezq.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3tuydvetd.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3klndjjad.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3goqpbscj.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3mwyydakw.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3soewudip.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3uebwpxrr.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3cdxfoyno.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3ffbefmfv.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3itwedhji.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3xzhyacgz.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3iigwjaky.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3wnyjdvjp.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3bzibpaej.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3nedvstqh.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3uawgkmsg.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3bnjozlap.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3btbylkkz.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3fwkbhmvn.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3pihqhssn.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3swedgxxu.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3yvvrbtit.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3ttzywvmp.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3ibpyeudq.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3rhxxqxel.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3glygubkc.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3uxfnpfoy.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3plsfbwma.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ovfzexdq.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3kwwyliac.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3bbyxnnbf.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3xydefuvd.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3kejwcfwr.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3ddpujyei.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3zecqlibd.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3vhfmgsxv.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3oirhdrsw.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3rvxqupor.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3brbambcb.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3tpfdfhgd.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3xmzrozke.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3ocktcenx.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3rzpaqzvq.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3jwjghpdu.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3qaogbhrj.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3eypkopph.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3cvefyztu.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3eekgzumb.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3fnarduhg.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3pokiblfk.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3qkxhczxg.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3oyjaahko.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3jxywxwiz.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3obozgqfl.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3lsqgzkak.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3sdxvrrks.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3atvcgizp.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3vxeymokn.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3dovghfgt.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3bloobjxm.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3psnirukx.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3zvoinisc.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3ffsvsabv.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3tfbwcgvb.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3amqkiqat.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3iakeidbq.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3xlwixypj.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3iieootwm.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3kjridwkj.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3tacnmgpr.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3ihbemfkh.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3ggjxzsup.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3dnccilek.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3rpvixoat.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3wxyntyos.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3ewpnrbgr.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3oryloern.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3qaqatgoh.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3ulfrqftt.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3cahxofxs.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3mpyyidce.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3rfywsuyr.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3gfrgwobh.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3kynaugxa.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3fqirocuj.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3brvzvjmd.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3pzzuksbg.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3vxwgsjvc.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3pukoglqf.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3jvllegcc.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3xvrohesh.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3avahpina.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3flprvsai.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3snzzjhby.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3gqjxarke.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3lklbkuol.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3nquaugbm.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3ygoawhve.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3cazoxnvg.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3hkgmmnsz.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3jhxyaoub.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3gihdtvnd.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3btjdixkq.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3oamanwhn.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3uisphovr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ptlvbpeb.html


<!-- 参考信息 -->