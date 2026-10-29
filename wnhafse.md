代发 wailian999

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.blog.fehbvm.com/Article/details/gqffgzdaa.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.hesvh.cn/Article/details/gaacfsfrf.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wap.hesvh.cn/Article/details/gkjrnswqn.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mobile.hesvh.cn/Article/details/gxkeolzpx.sHtML

[Q33] 多列分组
来源：http://baike.fehbvm.com/Article/details/gwhieuudm.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wap.fehbvm.com/Article/details/gegwzzjwy.sHtML

[Q34] 每组取第一条
来源：http://m.share.hesvh.cn/Article/details/gdtdlgvxx.sHtML

SELECT * FROM (
来源：http://mobile.zdbjq.cn/Article/details/gguoyhkos.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.share.fehbvm.com/Article/details/gidwzhbhv.sHtML

) t WHERE rn = 1;
来源：http://3g.zdbjq.cn/Article/details/gnakmgwcy.sHtML

[Q35] 内连接
来源：http://blog.fehbvm.com/Article/details/gktupybec.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://3g.hesvh.cn/Article/details/gvxdbrfyq.sHtML

[Q36] 左连接
来源：http://m.share.fehbvm.com/Article/details/grzqujhql.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://read.share.zdbjq.cn/Article/details/gnlwhgoqy.sHtML

[Q37] 右连接
来源：http://blog.hesvh.cn/Article/details/gkafqiohk.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.m.share.zdbjq.cn/Article/details/gjzwbqyvb.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.zdbjq.cn/Article/details/gigefifdr.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mobile.zdbjq.cn/Article/details/gxrfuccgg.sHtML

[Q39] 自连接（查上下级）
来源：http://mobile.zdbjq.cn/Article/details/ghrnflqax.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.fehbvm.com/Article/details/grxsaoiwx.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.zdbjq.cn/Article/details/gaubiqavu.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.hesvh.cn/Article/details/goabpjkup.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.zdbjq.cn/Article/details/gkxxgjcsc.sHtML

[Q41] 多表连接
来源：http://blog.zdbjq.cn/Article/details/gjdspibzd.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://read.share.hesvh.cn/Article/details/gfexhyvtl.sHtML

JOIN users u ON u.id = o.user_id
来源：http://blog.zdbjq.cn/Article/details/gmkefwifc.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.m.share.fehbvm.com/Article/details/gsptuflcg.sHtML

[Q42] 连接条件附加过滤
来源：http://wap.hesvh.cn/Article/details/gfvlxlarj.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.share.fehbvm.com/Article/details/gjkovhbgg.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://m.share.zdbjq.cn/Article/details/gkylnzpke.sHtML

[Q43] 标量子查询
来源：http://blog.hesvh.cn/Article/details/gubpdelhl.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wap.hesvh.cn/Article/details/gaqxglfeo.sHtML

[Q44] IN 子查询
来源：http://www.m.share.hesvh.cn/Article/details/gjecylodz.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wap.hesvh.cn/Article/details/gqytrvfxy.sHtML

[Q45] EXISTS 判断存在
来源：http://read.share.hesvh.cn/Article/details/gcnjytjee.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.hesvh.cn/Article/details/gwhgloitz.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.hesvh.cn/Article/details/gjtgxleqe.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.hesvh.cn/Article/details/gibsihzmu.sHtML

[Q47] 与平均值比较
来源：http://mobile.hesvh.cn/Article/details/gbjzcbkjd.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://m.share.fehbvm.com/Article/details/ghlotxfty.sHtML

[Q48] CTE 公用表表达式
来源：http://3g.zdbjq.cn/Article/details/gwnfxgspx.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.share.zdbjq.cn/Article/details/gdliedduv.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.blog.zdbjq.cn/Article/details/gpodskpoq.sHtML

[Q49] 更新单行
来源：http://www.share.hesvh.cn/Article/details/gwmjkdvqh.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.blog.hesvh.cn/Article/details/gyeldnfda.sHtML

