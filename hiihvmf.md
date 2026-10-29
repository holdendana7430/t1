代发 wailian999

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gdrvjjjqm.sHtML

[Q28] 求和与平均
来源：http://baike.fehbvm.com/Article/details/ghowdjorp.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/gvxhsbhpt.sHtML

[Q29] 最大最小值
来源：http://www.blog.zdbjq.cn/Article/details/ghdqjnlxx.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gxqyunfnx.sHtML

[Q30] 分组统计
来源：http://www.blog.fehbvm.com/Article/details/gjkcmlgvy.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.hesvh.cn/Article/details/gwlguvozp.sHtML

[Q31] 分组后过滤
来源：http://www.share.zdbjq.cn/Article/details/gjmnijvob.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.m.share.fehbvm.com/Article/details/ggxdwnvor.sHtML

[Q32] 分组拼接字符串
来源：http://baike.hesvh.cn/Article/details/gxfxidmhy.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://baike.hesvh.cn/Article/details/glublenvn.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.share.hesvh.cn/Article/details/gvmyrjpig.sHtML

[Q33] 多列分组
来源：http://mobile.hesvh.cn/Article/details/gsuyttrlo.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.blog.fehbvm.com/Article/details/gnafuxjxs.sHtML

[Q34] 每组取第一条
来源：http://m.share.fehbvm.com/Article/details/gvijgcgir.sHtML

SELECT * FROM (
来源：http://www.blog.zdbjq.cn/Article/details/gtdkavvml.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.blog.fehbvm.com/Article/details/gmpmkqjah.sHtML

) t WHERE rn = 1;
来源：http://baike.fehbvm.com/Article/details/ghinwjfmu.sHtML

[Q35] 内连接
来源：http://wap.fehbvm.com/Article/details/gfbyusuoh.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://m.share.zdbjq.cn/Article/details/gkfqpwofg.sHtML

[Q36] 左连接
来源：http://mobile.hesvh.cn/Article/details/ggjioqyhl.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://read.share.zdbjq.cn/Article/details/gijoqlksf.sHtML

[Q37] 右连接
来源：http://wap.hesvh.cn/Article/details/gudkpjjkt.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.share.hesvh.cn/Article/details/gqnyvqtla.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://3g.zdbjq.cn/Article/details/gkeuqvrmj.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.share.zdbjq.cn/Article/details/gjmiwthbe.sHtML

[Q39] 自连接（查上下级）
来源：http://blog.fehbvm.com/Article/details/gggpstsva.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.hesvh.cn/Article/details/gvajyoyrg.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://m.share.zdbjq.cn/Article/details/gwilystff.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.zdbjq.cn/Article/details/gtibtosha.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.blog.zdbjq.cn/Article/details/gfbjyudwx.sHtML

[Q41] 多表连接
来源：http://baike.hesvh.cn/Article/details/gnhcszqhu.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://baike.zdbjq.cn/Article/details/gjsbtjjth.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.zdbjq.cn/Article/details/gmlfjzroy.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.zdbjq.cn/Article/details/gifltyjmf.sHtML

[Q42] 连接条件附加过滤
来源：http://blog.hesvh.cn/Article/details/gewpehnfn.sHtML

SELECT u.name, o.amount FROM users u
来源：http://wap.hesvh.cn/Article/details/ggpszntwa.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.hesvh.cn/Article/details/gyxhtkgts.sHtML

[Q43] 标量子查询
来源：http://read.share.zdbjq.cn/Article/details/gxdlbqngc.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.fehbvm.com/Article/details/gwjzluild.sHtML

[Q44] IN 子查询
来源：http://wap.hesvh.cn/Article/details/gcyzqtive.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://baike.hesvh.cn/Article/details/gyjqnekll.sHtML

