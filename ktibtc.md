代发 wailian999

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2yikgnaux.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2oydpeqnj.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2fazzgdry.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2jrbskvdt.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2niwodzul.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2vvvdcllj.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2rdknzzes.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2nrddkzed.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2zdxsobfd.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2tcczltcu.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2wxuzmjfk.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2tiqdftal.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2bquyetmv.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2jtopejah.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2ephprmlg.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2dknhkgsa.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2fskylwef.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2sxfhnwgr.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2krsrwcou.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2wcdnvgml.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2njcbvetw.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2wgpcbakq.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ajzqcrmk.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2lsebwwvv.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2lmzxirez.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2rrrfxifn.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2amlydkwe.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2rhgqfoin.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2uhcspthf.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2mvoqrpdg.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2idwkrnlh.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2cxesnsrl.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2dkfqbzdz.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2yjficqeo.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2nclhzxen.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2lnqkrspb.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2cqysvkyc.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2vatjbrzu.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2wtuhetsq.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2sganbfji.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2celpyxwf.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2jdwbuakv.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2visdrjtb.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2fwbofmoa.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2cjjgxorq.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2gdilhzsd.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2gxzmlsqa.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2pacgfwdo.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2iutpctyx.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2vyetcjhz.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2zqefhkna.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2jovjcssv.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2dbffswpc.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2hdqzylkk.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2rbpfvyan.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2dvjbegwd.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2ntuadmap.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2noqsjqji.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2znvtfhto.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2eszjnblw.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2qozbtjtq.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2kbnlpnsr.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2idpcjkkp.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2xuwlegsy.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2mnzfetdj.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2rulwnozb.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2nhnbmpxl.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2ffvkxlxq.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2hqdchano.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2acjgkkyi.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2fbwccong.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2gmcyaepe.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2sknsvwus.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2vnuetwly.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2ldllmvcq.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2dyohduvn.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2ljprpilo.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2ablrmcwj.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2tuaclvjl.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2ilfzqkhe.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2mbvwhwnz.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2vademyav.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2ricwsobc.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2vrqlldkd.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2mtuhgoid.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2biltfxau.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2xfkgndkf.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2mfgdfhet.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2odokhrha.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2dhbnpydr.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2wccznlfc.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2znwkvumf.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ajusoftu.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2nkcexuez.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2infjuaar.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2wchcdnoa.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ejacqerp.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2onqtlpik.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2tmubugvk.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2uchsmrat.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2sohcehdn.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2uyugxjic.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2hbkqyldi.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2tqnfbufi.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2iupajqrd.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2elaaxcxd.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2kaljkpnv.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2glekwkja.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2qjcwgnhp.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2tcbmnrya.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2eumazjvm.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2gkknnuvv.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2iannslth.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2zfloesnj.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2ngwpnvqf.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2grsltaee.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2ktlaracc.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2pcplvxta.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2hhtjmpad.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2jebwbdmp.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2cyphftqa.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2jhcapylm.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2bkhjerut.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2dqfmscbq.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2vhqdlbkc.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2wbizmszd.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2rsrhhcut.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2bpwojjgf.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2jgluvhhs.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2vnockdfd.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2xumtvnrz.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2igqhcdan.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2mazshyyn.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2rpncsujb.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2xuvuqymt.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2jtgjfeoo.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2qxpxdijv.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2mxyrrzcs.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2lknjjkzm.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2oyuldksd.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2opygnmae.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2anpgtnif.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2isktyhus.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2dujoycme.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2zqslcsvq.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2twhbrhmf.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2cmgjivop.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2akznnoxj.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2uvruqaas.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2xuvlakte.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2mnbrsnyn.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2qtkbcwgq.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2oxdpjrcc.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2btslkjxd.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2smcxisrz.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2nreufaxm.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2lntnjbug.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2flgefboj.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2fvmvdhet.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2ymxeyvin.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2ocfijnjg.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2qiknaxer.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2spgiojqj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rppkjgpc.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2hdudafll.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2iwsfnvkl.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2jjqbgkhx.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2locvswxe.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2ayuckcuc.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2rndtclbc.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2mzxorodd.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2nbmwwojc.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2cvxxagnk.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2kvmopsac.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2bklhbvjp.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2fzlptyfj.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2ytlvgave.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2ptjpbkvx.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2hhfnsowh.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2awprvmhn.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2pqweficj.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2kmduhcet.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2trvixvkn.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2sohwbytf.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2hgyqyaym.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2jrecehfs.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2wycyknnx.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2jmfccxqv.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2qduaokid.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2uqawqahp.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2sexphpow.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2fnvqmpap.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2fjfwzrlf.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2amuyyirb.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2fghwhisn.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2vbbyyadt.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2xlrklpoc.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2moqgoyep.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2uetpbwkt.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2zbfqanjt.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2fycyjfdt.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2khgndxoh.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2ekfxrxdr.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2odphitua.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2temnslbl.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2xtupkkuu.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2rzkmjnsy.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2iokoxeks.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2qphfkqmf.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2jrvluspe.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2jmwvaqlr.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2kcjpawvy.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2kinkmald.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2lgipejzy.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2jjopospm.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2slnqjkwx.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2cdafvstq.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2qgvsoxqq.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2ulzeooff.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2bpclksvs.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2orbmjvcm.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2xvddlfrn.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2ymwxntjq.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2fmtjkxmt.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2yubkuicv.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2bmiuonqd.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2cnocixkl.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2dbepsmkb.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2ztcozydk.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2ftkvudbj.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2hbkbssbj.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2eresedqw.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2mefbohdl.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2gddihlxr.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2ibpczdfz.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2xzhqoznp.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2lsglrkoh.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2dbuicotg.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2guwmdgsc.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2kfwpkckv.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2usqukpuz.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2joenmeof.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2abvjteao.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2dncqbmvc.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2kyfhwzzj.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2jbhywhiw.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2mqdasrow.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2luhlgkio.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2sojzhozc.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2simefqjf.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2dwmiaxsd.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2dgqqeprc.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2asizwpgg.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2gqtxlnyq.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ndnfcjwp.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2dpqalzrh.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2vxwkwmvu.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2lwcdbiuo.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2zjdjvwhd.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2stxcflof.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2dthstuyo.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2fjsnconx.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2pxinkdqn.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2ftodwbbv.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2hibdsgvx.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2aufqegcy.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2nymckxkf.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2ncwisakh.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2vylaxxwg.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2tycjzycy.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2vyqibqjq.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2oklrjdnj.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2qpuzhqsc.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2nuufklks.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2vnfozvcd.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2lhjwwwbp.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2jeggbpui.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2weqnqsdd.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2zpnayrzz.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2tztdukgn.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2tiqloioy.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2mxoqltfx.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2nelolecs.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2rqhywsbj.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2nhqfoaet.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2zekivwca.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2zyuxyiir.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2ajapzlfv.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2stvfvphj.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2hnfripgr.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2vuifvixi.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2bzdgihlf.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2jvosmmga.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2tkpkdcvr.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2ksnvtfzo.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2ncfyzovj.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2juivyttj.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2chjhapux.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2uqldkigs.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2gifbveet.html


<!-- 参考信息 -->