[Q50] 批量更新
来源：http://wap.hesvh.cn/Article/details/ghgsvkxxp.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://m.share.fehbvm.com/Article/details/gevgidwpb.sHtML

[Q51] 用子查询更新
来源：http://baike.fehbvm.com/Article/details/gszwyxkga.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://3g.zdbjq.cn/Article/details/givxoxudm.sHtML

[Q52] 删除指定行
来源：http://3g.hesvh.cn/Article/details/gbvkkxhlf.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.m.share.zdbjq.cn/Article/details/ggjspeixf.sHtML

[Q53] 按条件删除
来源：http://mobile.hesvh.cn/Article/details/gesgualyg.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.share.fehbvm.com/Article/details/ggocfjxij.sHtML

[Q54] 清空表
来源：http://www.share.hesvh.cn/Article/details/gusljkbdr.sHtML

TRUNCATE TABLE logs;
来源：http://baike.zdbjq.cn/Article/details/gltodymfz.sHtML

[Q55] 排名（并列占位）
来源：http://baike.hesvh.cn/Article/details/globrlcjg.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.blog.zdbjq.cn/Article/details/gglydzmef.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.hesvh.cn/Article/details/gdbooqsgu.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.zdbjq.cn/Article/details/gjcpbilcw.sHtML

[Q57] 行号
来源：http://www.m.share.hesvh.cn/Article/details/gmonthfqs.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gresuifzz.sHtML

[Q58] 累计求和
来源：http://3g.zdbjq.cn/Article/details/ggsjmtdeq.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.zdbjq.cn/Article/details/gmsfgnmtb.sHtML

[Q59] 分组内累计
来源：http://www.blog.hesvh.cn/Article/details/gvwbumszc.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://read.share.fehbvm.com/Article/details/gizdpokeu.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.zdbjq.cn/Article/details/gjcbheimk.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.m.share.fehbvm.com/Article/details/gzudemsbf.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.hesvh.cn/Article/details/geilmdojt.sHtML

[Q61] 移动平均
来源：http://m.share.hesvh.cn/Article/details/guwfbbwig.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://blog.zdbjq.cn/Article/details/gvyaegjkc.sHtML

[Q62] 分组占比
来源：http://www.blog.zdbjq.cn/Article/details/gwvahsaid.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://baike.fehbvm.com/Article/details/gplqvqfwp.sHtML

[Q63] 开启事务
来源：http://3g.zdbjq.cn/Article/details/guqetbwsp.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://wap.zdbjq.cn/Article/details/gnaxxrtjm.sHtML

[Q64] 提交事务
来源：http://3g.zdbjq.cn/Article/details/gzcgrnnoh.sHtML

COMMIT;
来源：http://mobile.zdbjq.cn/Article/details/gxmuqrlev.sHtML

[Q65] 回滚事务
来源：http://baike.fehbvm.com/Article/details/gbwsumuwj.sHtML

ROLLBACK;
来源：http://3g.fehbvm.com/Article/details/gazqymtln.sHtML

[Q66] 行锁查询
来源：http://www.blog.fehbvm.com/Article/details/gslutvhwu.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://baike.fehbvm.com/Article/details/gcxnxngop.sHtML

[Q67] 设置隔离级别
来源：http://wap.hesvh.cn/Article/details/gmtecjluk.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://3g.zdbjq.cn/Article/details/gbccbbnrj.sHtML

[Q68] 保存点
来源：http://wap.zdbjq.cn/Article/details/gixbyjipm.sHtML

SAVEPOINT sp1;
来源：http://read.share.fehbvm.com/Article/details/ggwlphhur.sHtML

ROLLBACK TO sp1;
来源：http://wap.zdbjq.cn/Article/details/gevurfaxc.sHtML