[Q45] EXISTS 判断存在
来源：http://m.share.zdbjq.cn/Article/details/ggqrmjvwj.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.zdbjq.cn/Article/details/gfhrtzxxs.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.zdbjq.cn/Article/details/gerqrzvar.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.hesvh.cn/Article/details/gvmsrhxzm.sHtML

[Q47] 与平均值比较
来源：http://wap.zdbjq.cn/Article/details/gjxpmcmge.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://baike.zdbjq.cn/Article/details/gpamckwfz.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.zdbjq.cn/Article/details/giolbeovs.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.zdbjq.cn/Article/details/giyvrsvmd.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.blog.zdbjq.cn/Article/details/ggtnuhcuf.sHtML

[Q49] 更新单行
来源：http://mobile.zdbjq.cn/Article/details/gyprwfviq.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://blog.hesvh.cn/Article/details/gyjmbwasi.sHtML

[Q50] 批量更新
来源：http://wap.zdbjq.cn/Article/details/gsnxcsuvy.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.fehbvm.com/Article/details/gqjpninav.sHtML

[Q51] 用子查询更新
来源：http://3g.hesvh.cn/Article/details/gnvebetxy.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.blog.fehbvm.com/Article/details/ggjhotydv.sHtML

[Q52] 删除指定行
来源：http://baike.hesvh.cn/Article/details/gvsdenrym.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.zdbjq.cn/Article/details/gbhfrencv.sHtML

[Q53] 按条件删除
来源：http://baike.hesvh.cn/Article/details/gbocsbqoq.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://m.share.fehbvm.com/Article/details/gsbdvuiaw.sHtML

[Q54] 清空表
来源：http://www.blog.zdbjq.cn/Article/details/grzxgmfss.sHtML

TRUNCATE TABLE logs;
来源：http://wap.fehbvm.com/Article/details/gcjhfripd.sHtML

[Q55] 排名（并列占位）
来源：http://wap.hesvh.cn/Article/details/glmdwckcx.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.zdbjq.cn/Article/details/gxixlwtos.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.hesvh.cn/Article/details/gaindkyya.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://blog.zdbjq.cn/Article/details/gjqasvjog.sHtML

[Q57] 行号
来源：http://baike.zdbjq.cn/Article/details/gblghlnvx.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gwvfynpql.sHtML

[Q58] 累计求和
来源：http://www.m.share.fehbvm.com/Article/details/geelsmolp.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/gdvphqrqc.sHtML

[Q59] 分组内累计
来源：http://read.share.zdbjq.cn/Article/details/gvefcfngh.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gfcxgtmwb.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.fehbvm.com/Article/details/gncgroomy.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.fehbvm.com/Article/details/gxiythopp.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://baike.hesvh.cn/Article/details/gpotckerq.sHtML

[Q61] 移动平均
来源：http://www.m.share.fehbvm.com/Article/details/gkrsbaegi.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gdtfybefc.sHtML

[Q62] 分组占比
来源：http://m.share.zdbjq.cn/Article/details/gmcbkmxrb.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://read.share.fehbvm.com/Article/details/gwjdcvbxd.sHtML

[Q63] 开启事务
来源：http://m.share.hesvh.cn/Article/details/gvdkrmcwi.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://blog.zdbjq.cn/Article/details/gzrwfefqd.sHtML

[Q64] 提交事务
来源：http://www.m.share.hesvh.cn/Article/details/gscstjpjn.sHtML

COMMIT;
来源：http://m.share.hesvh.cn/Article/details/gooqcwiuk.sHtML

[Q65] 回滚事务
来源：http://mobile.hesvh.cn/Article/details/gpseewfwt.sHtML

ROLLBACK;
来源：http://www.m.share.zdbjq.cn/Article/details/gvinqhmbw.sHtML

[Q66] 行锁查询
来源：http://blog.hesvh.cn/Article/details/gkkyqmadr.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.hesvh.cn/Article/details/gmjmgadud.sHtML

