代发 wailian999

[Q33] 多列分组
来源：http://www.blog.zdbjq.cn/Article/details/gzrwdnfwq.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://3g.zdbjq.cn/Article/details/ggbmbljxv.sHtML

[Q34] 每组取第一条
来源：http://3g.fehbvm.com/Article/details/gqgzstbyl.sHtML

SELECT * FROM (
来源：http://baike.zdbjq.cn/Article/details/gxrjwnohv.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://blog.hesvh.cn/Article/details/geflawaew.sHtML

) t WHERE rn = 1;
来源：http://3g.zdbjq.cn/Article/details/gwdvtlcko.sHtML

[Q35] 内连接
来源：http://m.share.hesvh.cn/Article/details/guojqottl.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://m.share.zdbjq.cn/Article/details/gmtaaqefj.sHtML

[Q36] 左连接
来源：http://www.share.hesvh.cn/Article/details/gwtgrlhuq.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.fehbvm.com/Article/details/gfkpcpzvu.sHtML

[Q37] 右连接
来源：http://mobile.fehbvm.com/Article/details/gcuwpnlyf.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.m.share.zdbjq.cn/Article/details/gdoplenqp.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://baike.fehbvm.com/Article/details/gzuiuyawj.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://baike.fehbvm.com/Article/details/gmqhyvwnr.sHtML

[Q39] 自连接（查上下级）
来源：http://wap.hesvh.cn/Article/details/guflfbctu.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.fehbvm.com/Article/details/ggmcfhbme.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://m.share.hesvh.cn/Article/details/gsrwpmdmc.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.hesvh.cn/Article/details/gddxfcckl.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mobile.zdbjq.cn/Article/details/gdudbnczj.sHtML

[Q41] 多表连接
来源：http://www.m.share.zdbjq.cn/Article/details/gasztngtz.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://baike.hesvh.cn/Article/details/gydnfjoup.sHtML

JOIN users u ON u.id = o.user_id
来源：http://mobile.zdbjq.cn/Article/details/gkecprwpq.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.fehbvm.com/Article/details/gdsnipaaa.sHtML

[Q42] 连接条件附加过滤
来源：http://blog.zdbjq.cn/Article/details/garenbbtr.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.blog.fehbvm.com/Article/details/gnzmqkvwm.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://read.share.hesvh.cn/Article/details/gkunfktym.sHtML

[Q43] 标量子查询
来源：http://www.m.share.fehbvm.com/Article/details/gzvzzznku.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.share.hesvh.cn/Article/details/gwnyuigpm.sHtML

[Q44] IN 子查询
来源：http://www.blog.zdbjq.cn/Article/details/gyqpdtfot.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mobile.zdbjq.cn/Article/details/glvbkduft.sHtML

[Q45] EXISTS 判断存在
来源：http://www.share.zdbjq.cn/Article/details/gbbranlci.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.hesvh.cn/Article/details/glbwtateo.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://wap.zdbjq.cn/Article/details/grnrrodrd.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.zdbjq.cn/Article/details/gfigqdomr.sHtML

[Q47] 与平均值比较
来源：http://blog.hesvh.cn/Article/details/gjwogmukv.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.m.share.hesvh.cn/Article/details/gbifsimev.sHtML

[Q48] CTE 公用表表达式
来源：http://baike.hesvh.cn/Article/details/gzrdgjixf.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.blog.zdbjq.cn/Article/details/ggndpwwpj.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://wap.hesvh.cn/Article/details/gwtmayrbz.sHtML

[Q49] 更新单行
来源：http://m.share.zdbjq.cn/Article/details/gdadajydh.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mobile.fehbvm.com/Article/details/ggwzizyrn.sHtML

[Q50] 批量更新
来源：http://www.blog.hesvh.cn/Article/details/glsbxynub.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.zdbjq.cn/Article/details/glhtqwork.sHtML

[Q51] 用子查询更新
来源：http://mobile.fehbvm.com/Article/details/gjfpykizh.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.share.zdbjq.cn/Article/details/gaighedaf.sHtML