[Q69] 查看执行计划
来源：http://3g.fehbvm.com/Article/details/gumafvheg.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://m.share.fehbvm.com/Article/details/gyfoedoxv.sHtML

[Q70] 更新统计信息
来源：http://read.share.hesvh.cn/Article/details/gepgnzcne.sHtML

ANALYZE TABLE users;
来源：http://wap.fehbvm.com/Article/details/gfatpktvq.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.zdbjq.cn/Article/details/gdkkctyzp.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.fehbvm.com/Article/details/gzqjztjju.sHtML

[Q72] 查看索引
来源：http://m.share.zdbjq.cn/Article/details/garrjhczo.sHtML

SHOW INDEX FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/ggvhxquzs.sHtML

[Q73] 查看表状态
来源：http://3g.zdbjq.cn/Article/details/ggaohguqg.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.zdbjq.cn/Article/details/gmyidnbdn.sHtML

[Q74] 强制使用索引
来源：http://mobile.zdbjq.cn/Article/details/ghtdwmagh.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.fehbvm.com/Article/details/geircndbo.sHtML

[Q75] 日期格式化
来源：http://3g.hesvh.cn/Article/details/gozuantfa.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/gnvfyrcjq.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.blog.hesvh.cn/Article/details/gqyymyovh.sHtML

[Q76] 按天统计
来源：http://m.share.hesvh.cn/Article/details/grzvwsaat.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.zdbjq.cn/Article/details/gejqtoakr.sHtML

[Q77] 时间加减
来源：http://m.share.zdbjq.cn/Article/details/gacavxjmq.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://m.share.hesvh.cn/Article/details/gqyedfeyj.sHtML

[Q78] 当前时间
来源：http://mobile.hesvh.cn/Article/details/gixfvsceh.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.zdbjq.cn/Article/details/gzbiutwdg.sHtML

[Q79] 字符串拼接
来源：http://mobile.zdbjq.cn/Article/details/gfhogtvvv.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.hesvh.cn/Article/details/gqpotonav.sHtML

[Q80] 字符串截取
来源：http://mobile.zdbjq.cn/Article/details/gsxxidgks.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.zdbjq.cn/Article/details/gvjqefrcn.sHtML

[Q81] 字符串替换
来源：http://wap.zdbjq.cn/Article/details/gcahoihgv.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gihbvmndd.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.hesvh.cn/Article/details/geycrzoxd.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.fehbvm.com/Article/details/gpqxrqfoy.sHtML

[Q83] 大小写转换
来源：http://m.share.hesvh.cn/Article/details/gjluqrpul.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.zdbjq.cn/Article/details/goybhvcbp.sHtML

[Q84] 去除首尾空格
来源：http://read.share.zdbjq.cn/Article/details/gspcsqsrh.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gvaaizvmq.sHtML

[Q85] 数值取整
来源：http://baike.hesvh.cn/Article/details/gcmxxqhgr.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.hesvh.cn/Article/details/gyppatbjp.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.hesvh.cn/Article/details/getspsurm.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.fehbvm.com/Article/details/gewkejcdu.sHtML

[Q87] JSON 字段做条件
来源：http://baike.zdbjq.cn/Article/details/gkasojcwt.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wap.zdbjq.cn/Article/details/gpdrmsoyp.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.hesvh.cn/Article/details/gibhhneoi.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.zdbjq.cn/Article/details/gymiaopjg.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.fehbvm.com/Article/details/guvfrxaky.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.zdbjq.cn/Article/details/gybarzmnq.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.hesvh.cn/Article/details/gmuvyvtfj.sHtML

[Q90] 生成序号列
来源：http://read.share.fehbvm.com/Article/details/gtmttycvm.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.fehbvm.com/Article/details/gmtjucdwv.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gyebhiurb.sHtML

R. Bash 专题
来源：http://read.share.zdbjq.cn/Article/details/gwkllsqtd.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gnkdcwcyn.sHtML