[Q67] 设置隔离级别
来源：http://www.m.share.zdbjq.cn/Article/details/gcgszhkgn.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wap.zdbjq.cn/Article/details/geofqzocp.sHtML

[Q68] 保存点
来源：http://www.share.hesvh.cn/Article/details/ghwfeynly.sHtML

SAVEPOINT sp1;
来源：http://baike.fehbvm.com/Article/details/gsuzbimry.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.hesvh.cn/Article/details/grpugqqoa.sHtML

[Q69] 查看执行计划
来源：http://wap.fehbvm.com/Article/details/geliphcuu.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.hesvh.cn/Article/details/gvaltlxus.sHtML

[Q70] 更新统计信息
来源：http://www.blog.fehbvm.com/Article/details/gwomgnitf.sHtML

ANALYZE TABLE users;
来源：http://3g.zdbjq.cn/Article/details/gylyewdit.sHtML

[Q71] 查看建表语句
来源：http://blog.fehbvm.com/Article/details/gxyqbonjm.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.zdbjq.cn/Article/details/genoawxmm.sHtML

[Q72] 查看索引
来源：http://www.blog.fehbvm.com/Article/details/gepmkocni.sHtML

SHOW INDEX FROM users;
来源：http://read.share.hesvh.cn/Article/details/glaoaogzv.sHtML

[Q73] 查看表状态
来源：http://blog.hesvh.cn/Article/details/guneaigab.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.zdbjq.cn/Article/details/gqcglybgh.sHtML

[Q74] 强制使用索引
来源：http://3g.fehbvm.com/Article/details/gicrigtjf.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.zdbjq.cn/Article/details/gkavgggas.sHtML

[Q75] 日期格式化
来源：http://www.share.fehbvm.com/Article/details/gysktajrq.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.hesvh.cn/Article/details/goeugpyir.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.fehbvm.com/Article/details/gaenmybie.sHtML

[Q76] 按天统计
来源：http://mobile.zdbjq.cn/Article/details/gdnccirhj.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.fehbvm.com/Article/details/ghevczrdj.sHtML

[Q77] 时间加减
来源：http://m.share.fehbvm.com/Article/details/gkuguhtrh.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.hesvh.cn/Article/details/gliksrrzw.sHtML

[Q78] 当前时间
来源：http://baike.zdbjq.cn/Article/details/gxzespbtv.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.hesvh.cn/Article/details/guhllnere.sHtML

[Q79] 字符串拼接
来源：http://blog.hesvh.cn/Article/details/gkijdliln.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.fehbvm.com/Article/details/gaqcecwqs.sHtML

[Q80] 字符串截取
来源：http://wap.hesvh.cn/Article/details/gcpcbmmsz.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.fehbvm.com/Article/details/gzxmezizf.sHtML

[Q81] 字符串替换
来源：http://www.m.share.zdbjq.cn/Article/details/gcmbibmcp.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.zdbjq.cn/Article/details/gmtqmxjol.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.fehbvm.com/Article/details/gpubiibjj.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gpimwlhnx.sHtML

[Q83] 大小写转换
来源：http://www.blog.hesvh.cn/Article/details/guyrcezjs.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.fehbvm.com/Article/details/gbogkoyeu.sHtML

[Q84] 去除首尾空格
来源：http://www.blog.fehbvm.com/Article/details/ggmblkgfs.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.zdbjq.cn/Article/details/gnqytmwgf.sHtML

[Q85] 数值取整
来源：http://baike.zdbjq.cn/Article/details/gbydqxsxv.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.hesvh.cn/Article/details/goscqgohy.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.zdbjq.cn/Article/details/gwgrmllly.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.hesvh.cn/Article/details/guiepggkx.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.fehbvm.com/Article/details/gyqoeaeus.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.hesvh.cn/Article/details/gkbsyltke.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.share.hesvh.cn/Article/details/grgjjsyrh.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://3g.fehbvm.com/Article/details/gkvhoykad.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.hesvh.cn/Article/details/gbyosctap.sHtML