[Q52] 删除指定行
来源：http://baike.hesvh.cn/Article/details/gphtfbbox.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.blog.fehbvm.com/Article/details/gbypmgwbu.sHtML

[Q53] 按条件删除
来源：http://m.share.fehbvm.com/Article/details/ghfbpkekt.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wap.zdbjq.cn/Article/details/gxfkgtrov.sHtML

[Q54] 清空表
来源：http://baike.fehbvm.com/Article/details/grxpkqepl.sHtML

TRUNCATE TABLE logs;
来源：http://3g.fehbvm.com/Article/details/gkalabnrf.sHtML

[Q55] 排名（并列占位）
来源：http://www.share.fehbvm.com/Article/details/gpiltxgqv.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://blog.zdbjq.cn/Article/details/golvqyrnn.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.fehbvm.com/Article/details/gnlikkeha.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.blog.fehbvm.com/Article/details/gmypgwxkg.sHtML

[Q57] 行号
来源：http://mobile.hesvh.cn/Article/details/gaphjykty.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.zdbjq.cn/Article/details/gnltazjnt.sHtML

[Q58] 累计求和
来源：http://www.blog.fehbvm.com/Article/details/gunnvjetp.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://read.share.fehbvm.com/Article/details/gccwmbkbv.sHtML

[Q59] 分组内累计
来源：http://baike.zdbjq.cn/Article/details/gpmaumrme.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://baike.zdbjq.cn/Article/details/gaawraljj.sHtML

[Q60] 取上一行 / 下一行
来源：http://wap.hesvh.cn/Article/details/gzqyntmvi.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.m.share.fehbvm.com/Article/details/gbqtejnqt.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.hesvh.cn/Article/details/ggoyzicrr.sHtML

[Q61] 移动平均
来源：http://www.share.fehbvm.com/Article/details/gznyfrotp.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://blog.hesvh.cn/Article/details/gncyxryyn.sHtML

[Q62] 分组占比
来源：http://baike.fehbvm.com/Article/details/gilsicfks.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://baike.fehbvm.com/Article/details/gbyuzaxwa.sHtML

[Q63] 开启事务
来源：http://3g.zdbjq.cn/Article/details/gxwtjipja.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://3g.fehbvm.com/Article/details/gyvtfecoh.sHtML

[Q64] 提交事务
来源：http://www.m.share.zdbjq.cn/Article/details/gimxchxmj.sHtML

COMMIT;
来源：http://www.share.hesvh.cn/Article/details/gvxuxrzsw.sHtML

[Q65] 回滚事务
来源：http://read.share.zdbjq.cn/Article/details/gjnsvkrlz.sHtML

ROLLBACK;
来源：http://blog.fehbvm.com/Article/details/gbrudflga.sHtML

[Q66] 行锁查询
来源：http://www.share.fehbvm.com/Article/details/gbfzxcyah.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.blog.zdbjq.cn/Article/details/godnxrgee.sHtML

[Q67] 设置隔离级别
来源：http://3g.zdbjq.cn/Article/details/gnvtftkta.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.hesvh.cn/Article/details/gaxlgmgtn.sHtML

[Q68] 保存点
来源：http://www.share.fehbvm.com/Article/details/gbhcnvyct.sHtML

SAVEPOINT sp1;
来源：http://wap.fehbvm.com/Article/details/gvsomlfup.sHtML

ROLLBACK TO sp1;
来源：http://blog.hesvh.cn/Article/details/gspdwvbyr.sHtML

[Q69] 查看执行计划
来源：http://baike.zdbjq.cn/Article/details/glibeitkg.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.hesvh.cn/Article/details/gdeyoytuk.sHtML

[Q70] 更新统计信息
来源：http://mobile.zdbjq.cn/Article/details/gfxhzblmb.sHtML

ANALYZE TABLE users;
来源：http://3g.zdbjq.cn/Article/details/gpgrwzxsj.sHtML