[R01] shebang 与严格模式
来源：http://www.blog.fehbvm.com/Article/details/gdnhwknas.sHtML

#!/usr/bin/env bash
来源：http://www.share.zdbjq.cn/Article/details/gktgsejji.sHtML

set -euo pipefail
来源：http://www.share.hesvh.cn/Article/details/gbfgmytqs.sHtML

[R02] 变量赋值与使用
来源：http://blog.hesvh.cn/Article/details/guprmppcb.sHtML

name="Tom"; echo "$name"
来源：http://m.share.hesvh.cn/Article/details/gzlwjcxuw.sHtML

[R03] 只读变量
来源：http://blog.zdbjq.cn/Article/details/gqfiljmfz.sHtML

readonly PI=3.14
来源：http://www.m.share.hesvh.cn/Article/details/gkqnmgdbw.sHtML

[R04] 位置参数
来源：http://3g.fehbvm.com/Article/details/ghoqgiimb.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.hesvh.cn/Article/details/gndslvyaj.sHtML

[R05] 参数默认值
来源：http://baike.zdbjq.cn/Article/details/giklkiuxb.sHtML

name="${1:-default}"
来源：http://www.blog.hesvh.cn/Article/details/gyvkucade.sHtML

[R06] 判断命令是否存在
来源：http://www.share.fehbvm.com/Article/details/guycigchz.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.zdbjq.cn/Article/details/guzaisxqf.sHtML

[R07] if 判断文件
来源：http://blog.hesvh.cn/Article/details/gxmxiwyei.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.fehbvm.com/Article/details/gabcgbrrp.sHtML

[R08] 数值比较
来源：http://3g.hesvh.cn/Article/details/gjnfbixmq.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.fehbvm.com/Article/details/gitktzpwn.sHtML

[R09] 字符串比较
来源：http://blog.zdbjq.cn/Article/details/gmhfbkpcp.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.zdbjq.cn/Article/details/gctpptzbb.sHtML

[R10] 正则匹配
来源：http://blog.hesvh.cn/Article/details/gumbxtsfd.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.hesvh.cn/Article/details/gphtchcjb.sHtML

[R11] case 多分支
来源：http://wap.hesvh.cn/Article/details/gvkacpsgo.sHtML

case "$1" in
来源：http://m.share.zdbjq.cn/Article/details/gmxbcwzqn.sHtML

start) echo "启动" ;;
来源：http://www.share.fehbvm.com/Article/details/gjftxynfv.sHtML

stop)  echo "停止" ;;
来源：http://mobile.fehbvm.com/Article/details/gbacgixkk.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.fehbvm.com/Article/details/gdqjthhjm.sHtML

esac
来源：http://blog.zdbjq.cn/Article/details/gykutgtng.sHtML

[R12] for 遍历文件
来源：http://3g.zdbjq.cn/Article/details/ggffzdfde.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.hesvh.cn/Article/details/gzyjaqetj.sHtML

[R13] for 计数循环
来源：http://mobile.zdbjq.cn/Article/details/gxyunthdt.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.fehbvm.com/Article/details/gbbiyjgxb.sHtML

[R14] C 风格 for
来源：http://baike.zdbjq.cn/Article/details/gpghluoci.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.hesvh.cn/Article/details/gwxanzhid.sHtML

[R15] while 逐行读文件
来源：http://3g.hesvh.cn/Article/details/gyodjvczo.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.hesvh.cn/Article/details/gplempukw.sHtML

[R16] until 等待条件
来源：http://www.blog.hesvh.cn/Article/details/gkejelumx.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.fehbvm.com/Article/details/gsdcowhsh.sHtML

[R17] 数组定义与取值
来源：http://blog.hesvh.cn/Article/details/gyhkbamnf.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.zdbjq.cn/Article/details/gzzwwrrcm.sHtML

[R18] 遍历数组
来源：http://read.share.zdbjq.cn/Article/details/gnaezxpsb.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.fehbvm.com/Article/details/geveirskt.sHtML