[Q89] 判断表是否存在
来源：http://wap.fehbvm.com/Article/details/gvpaddkos.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.hesvh.cn/Article/details/gyuhclvkp.sHtML

[Q90] 生成序号列
来源：http://read.share.zdbjq.cn/Article/details/gwykjlkkf.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.hesvh.cn/Article/details/gozuatvnd.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/goywxhrua.sHtML

R. Bash 专题
来源：http://www.share.fehbvm.com/Article/details/gnfbnrdsu.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gcsoewyen.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.zdbjq.cn/Article/details/gbcobfquq.sHtML

#!/usr/bin/env bash
来源：http://www.blog.fehbvm.com/Article/details/glxuslzhy.sHtML

set -euo pipefail
来源：http://www.share.hesvh.cn/Article/details/gppsnomxq.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.hesvh.cn/Article/details/gjcodaspr.sHtML

name="Tom"; echo "$name"
来源：http://read.share.hesvh.cn/Article/details/gosscnvet.sHtML

[R03] 只读变量
来源：http://m.share.zdbjq.cn/Article/details/glnbalzyh.sHtML

readonly PI=3.14
来源：http://baike.fehbvm.com/Article/details/gzrjsacew.sHtML

[R04] 位置参数
来源：http://m.share.zdbjq.cn/Article/details/gwwwrtvor.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.zdbjq.cn/Article/details/glzvpaieb.sHtML

[R05] 参数默认值
来源：http://www.share.fehbvm.com/Article/details/gmbcdfadd.sHtML

name="${1:-default}"
来源：http://wap.hesvh.cn/Article/details/glsrpioqm.sHtML

[R06] 判断命令是否存在
来源：http://baike.zdbjq.cn/Article/details/gljmuqays.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.zdbjq.cn/Article/details/gusdezinw.sHtML

[R07] if 判断文件
来源：http://3g.zdbjq.cn/Article/details/gsftkunou.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.hesvh.cn/Article/details/grpsxcxwi.sHtML

[R08] 数值比较
来源：http://www.share.hesvh.cn/Article/details/gavnqhzmi.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://mobile.zdbjq.cn/Article/details/gcpgvjqll.sHtML

[R09] 字符串比较
来源：http://wap.hesvh.cn/Article/details/goumaktcr.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.zdbjq.cn/Article/details/gokbxwpku.sHtML

[R10] 正则匹配
来源：http://read.share.fehbvm.com/Article/details/gkojjjopc.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.hesvh.cn/Article/details/grviysefu.sHtML

[R11] case 多分支
来源：http://www.m.share.zdbjq.cn/Article/details/gclrethlf.sHtML

case "$1" in
来源：http://3g.fehbvm.com/Article/details/gdodomcjq.sHtML

start) echo "启动" ;;
来源：http://www.blog.fehbvm.com/Article/details/grjatzxsn.sHtML

stop)  echo "停止" ;;
来源：http://www.share.fehbvm.com/Article/details/grsnuhyrm.sHtML

*)     echo "未知命令" ;;
来源：http://blog.hesvh.cn/Article/details/gyuywhhjr.sHtML

esac
来源：http://read.share.fehbvm.com/Article/details/gdmvoqnpx.sHtML

[R12] for 遍历文件
来源：http://wap.zdbjq.cn/Article/details/gmlnmsxlk.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.hesvh.cn/Article/details/gjnazwrbu.sHtML

[R13] for 计数循环
来源：http://www.share.hesvh.cn/Article/details/gofemcdtp.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.hesvh.cn/Article/details/gttvbkchv.sHtML

[R14] C 风格 for
来源：http://3g.fehbvm.com/Article/details/gkefwleke.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.fehbvm.com/Article/details/gjvoymbax.sHtML