[Q71] 查看建表语句
来源：http://read.share.fehbvm.com/Article/details/ggejhqkqv.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.fehbvm.com/Article/details/gnrpbmfyl.sHtML

[Q72] 查看索引
来源：http://www.share.zdbjq.cn/Article/details/gnnqijxvb.sHtML

SHOW INDEX FROM users;
来源：http://m.share.hesvh.cn/Article/details/gynmwcxlc.sHtML

[Q73] 查看表状态
来源：http://baike.fehbvm.com/Article/details/gmuolvyrj.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.hesvh.cn/Article/details/gnpkrczek.sHtML

[Q74] 强制使用索引
来源：http://3g.hesvh.cn/Article/details/gkitqeyyi.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.fehbvm.com/Article/details/gzfyzmpqq.sHtML

[Q75] 日期格式化
来源：http://read.share.fehbvm.com/Article/details/gkzaagmtp.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.zdbjq.cn/Article/details/gwfluiqac.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://baike.hesvh.cn/Article/details/gettbmjdx.sHtML

[Q76] 按天统计
来源：http://www.m.share.zdbjq.cn/Article/details/gghpuyelg.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.zdbjq.cn/Article/details/gwzwagliw.sHtML

[Q77] 时间加减
来源：http://baike.fehbvm.com/Article/details/gpemhtptk.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.hesvh.cn/Article/details/gbmfxkpgy.sHtML

[Q78] 当前时间
来源：http://www.m.share.hesvh.cn/Article/details/gjvpedakr.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.m.share.zdbjq.cn/Article/details/gxuqughuk.sHtML

[Q79] 字符串拼接
来源：http://3g.hesvh.cn/Article/details/glgqdewio.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.fehbvm.com/Article/details/gyexsnpdf.sHtML

[Q80] 字符串截取
来源：http://read.share.hesvh.cn/Article/details/gmyvixqpu.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.hesvh.cn/Article/details/gqebrdmyz.sHtML

[Q81] 字符串替换
来源：http://read.share.zdbjq.cn/Article/details/gppslkktj.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.hesvh.cn/Article/details/gqtamlsdf.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.fehbvm.com/Article/details/gdrcyphda.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.fehbvm.com/Article/details/gwjxvzftu.sHtML

[Q83] 大小写转换
来源：http://www.m.share.fehbvm.com/Article/details/gmtgjdbnn.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.zdbjq.cn/Article/details/gvmyhhmtj.sHtML

[Q84] 去除首尾空格
来源：http://wap.hesvh.cn/Article/details/gtcuulhzs.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.fehbvm.com/Article/details/geqvuzrpo.sHtML

[Q85] 数值取整
来源：http://mobile.hesvh.cn/Article/details/gptejvmpo.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.fehbvm.com/Article/details/gexixqace.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.fehbvm.com/Article/details/gdwyrpdkj.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.zdbjq.cn/Article/details/giqjrqmtl.sHtML

[Q87] JSON 字段做条件
来源：http://blog.hesvh.cn/Article/details/ggmsskgov.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.hesvh.cn/Article/details/gglcheyxf.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.hesvh.cn/Article/details/gsxheoyli.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.fehbvm.com/Article/details/gjirzqnby.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/glqdsqwpd.sHtML

[Q89] 判断表是否存在
来源：http://mobile.zdbjq.cn/Article/details/giocarvpt.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.zdbjq.cn/Article/details/gaddbzxyy.sHtML

[Q90] 生成序号列
来源：http://wap.fehbvm.com/Article/details/gxkdoachd.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.hesvh.cn/Article/details/gnqtfdewi.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/guojclcji.sHtML

R. Bash 专题
来源：http://m.share.hesvh.cn/Article/details/guawmewlc.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gzcrvtvzk.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.hesvh.cn/Article/details/gfvulbvfg.sHtML

#!/usr/bin/env bash
来源：http://blog.hesvh.cn/Article/details/gftarrjtd.sHtML