[R19] 数组长度
来源：http://mobile.hesvh.cn/Article/details/gjoasyyxj.sHtML

echo "${#arr[@]}"
来源：http://www.share.fehbvm.com/Article/details/glzxzfjzz.sHtML

[R20] 关联数组（字典）
来源：http://mobile.zdbjq.cn/Article/details/gurotxttj.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.hesvh.cn/Article/details/gigjmpydi.sHtML

[R21] 字符串长度
来源：http://baike.hesvh.cn/Article/details/gpechgcyv.sHtML

echo "${#s}"
来源：http://3g.fehbvm.com/Article/details/gjaxgdxfi.sHtML

[R22] 截取子串
来源：http://3g.fehbvm.com/Article/details/gouvuwavm.sHtML

echo "${s:0:5}"
来源：http://www.m.share.hesvh.cn/Article/details/gqcxttbdh.sHtML

[R23] 字符串替换
来源：http://www.share.fehbvm.com/Article/details/gwxlwepuf.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.fehbvm.com/Article/details/grfovugvb.sHtML

[R24] 大小写转换
来源：http://read.share.hesvh.cn/Article/details/gdsvzslaz.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.zdbjq.cn/Article/details/gktpnudmm.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.hesvh.cn/Article/details/gsxkmahra.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.zdbjq.cn/Article/details/gthqsciuz.sHtML

[R26] 命令替换
来源：http://mobile.zdbjq.cn/Article/details/gxlhmbled.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.zdbjq.cn/Article/details/gdhxucfdn.sHtML

[R27] 算术展开
来源：http://mobile.fehbvm.com/Article/details/gvgyrmuqg.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.zdbjq.cn/Article/details/gqyrhciai.sHtML

[R28] 浮点运算
来源：http://3g.hesvh.cn/Article/details/gumqxfovx.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.hesvh.cn/Article/details/gmqjrnmym.sHtML

[R29] 定义函数
来源：http://www.blog.fehbvm.com/Article/details/goumnucpr.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.zdbjq.cn/Article/details/gzkkwsskg.sHtML

[R30] 函数返回状态码
来源：http://3g.zdbjq.cn/Article/details/gbqffsoqd.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.hesvh.cn/Article/details/gmeroamqt.sHtML

[R31] 局部变量
来源：http://3g.fehbvm.com/Article/details/glfvkeonh.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.fehbvm.com/Article/details/grmibygjo.sHtML

[R32] 参数个数校验
来源：http://www.blog.fehbvm.com/Article/details/gfpqaqrxq.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.fehbvm.com/Article/details/gsyxsghgz.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.zdbjq.cn/Article/details/gaxpxblop.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.zdbjq.cn/Article/details/gnypskrlh.sHtML

[R34] 退出时清理
来源：http://blog.zdbjq.cn/Article/details/gbwfbujbd.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.fehbvm.com/Article/details/giejjacts.sHtML

[R35] 后台执行并等待
来源：http://m.share.zdbjq.cn/Article/details/gewqdbnxg.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.hesvh.cn/Article/details/gikvrhejk.sHtML

[R36] 并发执行多个任务
来源：http://m.share.fehbvm.com/Article/details/gwcfucouu.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.zdbjq.cn/Article/details/gkyjbgnqy.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.zdbjq.cn/Article/details/gxbxbusuh.sHtML

files=$(ls -1)
来源：http://read.share.fehbvm.com/Article/details/gojurmili.sHtML

[R38] 管道串联
来源：http://wap.hesvh.cn/Article/details/gpxiywuxc.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.fehbvm.com/Article/details/gcvsfmxto.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.hesvh.cn/Article/details/gusrxeflp.sHtML

cmd > out.log 2>&1
来源：http://m.share.hesvh.cn/Article/details/gsjivgmlx.sHtML