[R15] while 逐行读文件
来源：http://mobile.hesvh.cn/Article/details/gaojxazfs.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.zdbjq.cn/Article/details/ggkumdxvu.sHtML

[R16] until 等待条件
来源：http://www.share.fehbvm.com/Article/details/gtcszajsa.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.fehbvm.com/Article/details/gdecahabj.sHtML

[R17] 数组定义与取值
来源：http://baike.hesvh.cn/Article/details/gypsgyrfx.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.hesvh.cn/Article/details/gwuyuqigw.sHtML

[R18] 遍历数组
来源：http://3g.zdbjq.cn/Article/details/gbhencqaq.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.zdbjq.cn/Article/details/gzljpunwn.sHtML

[R19] 数组长度
来源：http://www.blog.fehbvm.com/Article/details/gbfjlteau.sHtML

echo "${#arr[@]}"
来源：http://baike.zdbjq.cn/Article/details/gpmmhmppj.sHtML

[R20] 关联数组（字典）
来源：http://m.share.zdbjq.cn/Article/details/gxwkbxjau.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.fehbvm.com/Article/details/gplipdffb.sHtML

[R21] 字符串长度
来源：http://blog.fehbvm.com/Article/details/gfxgdwldh.sHtML

echo "${#s}"
来源：http://mobile.fehbvm.com/Article/details/grvsivbnr.sHtML

[R22] 截取子串
来源：http://mobile.fehbvm.com/Article/details/gxbozjhmw.sHtML

echo "${s:0:5}"
来源：http://www.blog.fehbvm.com/Article/details/gokugciel.sHtML

[R23] 字符串替换
来源：http://baike.fehbvm.com/Article/details/gvrmmvmwd.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.zdbjq.cn/Article/details/gpupfmjbx.sHtML

[R24] 大小写转换
来源：http://www.m.share.hesvh.cn/Article/details/grmmnsslw.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.hesvh.cn/Article/details/gqkfjmrtp.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.zdbjq.cn/Article/details/gmxjbvxge.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.fehbvm.com/Article/details/gemyhjviu.sHtML

[R26] 命令替换
来源：http://wap.hesvh.cn/Article/details/glfmuuypp.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.fehbvm.com/Article/details/gahdjhovg.sHtML

[R27] 算术展开
来源：http://www.blog.zdbjq.cn/Article/details/gspzejzzn.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.zdbjq.cn/Article/details/gwcvhsanq.sHtML

[R28] 浮点运算
来源：http://baike.zdbjq.cn/Article/details/gzrqxsafw.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.fehbvm.com/Article/details/gcyaqicwg.sHtML

[R29] 定义函数
来源：http://m.share.zdbjq.cn/Article/details/grojgzgbr.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.hesvh.cn/Article/details/gshnzgfvs.sHtML

[R30] 函数返回状态码
来源：http://blog.hesvh.cn/Article/details/gbkmqtqya.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.hesvh.cn/Article/details/gfoayhqcl.sHtML

[R31] 局部变量
来源：http://m.share.fehbvm.com/Article/details/ggxdfjkfr.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.zdbjq.cn/Article/details/gkpbpdavv.sHtML

[R32] 参数个数校验
来源：http://www.blog.hesvh.cn/Article/details/gpxnplegp.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.fehbvm.com/Article/details/gvfthhcab.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.fehbvm.com/Article/details/ghaqyuqpz.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.hesvh.cn/Article/details/ggdbxsdbt.sHtML

[R34] 退出时清理
来源：http://wap.zdbjq.cn/Article/details/gmhjkxogk.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.hesvh.cn/Article/details/gxglnvtor.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.hesvh.cn/Article/details/glvtouort.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.hesvh.cn/Article/details/gadejixyb.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.hesvh.cn/Article/details/goevxizop.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.zdbjq.cn/Article/details/gugcoimya.sHtML

[R37] 把输出赋给变量
来源：http://3g.zdbjq.cn/Article/details/gznzrreit.sHtML

