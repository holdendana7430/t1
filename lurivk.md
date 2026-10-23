代发 wailian999

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3lwwnbjee.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3woomrgkp.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3mrvzmzlf.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3elxoajgz.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3tmggjljh.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3rvicxlgm.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3gglduczb.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3mcfjcygo.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3gfcxnnwo.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3bnygsush.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3iclcuopp.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3ebcthpjf.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3epuuztli.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3eqxucmoa.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3cbzcexec.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3vewlkknc.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ipcbwlbv.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3vlstjbzr.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ccjzhrvi.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3ckrpsufj.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3iqftrfvg.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3gyqorbmy.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3kgxsgbek.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3sfagjarj.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3hyjgpmwp.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3evromxee.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3ujednbsh.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3xphnuthe.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3aexmbfnd.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3qlqfpmwj.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3wzxdfkcz.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3wiylylue.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3igatfoms.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ujlnbbxe.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3qkyfxsor.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3hluapfem.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3deybxflb.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3bsahovlk.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3vqfckqgh.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3hrybbako.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3mtqmkjff.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3pvdhejgg.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3kjsufrcr.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3wlhjbzei.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3drqkvmxq.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3crrkgcnq.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3jxehamye.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3xatdhyiz.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3qxxygxvv.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3grkvxqhr.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3dmbitabr.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3nzqhphlu.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3vsnjrhwe.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3ynwtnywt.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3ryqwdixi.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3enmagywl.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3uhoulpja.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3dqzefrjc.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3zgsieyco.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3ptbzbmws.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3afsnkkny.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3xggbudyg.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3ermqlssy.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3uyafdjpd.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3aqkrslqb.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3ltwxomim.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3wouxqros.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3uyssdonw.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3xekcjnjn.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3dwidakrh.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3jkygeqla.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3zjzdxioq.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3mshbuyti.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3zmvurubw.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3unciwtyx.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3lyzwbbqo.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3eybsbbtz.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3azthvjdb.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3xoocpbva.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3sdpkqjog.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3knounbtl.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3zhubextz.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3podaeylf.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3ppflckfk.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3dfimfycq.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3rvkckvpw.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3cofkbgwh.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3jtyosdue.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3jzmoaqfl.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3ijwdzvko.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3liewuqod.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3hildzkpw.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3sgxpxlmh.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3ilnimtff.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3khkqrtst.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3chagxjbt.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3nghjvqqw.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3grdyiyus.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3mkhwquay.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3knbdsemp.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3cnfvopwj.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3wmoorfws.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3ugivfkpw.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3xoavixgi.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3zmmyisdc.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3bwvxtjoi.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3ubcpgtye.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3jsjyjcgx.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3karxmevs.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3gstpjewo.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3tfprcjsk.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3hdjfvpqu.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3xvgfxmyj.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3olrhawwo.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3lmubssut.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3tbyuabkd.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3wmdlkaut.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3gyyvbyyt.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3bggdukjh.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3rwixtlho.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3ounzdvde.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3mqexemlu.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3rpvftsfq.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3uvhdmijj.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3hyamrnoa.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3adkaeljn.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3zmdfedmg.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3pnfxzuxu.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3ilsfbjnk.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3taxotnus.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3glpcadxh.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3qumtbnig.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3obtopuxl.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3hpfmpbxd.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3hiwbemqp.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3zbwzaner.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3gsagckqf.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ckqtqgem.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3ajecbnnd.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3fggarunh.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3mdwcmjqt.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3rqrocxqj.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3wzbuvdut.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3ovhnweng.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3lptdtxlq.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3hkueybbe.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3xffcvwid.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3vztmuhjv.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3lmvqobwj.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3jrwxkicz.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3htozgypr.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3kcnowxfe.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3fgdaylwm.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3qewdbwwk.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3sjjrdios.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zguvhlum.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3shhcfkib.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zgbyboii.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3aujxaerr.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3xxdjftgm.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3eidnftzh.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3qklhkduc.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3ukxikgio.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3uwulross.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3cnqfvmep.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3pfqwiqen.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3jpyfiulh.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3gcfhksaf.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3fjhztnzt.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3ygwzdpav.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3rvzfekbr.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3yefwnefd.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3wacdlbyi.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3rgpsgzhi.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3rocwqlhl.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3rnkvaumz.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3mugrxltm.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3wqcmfstg.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3dbnydeww.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3pvkwrvzd.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3bwqircgl.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3mvfsagho.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3fmfyiznn.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3kwctzopn.html

esac
来源：http://www.52xcode.cn/Article/details/gt3oivnsxie.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3pzzccard.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3mgtcjsjy.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3jnpiwjup.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3afvouqek.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3pliewxtp.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3izhmulig.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3dogndqvu.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3mapdjbjs.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3boilxrrc.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3baxgzxih.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3ltimbysa.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3asroouce.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3xqgmtahx.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3vihqliew.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3lqdwxpwm.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3rzktxitm.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3uzkdpiml.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3bsdvcztq.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3ankzogri.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3ghrozeef.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3rcnvtcqi.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3uxtckctk.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3fbtqpxvy.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3tjkwfstd.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3afpgbrih.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3cglzfivn.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3qwcgorgj.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3vktutmen.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3ngedetcz.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3mkjsbvkg.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3mpadaunq.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3zvioivlb.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3nvdbcrmv.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3lhxxilsi.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3sovpwjbi.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3rzomtroc.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3aldngokr.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3lgxpnoqj.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3rsdffjvv.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3raxbvkxu.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3sojpchsx.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3qvvlsmow.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3misahwvb.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3kpuypymh.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3ovjwzprt.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3hzbyklfh.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3qxvkvaxm.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3ljphdvox.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3cxowdisj.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3lybszacl.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3ccrvgumv.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3octcdzat.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3eufqiamp.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3ycjmmryc.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3rgnptzas.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3pxnvbtlb.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3pqoarnwr.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3nebtrvnk.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3hoeqjmcz.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3zfahawne.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3jsuwlszt.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3angodhpw.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3gveskycp.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3uanfmcts.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3mvybjhge.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3aktmnygv.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3gmkhqeps.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3enwtilea.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3ghcxdovw.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3jmsmorpy.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3cyioaqiw.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3csxtoqkg.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3zwtqgzjd.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ccphrgxh.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3diqfurqq.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3asxjtpjr.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3zirmzula.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3lkhslrsk.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3pfunsapn.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3debabwpw.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3kxmwqjvn.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3enmoxkuv.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3redmbaai.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3niyjptma.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3ddboboik.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3qxrxppkq.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3qmydwglj.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3slnhnplr.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3fahignvu.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3bpiiogow.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3kmovnple.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3jokzmwtt.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3dratxqjl.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3ryruqlqs.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3tydxocaq.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3vehiuptt.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3ckwaufbn.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3dtfmhfuh.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3mgiqmkyt.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3lnjesuyj.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3zhtehfxj.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3emxxttgx.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3lwvyanfj.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3sdkpxvqp.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3lvindyuj.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3ddqfsvry.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3hwcmpzic.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3hadwihkr.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3dzyhhxic.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3hpgaiyit.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3xvnggbbb.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3cfzaftwu.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3ziilddbm.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3gewplpdm.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3hzaymfba.html


<!-- 参考信息 -->