[R40] 追加写日志
来源：http://m.share.fehbvm.com/Article/details/gfpywkvnp.sHtML

echo "log" >> out.log
来源：http://read.share.hesvh.cn/Article/details/gnfrjjzsc.sHtML

[R41] 丢弃输出
来源：http://m.share.hesvh.cn/Article/details/guiiyumxm.sHtML

cmd >/dev/null 2>&1
来源：http://baike.hesvh.cn/Article/details/gesgujdfb.sHtML

[R42] 输入重定向
来源：http://m.share.fehbvm.com/Article/details/gnznpkixh.sHtML

wc -l < a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gfzzzmjip.sHtML

[R43] 按名字查找文件
来源：http://baike.fehbvm.com/Article/details/gzyxnmjrw.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.zdbjq.cn/Article/details/gpzlrpoop.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.hesvh.cn/Article/details/gclzrglks.sHtML

find . -mtime -7 -type f
来源：http://www.blog.hesvh.cn/Article/details/gfrvjkgtf.sHtML

[R45] 批量删除
来源：http://wap.fehbvm.com/Article/details/glwlpcsmb.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.hesvh.cn/Article/details/gtknljbhx.sHtML

[R46] 递归替换文件内容
来源：http://mobile.fehbvm.com/Article/details/gnlewdtza.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.fehbvm.com/Article/details/gfydhrxri.sHtML

[R47] sed 单行替换
来源：http://www.blog.hesvh.cn/Article/details/gxsmxdvvc.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.zdbjq.cn/Article/details/gvmbhdyuz.sHtML

[R48] awk 取指定列
来源：http://3g.zdbjq.cn/Article/details/gymburbyn.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gnvvfmqds.sHtML

[R49] awk 带条件
来源：http://m.share.zdbjq.cn/Article/details/guwxkmbda.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.hesvh.cn/Article/details/glbluyvqs.sHtML

[R50] awk 求和
来源：http://blog.zdbjq.cn/Article/details/gaunpaznf.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.zdbjq.cn/Article/details/guyytoxgh.sHtML

[R51] 排序去重取前几
来源：http://blog.fehbvm.com/Article/details/gqakyvnht.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.hesvh.cn/Article/details/grngbbecx.sHtML

[R52] 统计行数
来源：http://read.share.fehbvm.com/Article/details/gupdrceqe.sHtML

wc -l a.txt
来源：http://3g.fehbvm.com/Article/details/gwbgixbbp.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.hesvh.cn/Article/details/gfzhpiuuq.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.zdbjq.cn/Article/details/gsoqngcje.sHtML

[R54] 比较两个文件
来源：http://www.m.share.fehbvm.com/Article/details/gzwdtxnvj.sHtML

diff a.txt b.txt
来源：http://wap.zdbjq.cn/Article/details/gtylxbdoe.sHtML

[R55] 压缩与解压
来源：http://www.share.zdbjq.cn/Article/details/gqivcpwsp.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.fehbvm.com/Article/details/gowrovllp.sHtML

[R56] 远程拷贝
来源：http://blog.zdbjq.cn/Article/details/gewxtswkq.sHtML

scp file user@host:/path/
来源：http://3g.zdbjq.cn/Article/details/gxatcpsmz.sHtML

[R57] 远程执行命令
来源：http://www.m.share.fehbvm.com/Article/details/gilyxewdz.sHtML

ssh user@host 'uptime'
来源：http://wap.zdbjq.cn/Article/details/gktrikdtv.sHtML

[R58] 下载文件
来源：http://wap.zdbjq.cn/Article/details/gozjyqock.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.hesvh.cn/Article/details/gmnfmzfot.sHtML

[R59] 发 POST JSON
来源：http://3g.fehbvm.com/Article/details/gkenbmnil.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.fehbvm.com/Article/details/gvezbhugz.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.fehbvm.com/Article/details/gmpdjxnrv.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.fehbvm.com/Article/details/gaambfykp.sHtML