files=$(ls -1)
来源：http://www.m.share.hesvh.cn/Article/details/gqakzsozf.sHtML

[R38] 管道串联
来源：http://3g.hesvh.cn/Article/details/gbwtfxbog.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.fehbvm.com/Article/details/gipejnxqy.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.zdbjq.cn/Article/details/gdakvjmsi.sHtML

cmd > out.log 2>&1
来源：http://blog.zdbjq.cn/Article/details/gkijpjhzc.sHtML

[R40] 追加写日志
来源：http://blog.zdbjq.cn/Article/details/gtvathazu.sHtML

echo "log" >> out.log
来源：http://wap.fehbvm.com/Article/details/gbjilrbhu.sHtML

[R41] 丢弃输出
来源：http://baike.hesvh.cn/Article/details/gbsfhaekx.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.zdbjq.cn/Article/details/gwaqxzfqr.sHtML

[R42] 输入重定向
来源：http://blog.fehbvm.com/Article/details/gcnxijbys.sHtML

wc -l < a.txt
来源：http://read.share.hesvh.cn/Article/details/gtqmyhotn.sHtML

[R43] 按名字查找文件
来源：http://www.share.fehbvm.com/Article/details/gadicnbrf.sHtML

find . -name "*.log" -type f
来源：http://blog.hesvh.cn/Article/details/grsjlglan.sHtML

[R44] 按修改时间查找
来源：http://3g.fehbvm.com/Article/details/gxntepozs.sHtML

find . -mtime -7 -type f
来源：http://3g.hesvh.cn/Article/details/gehysujfs.sHtML

[R45] 批量删除
来源：http://3g.fehbvm.com/Article/details/gjvmhdhfe.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.zdbjq.cn/Article/details/goqwmsifl.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.fehbvm.com/Article/details/gyttwpjvl.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.fehbvm.com/Article/details/gdniomsiq.sHtML

[R47] sed 单行替换
来源：http://3g.hesvh.cn/Article/details/geohardzp.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.hesvh.cn/Article/details/ggnrzgvlb.sHtML

[R48] awk 取指定列
来源：http://mobile.fehbvm.com/Article/details/gxyxhjvro.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gfiiptvdr.sHtML

[R49] awk 带条件
来源：http://www.m.share.zdbjq.cn/Article/details/gywujjqcc.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.fehbvm.com/Article/details/gphhfaaws.sHtML

[R50] awk 求和
来源：http://m.share.hesvh.cn/Article/details/gfxfbtjrz.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.hesvh.cn/Article/details/guhoddoto.sHtML

[R51] 排序去重取前几
来源：http://www.share.hesvh.cn/Article/details/ghylrfhzz.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.fehbvm.com/Article/details/gpwddczqt.sHtML

[R52] 统计行数
来源：http://www.m.share.hesvh.cn/Article/details/gdfxklarr.sHtML

wc -l a.txt
来源：http://wap.hesvh.cn/Article/details/ghlyjyktp.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.hesvh.cn/Article/details/geyhuhmzc.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.hesvh.cn/Article/details/gogbkrizj.sHtML

[R54] 比较两个文件
来源：http://blog.fehbvm.com/Article/details/gpncafswj.sHtML

diff a.txt b.txt
来源：http://www.m.share.fehbvm.com/Article/details/gennddfqa.sHtML

[R55] 压缩与解压
来源：http://www.m.share.zdbjq.cn/Article/details/gboxqmohy.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.fehbvm.com/Article/details/gvxsmjnqf.sHtML

[R56] 远程拷贝
来源：http://www.m.share.zdbjq.cn/Article/details/goeyfhxpw.sHtML

scp file user@host:/path/
来源：http://www.m.share.zdbjq.cn/Article/details/ghfvkfzjv.sHtML

[R57] 远程执行命令
来源：http://wap.hesvh.cn/Article/details/gpazckhpo.sHtML