set -euo pipefail
来源：http://wap.fehbvm.com/Article/details/gwrqtfozf.sHtML

[R02] 变量赋值与使用
来源：http://baike.fehbvm.com/Article/details/glcikrijd.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.zdbjq.cn/Article/details/gqlsugwyw.sHtML

[R03] 只读变量
来源：http://read.share.fehbvm.com/Article/details/gljhefxqq.sHtML

readonly PI=3.14
来源：http://www.m.share.fehbvm.com/Article/details/gvasmmrch.sHtML

[R04] 位置参数
来源：http://3g.fehbvm.com/Article/details/glmvnvolv.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.hesvh.cn/Article/details/gtfhvpwbv.sHtML

[R05] 参数默认值
来源：http://www.share.fehbvm.com/Article/details/gewbogrsx.sHtML

name="${1:-default}"
来源：http://wap.fehbvm.com/Article/details/gxvcrvhjt.sHtML

[R06] 判断命令是否存在
来源：http://baike.hesvh.cn/Article/details/gdjuqmxwk.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.hesvh.cn/Article/details/gsgjugsrr.sHtML

[R07] if 判断文件
来源：http://m.share.hesvh.cn/Article/details/ggsixcryw.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.hesvh.cn/Article/details/gtgxmsahx.sHtML

[R08] 数值比较
来源：http://read.share.hesvh.cn/Article/details/gnjvhurhl.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.hesvh.cn/Article/details/gtqgixhlr.sHtML

[R09] 字符串比较
来源：http://www.blog.zdbjq.cn/Article/details/gaaytvbsl.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.zdbjq.cn/Article/details/gjdocejmj.sHtML

[R10] 正则匹配
来源：http://www.m.share.zdbjq.cn/Article/details/geclozdnt.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.fehbvm.com/Article/details/galsohmnc.sHtML

[R11] case 多分支
来源：http://wap.fehbvm.com/Article/details/gnhxahopx.sHtML

case "$1" in
来源：http://www.share.hesvh.cn/Article/details/grpqhgqcg.sHtML

start) echo "启动" ;;
来源：http://blog.hesvh.cn/Article/details/gyskhxfge.sHtML

stop)  echo "停止" ;;
来源：http://blog.hesvh.cn/Article/details/gmndbprit.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.fehbvm.com/Article/details/ghdiicslk.sHtML

esac
来源：http://mobile.zdbjq.cn/Article/details/gpuqmquik.sHtML

[R12] for 遍历文件
来源：http://mobile.hesvh.cn/Article/details/gmhcwzzck.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.hesvh.cn/Article/details/grgqevvzf.sHtML

[R13] for 计数循环
来源：http://www.share.hesvh.cn/Article/details/gbufoovuz.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.zdbjq.cn/Article/details/gavazknni.sHtML

[R14] C 风格 for
来源：http://www.m.share.fehbvm.com/Article/details/gslfymebl.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.fehbvm.com/Article/details/gbwwpktdh.sHtML

[R15] while 逐行读文件
来源：http://www.share.fehbvm.com/Article/details/gmcmoloim.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.fehbvm.com/Article/details/grdbujhds.sHtML

[R16] until 等待条件
来源：http://www.m.share.zdbjq.cn/Article/details/gjrbyesnt.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.zdbjq.cn/Article/details/gzrgsrcvs.sHtML

[R17] 数组定义与取值
来源：http://www.share.fehbvm.com/Article/details/gdijhtfhq.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.zdbjq.cn/Article/details/ggntnjvka.sHtML

[R18] 遍历数组
来源：http://read.share.fehbvm.com/Article/details/grkdwidll.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.hesvh.cn/Article/details/giowlmqlx.sHtML

[R19] 数组长度
来源：http://mobile.zdbjq.cn/Article/details/gevljyied.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.zdbjq.cn/Article/details/gwxkegfmx.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.zdbjq.cn/Article/details/gvbcnglyb.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.hesvh.cn/Article/details/gujvbueeo.sHtML

