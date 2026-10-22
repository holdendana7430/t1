代发 wailian999

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2fxmjmrej.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2wqyrkdmo.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2kharhctq.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2jtuogajk.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2qlczneza.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2uxadoxfn.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2nvgftsal.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2efumyudx.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2ntrbrjvv.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2jafecugv.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2roebxoco.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2kqslqwhw.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2hfyiyifq.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2mumtyhwn.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2qmyzydhj.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2gsvfflcw.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ykyrhnjx.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2fzvysfoo.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2vwqtkucm.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2cemospve.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2gloeougj.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2ysobzlju.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2odwaugun.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2zyvvsbcc.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2ahawcusk.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2vassovcc.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2pdgxsixm.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2rjgcshhw.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2jvvnojwh.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2ygtntjml.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2ncemyzix.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2bwocjwyo.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2bxqpxncq.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2tawymcye.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2msckgbnp.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2edjjlglw.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2wotaobdu.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2ypvxwcnv.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2hkocypvl.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2wjycjprp.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2ndxlrcwr.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2cdyadadn.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2yfabcwav.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2cfqjjwkk.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2jtztoudk.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2bibdnewv.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2noxavdef.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2wuapxrju.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2hywrybcz.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2pzstohqw.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2wanrydio.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2widaxxsf.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2nifgsdkc.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2ssdlqggt.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2kammvjfg.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2mjusqutb.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2araavdzn.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2tstulylp.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2jbywzoec.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2wueyuofi.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2xvrossjw.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2hujhrtmu.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2nhgvyhst.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2pbsybdwt.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2yprprspl.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2bjjkpuak.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2ethgryyh.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2sgqbfpny.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2nzynvwhg.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2uyzftmzh.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2ooifquwy.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2xoknnipt.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2jnlrlmdi.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2ivgryecs.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2qmokavou.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2mybrsvtn.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2klptmwjw.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2wapbctra.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2ndbptkec.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2xlhhgyso.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2hvuzybux.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2tvwlvpcx.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2fgnosmxx.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2zdrqjwrt.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2owegioug.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2onvticwy.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2yxlyazxe.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2icxmegoa.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2bsutkhxn.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2agtjbknr.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2tkstmljq.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2plyljvvf.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2qtqmwedf.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ehpceexd.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2oqplolce.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2txfsuuad.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2mcspagbh.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2fzdqueye.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2semoywdi.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2wmjiwnzp.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2gxgfvmfw.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2htevxnwj.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2qdowplut.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2jfikyzwn.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2dfgztppn.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2gwbygclf.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2ewcxybea.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2kioeyngy.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2thqqirbl.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2pnnavyai.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2khguuntc.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2uzisjyka.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2ibvltven.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2tjantilm.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2ucvqrcoj.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2ovzdhvki.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2uevxomue.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2nvqdltaa.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2ebzcghda.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2zruikkev.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2oehrbrzp.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2usxtprmw.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2odcehxyz.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2zecywlii.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2dldtgljq.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2gaqnpjqy.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2ntuxpqyh.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2awzwhvks.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2kwqqdimp.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2qbsrakpo.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2xcrtomce.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2hvawhplc.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2dpiwfgpg.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ajexkyix.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2hfgnbcin.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2jhriusxt.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2uqkjenai.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2srxjstke.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2uvnlbjxc.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2eflgjsyt.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2qihohzsb.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2larthwjn.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2wywjluqh.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2cehcaggt.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2aoixvwqb.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2azfcoons.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2trpqifxv.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2pbmcevwy.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2tznofjap.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2bsyeukzb.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2vftetavb.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2ojstkyyy.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2jicbfaat.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2qmtinueu.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2rghewwda.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rvxhbkkj.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2kfcfcyij.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2llgctezu.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2srgmhrmr.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2ldqzfksr.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2ihjogzwv.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2mmysjwym.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2gqktltbd.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2xbafuegk.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2cbdvqlmg.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2yshfolgq.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2ogmrhmuj.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2tcdmqnau.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2huarelic.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2bpbanlbu.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2nyeqxfft.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2lhmtgzgx.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2rlfklzfw.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2dhcsctex.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2rlshdwwq.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2difjphbw.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2iboatyvr.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2rimwsobl.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2sjgimqng.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2cruqqbne.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2kjaofksa.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2vxkelshf.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2lfrpxhmn.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2tkofggdb.html

esac
来源：http://www.52xcode.cn/Article/details/gt2egvltbmn.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2zbfipzum.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2xbxlhxjv.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2xgfwsdob.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2erzqsbrj.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2qguwyesu.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2ictfsjlv.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2ptgzyfvl.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2wofysvmh.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2bsloqxrt.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2dsbmgoli.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2jncmkooz.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2mhmysyvl.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2rvoaaxdv.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2vllbwnwe.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2avmtpxyr.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2rycuumsr.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2hjnvamzc.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2qbbsgvsn.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2duwulkhi.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2prokodut.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2lazhowev.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2gvuvikhu.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2kxudyfut.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2cqszbhqp.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2tfbslzlc.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2jykkziuv.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2gqbtovll.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2pzxixjka.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2xqkpmzoh.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2bxslkjkz.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2cbkqfhoi.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2rjhistdz.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2efyjcpbh.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2abkiabcw.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2ifeboubn.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2gujjdueq.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2chzoyfac.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2nnzpydgv.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2gfcnhqlr.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2tbjuzfxm.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2qzsslewz.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2vzvhmztx.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2mlwzhpcg.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2bybnerjy.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2lvttkwfk.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2rjpeohmd.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2tnynvdmu.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2dzqhihda.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2rjkctadz.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2fcnhjzdy.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2jhvbjhre.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2snxhrizc.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2kedjpswc.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2fanhctbh.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2pfvlwdhr.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2ewtfuijr.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2bivhuaxv.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2oxmktxrn.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2xbkvishl.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2syhrxnbn.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2abwjvhwt.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2heiaiplq.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2oqtqiryh.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2jkwifcie.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2cgiigyfz.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2hrsjdrbh.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2dhbyaigq.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2acuxrwyv.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2tarvoumo.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2zibakrnj.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2uhrxqetn.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2klwugyti.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2pwtmnwej.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2vcrwxqzn.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2ofwcijwp.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2eanvgocv.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2hulncwrd.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2vwctulrh.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2gvrwgywz.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2mubugmev.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2qikklinu.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2vzhgderh.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2zxnzgumb.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2gtmgtlmu.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2rzkacaez.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2uxirbzwn.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2odbrwusy.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2oqmvnvml.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2jzulxyyl.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2sqcieiqd.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2trqkrtmd.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2gvprwyag.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2cgdaqiej.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2frzohcbt.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2ipwgjxqp.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2ieavcqhm.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2tuazpmsd.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2aecwrdqc.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2fahmxqjm.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2fmlgbuej.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2vbkhpuhn.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2nnoxzafz.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2naoycyqz.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2gysnvvfv.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2ggccvirs.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2rcvbtmau.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2ugtluole.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2kcxemvkk.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2jpwqxjgg.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2tnxsppnl.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2ohgfxzuk.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2ubpodzax.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2dhnmoffy.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ogzjrxpw.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2fmsfqxhf.html


<!-- 参考信息 -->