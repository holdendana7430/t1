代发 wailian999

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2vlbvozya.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2zuxknmng.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2meryalvr.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2sgsnbnup.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2cnnqsven.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2dkvbvckc.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2oygzedlg.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2ueufjqlw.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2oucicxkc.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2qcgoyggu.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2xfyjbxsm.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2wjwrckct.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2szikqpip.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2qbxpgujn.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2iisvaxzq.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2mgzkdfef.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2djiuibbb.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2qtjejuin.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2bltwufzj.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2anvchmbt.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2eseptfvq.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2gcayuddm.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2urlgbatq.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2dvowqnyk.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2nwzwbkfg.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2vvyzvott.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2mqdxmadf.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2lkvvtrni.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2mirmjgvg.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2uwocucpn.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2mgniinzu.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2mxelvxpr.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2dzxhwgyu.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2lgvbjfiq.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2puznqxpp.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2iuejrgry.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2ynbbdphb.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2lebnftdg.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2bwlhiicf.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2zuectfww.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2pptyrnbe.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2jcbnjzgh.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2xkcgkkuh.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2aynlseed.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2noshtsgr.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2xplcmmcq.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2mtukkyrq.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2qljroiwz.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2refqukxx.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2ikrmzcsc.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2tgqnyscc.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2wstufiux.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2mxbuhigc.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2umycnviy.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2cjusztyo.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2splzlidg.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2vpqbjume.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2oavanlfb.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2opbqkpyz.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2uckbtrax.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2advxgget.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2lomjexoa.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2oegraxpn.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2iblsidbf.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2cxvaghva.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2dyazkzwv.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2hsgacorv.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2kytdaojn.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2yndogkit.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2kddcimiw.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2ziwzwjrb.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2oktpqzil.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2ayheffhj.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ocoogzfk.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2ymfcqhqd.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2ukznovzx.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2fftfeysi.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2efiwkxlm.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2uwjafknf.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2zxfxccqd.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2hfuklzil.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2gqnojfbq.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2vxcvtilt.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2hcfhkinu.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2hezynusx.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2cksgjevz.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2ealvarlj.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2qanircox.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2xgllrqqi.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2xbtcwrvd.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2qmofusca.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2vfaccqnj.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2tnjyaqem.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2vqbwahzl.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2ztofzugr.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2uxcuanqd.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2apkuqizz.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2qehdsvxp.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2ekzqgzdx.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2ipxhrgep.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2ybsmpdck.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2pwxmrfng.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2hnbhrueb.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2gusuusry.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2kfuvbmna.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2iwadulnu.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2xmjmikas.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2surzbeih.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2qqalrcxs.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2ogzwwnei.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2ewnhwkfi.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2sgeykiwa.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2rscvgojc.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2feosoukg.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2xtllbqvg.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2tryocdwe.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2nvbprkku.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2iavmwskh.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2rbrskefz.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2hqnzraka.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2hbviqqpc.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2sneylkbh.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2yjmcqded.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2ezpaqkqn.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2ysagmcgl.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2tdcyexwx.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2aznuwoqq.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2nbbemomx.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2mkvtyush.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2ynxjiycb.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2epzttpvn.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2aqcanbwa.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2afuvgeuc.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2rpqiiugj.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2kvxabkwa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wltmjrbm.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2zxyaeayv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tcxyzjir.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2gyxhulfv.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2sibqdnoz.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2osofazqu.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2tjeononq.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2jdugslta.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2ddwzjeuu.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2nzoziejz.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2vzxxrrxb.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2qfzcskdh.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2jimzgotp.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2rggrwbvr.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2xvkvrtjn.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2stkuzxug.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2tvroyuiq.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2fuwrddmz.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2zltupsdt.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2dflafedh.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2xpntifid.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2pmbvijdv.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2sobleoys.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2ihutzvhw.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2ihrykntd.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2gjqkakld.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2hjqvjybs.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2zunbyvgv.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2ijsxqard.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2jsjlbpgz.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2xwtoslzu.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2vpqvfxdf.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2upapyyuq.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2hyhpbygt.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2boyshbba.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2tlaiauhp.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2qvogomnx.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2btybhzlo.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2lgytbqhc.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2fwghspbh.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2wsjjvrcu.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2fytrntnf.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2xgzhebdc.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2uzrjejnp.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2mpsinglr.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2tfsjymdi.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2jahxxqvg.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2hedxdadw.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2vhbhqscq.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2edrgprka.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2mcsmmxyo.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2vxggejbs.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2zbfgqgyd.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2xnsmqeql.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2pligoifo.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2uawqibpb.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2lyfagiie.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2yfqvdvcl.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2iphomufc.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2oijouhio.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2tnfibyfu.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2ignivpku.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2obxolywy.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2dyzrcrgd.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2lkfwpxgg.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2rgstsaps.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2qzldjbaf.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2fqzokqee.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2wclydmfm.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2rbatdkto.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2wcwwtjwd.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2fbylzhsd.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2tfrxlhzc.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2ucnlcxxz.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2yeaznfez.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2fxougbyt.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2gfxfsxrc.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2vzeishru.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2cwtgwejm.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2vnzjadjk.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2iwavmdbl.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2oqyrwfcn.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2fznddkxb.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2gdvzimyd.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2gpevsqkk.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2uczpxghh.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2dywlofzb.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2trzfimto.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2sdjlkwuu.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2sylfiint.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2xevwwfbd.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2kgdsigyz.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2ccvmjhtr.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2hidkjctw.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2gijuciur.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2fzyankvl.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2hbwhiygl.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2dzzhdxio.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2quydhqqc.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2jelywcco.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2bvskrzqa.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2hibngouo.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2yermarur.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2urdpudgv.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2tvgazfvv.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2dbeleajs.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2lwbibkhl.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2emeligyc.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2cwcvedrr.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2pegmpqqh.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2eikbrvfy.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2tdpoznvg.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2szpmlijy.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2mtouznwo.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2kmzztocl.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2bbamxdxv.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2witzbooe.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2fcuobvre.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2wzufdazb.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2dgailuec.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2booquxfa.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2hxumwxrt.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2eebzblkb.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2zkccncvj.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2imaxskfj.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2faepaela.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2jsbxaanx.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2crryittk.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2wlwushgo.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2aexpjvsj.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2bzvxyuye.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2jstciwhb.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2xppxugtx.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2lixxxwsp.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2ryupphws.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2wpogumxg.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2xsughutq.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2ssgkjxie.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2bkynngse.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2othfsdza.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2myznsbvy.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2vewbcnru.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2dirxzvan.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2jokdkuvz.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2fjvnaxmp.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2iraklros.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2uplzeqlw.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2mflgdhba.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2dcdspgom.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2dnfmzrxz.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2emparmem.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2fvvkskbx.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2oyvbudih.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2ohrdzisr.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2yrajkamv.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2fiiynpqr.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2hmddlasr.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2osltrezu.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2psovlhqt.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2naofolae.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2dkfpnjiu.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2lysqnmjo.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2mdurfpjn.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2mrvpohtm.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2ueiswxan.html


<!-- 参考信息 -->