[R21] 字符串长度
来源：http://baike.zdbjq.cn/Article/details/gqugxpymo.sHtML

echo "${#s}"
来源：http://m.share.hesvh.cn/Article/details/gwjvbjznf.sHtML

[R22] 截取子串
来源：http://mobile.zdbjq.cn/Article/details/gwkcpwgxk.sHtML

echo "${s:0:5}"
来源：http://www.blog.hesvh.cn/Article/details/gthhlewiq.sHtML

[R23] 字符串替换
来源：http://blog.hesvh.cn/Article/details/gcckqrpam.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.zdbjq.cn/Article/details/gefukhhth.sHtML

[R24] 大小写转换
来源：http://blog.hesvh.cn/Article/details/gjencrsgq.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.fehbvm.com/Article/details/gdafurwqy.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.zdbjq.cn/Article/details/gkwnvzewa.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.zdbjq.cn/Article/details/gxyxgvboy.sHtML

[R26] 命令替换
来源：http://www.blog.fehbvm.com/Article/details/ghcwxxjse.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.fehbvm.com/Article/details/gemvjaary.sHtML

[R27] 算术展开
来源：http://3g.fehbvm.com/Article/details/gomgpheff.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.hesvh.cn/Article/details/gchtbulss.sHtML

[R28] 浮点运算
来源：http://blog.fehbvm.com/Article/details/gkvifrppr.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.fehbvm.com/Article/details/gqxhracza.sHtML

[R29] 定义函数
来源：http://m.share.hesvh.cn/Article/details/gckihdltm.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.hesvh.cn/Article/details/gvqulatji.sHtML

[R30] 函数返回状态码
来源：http://blog.fehbvm.com/Article/details/gsdqeosdp.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.fehbvm.com/Article/details/glylpmhpy.sHtML

[R31] 局部变量
来源：http://blog.fehbvm.com/Article/details/gcnqlntjq.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.hesvh.cn/Article/details/ghjfpjohz.sHtML

[R32] 参数个数校验
来源：http://read.share.fehbvm.com/Article/details/gywsnsxwe.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.fehbvm.com/Article/details/guuttncon.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.hesvh.cn/Article/details/goeiytepf.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.zdbjq.cn/Article/details/geizsfvvp.sHtML

[R34] 退出时清理
来源：http://wap.hesvh.cn/Article/details/gleczddwb.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.hesvh.cn/Article/details/goedpccfb.sHtML

[R35] 后台执行并等待
来源：http://www.blog.hesvh.cn/Article/details/gppkgazjo.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.fehbvm.com/Article/details/gqltwscyb.sHtML

[R36] 并发执行多个任务
来源：http://m.share.hesvh.cn/Article/details/giwnmqvep.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.hesvh.cn/Article/details/gsquucxlj.sHtML

[R37] 把输出赋给变量
来源：http://blog.hesvh.cn/Article/details/gykorvkzs.sHtML

files=$(ls -1)
来源：http://www.m.share.zdbjq.cn/Article/details/gpwehtooj.sHtML

[R38] 管道串联
来源：http://3g.zdbjq.cn/Article/details/glckulgdu.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.zdbjq.cn/Article/details/gwgwqbomz.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.hesvh.cn/Article/details/gcpxdpakm.sHtML

cmd > out.log 2>&1
来源：http://m.share.fehbvm.com/Article/details/gzeksnrbu.sHtML

[R40] 追加写日志
来源：http://www.blog.fehbvm.com/Article/details/grsijxijq.sHtML

echo "log" >> out.log
来源：http://www.m.share.zdbjq.cn/Article/details/gjntzonen.sHtML

[R41] 丢弃输出
来源：http://www.share.fehbvm.com/Article/details/gcutbapha.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.hesvh.cn/Article/details/gkfmdnvpf.sHtML

[R42] 输入重定向
来源：http://3g.fehbvm.com/Article/details/gjfeqwqxl.sHtML