[R61] 磁盘占用
来源：http://read.share.hesvh.cn/Article/details/gcuacfvdf.sHtML

df -h;  du -sh *
来源：http://baike.hesvh.cn/Article/details/grgxnacjb.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.hesvh.cn/Article/details/gmemmgsqb.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.fehbvm.com/Article/details/gezdjiewd.sHtML

[R63] 内存与进程
来源：http://www.share.zdbjq.cn/Article/details/gbysuabrd.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.hesvh.cn/Article/details/gqrcugpin.sHtML

[R64] 结束进程
来源：http://www.blog.hesvh.cn/Article/details/gcnwvaflm.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.hesvh.cn/Article/details/ghnnuwegd.sHtML

[R65] 查看端口占用
来源：http://www.m.share.fehbvm.com/Article/details/gbndbwpke.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.fehbvm.com/Article/details/gkmroaocu.sHtML

[R66] 定时任务
来源：http://3g.zdbjq.cn/Article/details/gjaxdsisd.sHtML

crontab -e;  crontab -l
来源：http://blog.hesvh.cn/Article/details/gjcfzapwp.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.fehbvm.com/Article/details/glqoonnnu.sHtML

openssl rand -hex 16
来源：http://www.blog.fehbvm.com/Article/details/gjebryjqi.sHtML

[R68] 计算文件校验值
来源：http://wap.zdbjq.cn/Article/details/gkludjcoz.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.fehbvm.com/Article/details/gdvqaeypw.sHtML

[R69] 生成随机密码
来源：http://baike.fehbvm.com/Article/details/gubvzruci.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.fehbvm.com/Article/details/grssgsoiq.sHtML

[R70] 时间戳与互转
来源：http://wap.fehbvm.com/Article/details/goiulyltt.sHtML

date +%s;  date -d @1700000000
来源：http://3g.hesvh.cn/Article/details/gsebaaroq.sHtML

[R71] 日期格式化
来源：http://blog.fehbvm.com/Article/details/gcjuyyihq.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.zdbjq.cn/Article/details/gcuqnpbrd.sHtML

[R72] 等待端口就绪
来源：http://blog.hesvh.cn/Article/details/gxruemewj.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.hesvh.cn/Article/details/guwqkzhuv.sHtML

[R73] 分割大日志
来源：http://www.share.zdbjq.cn/Article/details/gpzfhramv.sHtML

split -l 1000 big.log part_
来源：http://blog.hesvh.cn/Article/details/ghnqmfibl.sHtML

[R74] 批量重命名
来源：http://blog.fehbvm.com/Article/details/gjstligdj.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.zdbjq.cn/Article/details/greexznyi.sHtML

[R75] 导出环境变量
来源：http://www.m.share.fehbvm.com/Article/details/gsqknlpks.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.fehbvm.com/Article/details/gkiyzkjkm.sHtML

[R76] 使用临时文件
来源：http://3g.zdbjq.cn/Article/details/gdzyjflkp.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fehbvm.com/Article/details/gkhjndqyq.sHtML

[R77] 读取用户输入
来源：http://3g.zdbjq.cn/Article/details/gqbmlgdyr.sHtML

read -rp "请输入: " ans
来源：http://www.blog.hesvh.cn/Article/details/gsqrjkunv.sHtML

[R78] 交互式菜单
来源：http://baike.zdbjq.cn/Article/details/gxkoxfxfu.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.fehbvm.com/Article/details/gpcrwpvls.sHtML

[R79] 解析命令行选项
来源：http://m.share.zdbjq.cn/Article/details/gjskewhnz.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.fehbvm.com/Article/details/gzfiaoqgx.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.hesvh.cn/Article/details/gvblqegxx.sHtML

time ./run.sh
来源：http://www.m.share.fehbvm.com/Article/details/gqpxylqtj.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/guorxndqj.sHtML


<!-- 参考信息 -->