ssh user@host 'uptime'
来源：http://mobile.zdbjq.cn/Article/details/glisrxvol.sHtML

[R58] 下载文件
来源：http://wap.zdbjq.cn/Article/details/gatrkgtxd.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.hesvh.cn/Article/details/gbiygmkba.sHtML

[R59] 发 POST JSON
来源：http://3g.hesvh.cn/Article/details/gutqeedbt.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.fehbvm.com/Article/details/gsdaqekwe.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.fehbvm.com/Article/details/gkzdtfriz.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.fehbvm.com/Article/details/gqppkyzlf.sHtML

[R61] 磁盘占用
来源：http://m.share.hesvh.cn/Article/details/gvtfmhnnr.sHtML

df -h;  du -sh *
来源：http://www.blog.zdbjq.cn/Article/details/gjsemzdei.sHtML

[R62] 找最占空间的文件
来源：http://3g.fehbvm.com/Article/details/gluvffadw.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.fehbvm.com/Article/details/gtjojwsvy.sHtML

[R63] 内存与进程
来源：http://www.blog.zdbjq.cn/Article/details/gxqokqcnp.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.zdbjq.cn/Article/details/ghmkyujqr.sHtML

[R64] 结束进程
来源：http://www.share.hesvh.cn/Article/details/ggnxnvchs.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.hesvh.cn/Article/details/gbjargnag.sHtML

[R65] 查看端口占用
来源：http://3g.fehbvm.com/Article/details/gwywynnch.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.hesvh.cn/Article/details/gfttyjzkv.sHtML

[R66] 定时任务
来源：http://baike.hesvh.cn/Article/details/goasbwfec.sHtML

crontab -e;  crontab -l
来源：http://www.share.zdbjq.cn/Article/details/grkpjgzou.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.hesvh.cn/Article/details/gpqjepotm.sHtML

openssl rand -hex 16
来源：http://www.m.share.hesvh.cn/Article/details/gsfswxofz.sHtML

[R68] 计算文件校验值
来源：http://read.share.hesvh.cn/Article/details/gtgptncus.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.zdbjq.cn/Article/details/goqtwivzo.sHtML

[R69] 生成随机密码
来源：http://wap.zdbjq.cn/Article/details/gezcatlhb.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.hesvh.cn/Article/details/gcnstikxi.sHtML

[R70] 时间戳与互转
来源：http://read.share.fehbvm.com/Article/details/gvnmdkpis.sHtML

date +%s;  date -d @1700000000
来源：http://wap.hesvh.cn/Article/details/gheptnyhw.sHtML

[R71] 日期格式化
来源：http://www.blog.zdbjq.cn/Article/details/gzehpoihh.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.fehbvm.com/Article/details/gsghdgmnm.sHtML

[R72] 等待端口就绪
来源：http://3g.hesvh.cn/Article/details/guqqzgjsy.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.hesvh.cn/Article/details/govgfmsga.sHtML

[R73] 分割大日志
来源：http://mobile.hesvh.cn/Article/details/gcskkgial.sHtML

split -l 1000 big.log part_
来源：http://3g.zdbjq.cn/Article/details/ghlipscpi.sHtML

[R74] 批量重命名
来源：http://baike.fehbvm.com/Article/details/glwxtsqob.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.zdbjq.cn/Article/details/gytewlfgy.sHtML

[R75] 导出环境变量
来源：http://wap.zdbjq.cn/Article/details/gjdsmxhan.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.fehbvm.com/Article/details/gofpeyzlc.sHtML

[R76] 使用临时文件
来源：http://baike.zdbjq.cn/Article/details/gexeknzqf.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fehbvm.com/Article/details/gpwsvmkhg.sHtML

[R77] 读取用户输入
来源：http://mobile.zdbjq.cn/Article/details/guinqbfle.sHtML


<!-- 参考信息 -->