wc -l < a.txt
来源：http://read.share.fehbvm.com/Article/details/gtdkuswub.sHtML

[R43] 按名字查找文件
来源：http://www.share.zdbjq.cn/Article/details/gfuadedos.sHtML

find . -name "*.log" -type f
来源：http://m.share.hesvh.cn/Article/details/gylmqwaim.sHtML

[R44] 按修改时间查找
来源：http://baike.zdbjq.cn/Article/details/gqxfaclfm.sHtML

find . -mtime -7 -type f
来源：http://mobile.fehbvm.com/Article/details/gshqjogba.sHtML

[R45] 批量删除
来源：http://blog.zdbjq.cn/Article/details/gkpioaiai.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.zdbjq.cn/Article/details/gsulzqupg.sHtML

[R46] 递归替换文件内容
来源：http://www.share.zdbjq.cn/Article/details/gufvbbekp.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.zdbjq.cn/Article/details/gileetvvc.sHtML

[R47] sed 单行替换
来源：http://www.m.share.fehbvm.com/Article/details/gcgbimgke.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.fehbvm.com/Article/details/gtgdtyopi.sHtML

[R48] awk 取指定列
来源：http://read.share.fehbvm.com/Article/details/gziyurqku.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.zdbjq.cn/Article/details/gcrpbhsiq.sHtML

[R49] awk 带条件
来源：http://baike.zdbjq.cn/Article/details/gcnsiijvt.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.fehbvm.com/Article/details/gtbvzlabh.sHtML

[R50] awk 求和
来源：http://www.m.share.fehbvm.com/Article/details/grntnpeob.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.hesvh.cn/Article/details/goaqpxosn.sHtML

[R51] 排序去重取前几
来源：http://blog.zdbjq.cn/Article/details/gcjeaqpxg.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.hesvh.cn/Article/details/gxqobzjiw.sHtML

[R52] 统计行数
来源：http://3g.hesvh.cn/Article/details/gnqanthqo.sHtML

wc -l a.txt
来源：http://www.blog.zdbjq.cn/Article/details/gojivodzq.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.hesvh.cn/Article/details/gzabhhwwl.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.hesvh.cn/Article/details/gsyuptgvu.sHtML

[R54] 比较两个文件
来源：http://baike.hesvh.cn/Article/details/gsqcfcmzo.sHtML

diff a.txt b.txt
来源：http://blog.hesvh.cn/Article/details/gdfmkgdtr.sHtML

[R55] 压缩与解压
来源：http://3g.hesvh.cn/Article/details/gasatcppb.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.zdbjq.cn/Article/details/gyetbiior.sHtML

[R56] 远程拷贝
来源：http://wap.zdbjq.cn/Article/details/gzmabarxs.sHtML

scp file user@host:/path/
来源：http://m.share.hesvh.cn/Article/details/gapoxtxcg.sHtML

[R57] 远程执行命令
来源：http://www.share.zdbjq.cn/Article/details/gepxzfoji.sHtML

ssh user@host 'uptime'
来源：http://blog.fehbvm.com/Article/details/gsdyoynah.sHtML

[R58] 下载文件
来源：http://blog.zdbjq.cn/Article/details/gufvlhhhh.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.zdbjq.cn/Article/details/gvoswtwya.sHtML

[R59] 发 POST JSON
来源：http://www.blog.zdbjq.cn/Article/details/gbmpqwgll.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.fehbvm.com/Article/details/gxyhdkczr.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.hesvh.cn/Article/details/gedpgriea.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.hesvh.cn/Article/details/ggxbpsaxj.sHtML

[R61] 磁盘占用
来源：http://www.m.share.zdbjq.cn/Article/details/gxnjtphgm.sHtML

df -h;  du -sh *
来源：http://www.m.share.hesvh.cn/Article/details/ghfydlsqi.sHtML

[R62] 找最占空间的文件
来源：http://3g.zdbjq.cn/Article/details/gpqrmcpes.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.fehbvm.com/Article/details/gtrspfbwz.sHtML

[R63] 内存与进程
来源：http://www.share.hesvh.cn/Article/details/gopvdlbwh.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.zdbjq.cn/Article/details/gkehdhvrm.sHtML

[R64] 结束进程
来源：http://3g.hesvh.cn/Article/details/ghmzeugul.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.zdbjq.cn/Article/details/giemfcmdl.sHtML

[R65] 查看端口占用
来源：http://3g.hesvh.cn/Article/details/giyhlxcxp.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.zdbjq.cn/Article/details/glxmsqvvs.sHtML

[R66] 定时任务
来源：http://www.share.fehbvm.com/Article/details/grkdhelvf.sHtML

crontab -e;  crontab -l
来源：http://wap.fehbvm.com/Article/details/gfvdkljet.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.zdbjq.cn/Article/details/ghnkyvjru.sHtML

openssl rand -hex 16
来源：http://wap.hesvh.cn/Article/details/gzyprsiwx.sHtML

[R68] 计算文件校验值
来源：http://3g.hesvh.cn/Article/details/gpcvknrlj.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.hesvh.cn/Article/details/goscpwwyo.sHtML

[R69] 生成随机密码
来源：http://blog.zdbjq.cn/Article/details/gidyhvnzs.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.hesvh.cn/Article/details/gvbhbqkat.sHtML

[R70] 时间戳与互转
来源：http://www.share.hesvh.cn/Article/details/gxylpcqct.sHtML

date +%s;  date -d @1700000000
来源：http://baike.fehbvm.com/Article/details/gxkwtnzey.sHtML

[R71] 日期格式化
来源：http://read.share.zdbjq.cn/Article/details/geqtdwdxr.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.fehbvm.com/Article/details/grmuabmcl.sHtML

[R72] 等待端口就绪
来源：http://www.blog.zdbjq.cn/Article/details/gmlbxejug.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.zdbjq.cn/Article/details/guzeppclx.sHtML

[R73] 分割大日志
来源：http://mobile.zdbjq.cn/Article/details/gaizqttii.sHtML

split -l 1000 big.log part_
来源：http://m.share.zdbjq.cn/Article/details/ghavyxhze.sHtML

[R74] 批量重命名
来源：http://www.blog.zdbjq.cn/Article/details/gwprgymcz.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.hesvh.cn/Article/details/gdiqkkput.sHtML

[R75] 导出环境变量
来源：http://www.share.zdbjq.cn/Article/details/gxakrqeyb.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.hesvh.cn/Article/details/gzuzwjzmv.sHtML

[R76] 使用临时文件
来源：http://www.blog.zdbjq.cn/Article/details/gupffrcfl.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.hesvh.cn/Article/details/gqclkofhd.sHtML

[R77] 读取用户输入
来源：http://wap.zdbjq.cn/Article/details/glbimskri.sHtML

read -rp "请输入: " ans
来源：http://mobile.zdbjq.cn/Article/details/gyegoedbh.sHtML

[R78] 交互式菜单
来源：http://3g.fehbvm.com/Article/details/gfsrgpovr.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.fehbvm.com/Article/details/ggkumpjnt.sHtML

[R79] 解析命令行选项
来源：http://wap.fehbvm.com/Article/details/gopdaemmc.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.zdbjq.cn/Article/details/gnyaokzmf.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.fehbvm.com/Article/details/gqijnqkdh.sHtML

time ./run.sh
来源：http://www.share.hesvh.cn/Article/details/grwpfbffp.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gpbqjsbbd.sHtML

S. C / C++ 专题
来源：http://3g.zdbjq.cn/Article/details/gcaewokwk.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gvlwguaas.sHtML

[S01] C：Hello World
来源：http://m.share.hesvh.cn/Article/details/ganszxojm.sHtML

#include <stdio.h>
来源：http://baike.fehbvm.com/Article/details/ghxshyrvo.sHtML


<!-- 参考信息 -->