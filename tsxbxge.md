代发 wailian999

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://m.share.hesvh.cn/Article/details/gmrxxxqki.sHtML

[Q28] 求和与平均
来源：http://blog.zdbjq.cn/Article/details/gjaidaojg.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/gexwrhfmw.sHtML

[Q29] 最大最小值
来源：http://mobile.fehbvm.com/Article/details/glthjebpr.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://wap.fehbvm.com/Article/details/gdltosysd.sHtML

[Q30] 分组统计
来源：http://m.share.hesvh.cn/Article/details/grpgqggcr.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://read.share.zdbjq.cn/Article/details/gwqoaprrb.sHtML

[Q31] 分组后过滤
来源：http://wap.hesvh.cn/Article/details/gmnbelkbx.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.blog.hesvh.cn/Article/details/gwdvsguow.sHtML

[Q32] 分组拼接字符串
来源：http://www.share.hesvh.cn/Article/details/gcxdtaxsn.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.blog.zdbjq.cn/Article/details/gyxpdcnjo.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.zdbjq.cn/Article/details/glbtnynul.sHtML

[Q33] 多列分组
来源：http://www.blog.fehbvm.com/Article/details/goczvsmuy.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://blog.hesvh.cn/Article/details/giheepmcw.sHtML

[Q34] 每组取第一条
来源：http://3g.fehbvm.com/Article/details/gbesxgflq.sHtML

SELECT * FROM (
来源：http://www.m.share.hesvh.cn/Article/details/gmbwlpzqq.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.m.share.hesvh.cn/Article/details/galnnvcbh.sHtML

) t WHERE rn = 1;
来源：http://read.share.hesvh.cn/Article/details/gvartebid.sHtML

[Q35] 内连接
来源：http://www.share.hesvh.cn/Article/details/gfpudimss.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.fehbvm.com/Article/details/gylplxcma.sHtML

[Q36] 左连接
来源：http://read.share.zdbjq.cn/Article/details/gpzomldcw.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mobile.hesvh.cn/Article/details/gxyiybyjw.sHtML

[Q37] 右连接
来源：http://blog.hesvh.cn/Article/details/gcuzrjdzb.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://read.share.fehbvm.com/Article/details/grzgievcs.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://wap.hesvh.cn/Article/details/gljysexaq.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://baike.zdbjq.cn/Article/details/grlwvdkia.sHtML

[Q39] 自连接（查上下级）
来源：http://read.share.zdbjq.cn/Article/details/gyrqqvesf.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://baike.hesvh.cn/Article/details/glqbdhxld.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.hesvh.cn/Article/details/gzrlibqmx.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://m.share.hesvh.cn/Article/details/gfsmlphtv.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://m.share.fehbvm.com/Article/details/gewnkvjdw.sHtML

[Q41] 多表连接
来源：http://www.blog.zdbjq.cn/Article/details/gvhzhfden.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://m.share.zdbjq.cn/Article/details/gnxrglder.sHtML

JOIN users u ON u.id = o.user_id
来源：http://baike.hesvh.cn/Article/details/gfekhmuxr.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.fehbvm.com/Article/details/gcvyevxgm.sHtML

[Q42] 连接条件附加过滤
来源：http://www.blog.hesvh.cn/Article/details/gcepjjeoe.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.blog.hesvh.cn/Article/details/glzsymhxg.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.hesvh.cn/Article/details/gcgsktwvo.sHtML

[Q43] 标量子查询
来源：http://baike.fehbvm.com/Article/details/gxwjkeqdh.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wap.zdbjq.cn/Article/details/gjlpdorig.sHtML

[Q44] IN 子查询
来源：http://wap.fehbvm.com/Article/details/gxnufktlj.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mobile.fehbvm.com/Article/details/gvouiryvm.sHtML

[Q45] EXISTS 判断存在
来源：http://blog.zdbjq.cn/Article/details/grbhdilrv.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.fehbvm.com/Article/details/ghvtxrbwk.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.blog.fehbvm.com/Article/details/ggcqgyvrw.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.zdbjq.cn/Article/details/gfgjrqmqq.sHtML

[Q47] 与平均值比较
来源：http://read.share.zdbjq.cn/Article/details/gixwgphwv.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://m.share.zdbjq.cn/Article/details/gsintrwnd.sHtML

[Q48] CTE 公用表表达式
来源：http://baike.hesvh.cn/Article/details/grvqexzmb.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.share.fehbvm.com/Article/details/gmjtiqyur.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://mobile.hesvh.cn/Article/details/gpwzlcofh.sHtML

[Q49] 更新单行
来源：http://www.share.hesvh.cn/Article/details/gbzywuamd.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.hesvh.cn/Article/details/gpuqiclib.sHtML

[Q50] 批量更新
来源：http://mobile.hesvh.cn/Article/details/gsjawcian.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.fehbvm.com/Article/details/gtgitlgpa.sHtML

[Q51] 用子查询更新
来源：http://read.share.zdbjq.cn/Article/details/ggcibumpp.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.zdbjq.cn/Article/details/gznfksuck.sHtML

[Q52] 删除指定行
来源：http://www.share.hesvh.cn/Article/details/ghikvvldx.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.blog.zdbjq.cn/Article/details/gfypxrmha.sHtML

[Q53] 按条件删除
来源：http://read.share.fehbvm.com/Article/details/ghqellpwc.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.fehbvm.com/Article/details/gcphizbjs.sHtML

[Q54] 清空表
来源：http://blog.fehbvm.com/Article/details/grvskriab.sHtML

TRUNCATE TABLE logs;
来源：http://www.blog.zdbjq.cn/Article/details/gnadyxaek.sHtML

[Q55] 排名（并列占位）
来源：http://3g.hesvh.cn/Article/details/gcjwtbazk.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://m.share.hesvh.cn/Article/details/gyloepdhi.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.fehbvm.com/Article/details/guioovnli.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://baike.zdbjq.cn/Article/details/gswkkignd.sHtML

[Q57] 行号
来源：http://blog.fehbvm.com/Article/details/gfahwpgnc.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.zdbjq.cn/Article/details/gyviqvloe.sHtML

[Q58] 累计求和
来源：http://read.share.hesvh.cn/Article/details/glhtwnvbs.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://blog.zdbjq.cn/Article/details/grystpuen.sHtML

[Q59] 分组内累计
来源：http://www.share.fehbvm.com/Article/details/gzrxzflwl.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/ganumxvxm.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.hesvh.cn/Article/details/gyotjeims.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://baike.hesvh.cn/Article/details/getiklqio.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://baike.hesvh.cn/Article/details/ghfilsenw.sHtML

[Q61] 移动平均
来源：http://blog.fehbvm.com/Article/details/gcvnbzebr.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/gqfkomsml.sHtML

[Q62] 分组占比
来源：http://3g.fehbvm.com/Article/details/gglljjzxz.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://m.share.zdbjq.cn/Article/details/gtwkdiaje.sHtML

[Q63] 开启事务
来源：http://wap.fehbvm.com/Article/details/gyswjutto.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.fehbvm.com/Article/details/goinckhts.sHtML

[Q64] 提交事务
来源：http://blog.fehbvm.com/Article/details/goabovdhz.sHtML

COMMIT;
来源：http://www.m.share.zdbjq.cn/Article/details/gxuhfunsg.sHtML

[Q65] 回滚事务
来源：http://blog.zdbjq.cn/Article/details/grixdcawp.sHtML

ROLLBACK;
来源：http://blog.zdbjq.cn/Article/details/gwnchrgnj.sHtML

[Q66] 行锁查询
来源：http://blog.hesvh.cn/Article/details/ggaccextm.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://blog.hesvh.cn/Article/details/gmkruzxsj.sHtML

[Q67] 设置隔离级别
来源：http://mobile.zdbjq.cn/Article/details/gruijoobr.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.zdbjq.cn/Article/details/gbwmwkmnk.sHtML

[Q68] 保存点
来源：http://www.m.share.zdbjq.cn/Article/details/gecgjzlhq.sHtML

SAVEPOINT sp1;
来源：http://mobile.hesvh.cn/Article/details/ghewdldys.sHtML

ROLLBACK TO sp1;
来源：http://blog.zdbjq.cn/Article/details/gzcvcklwi.sHtML

[Q69] 查看执行计划
来源：http://baike.hesvh.cn/Article/details/gpgkihodv.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.fehbvm.com/Article/details/gxkjbmlfm.sHtML

[Q70] 更新统计信息
来源：http://www.blog.hesvh.cn/Article/details/gipronuca.sHtML

ANALYZE TABLE users;
来源：http://3g.fehbvm.com/Article/details/gmscumwla.sHtML

[Q71] 查看建表语句
来源：http://www.share.hesvh.cn/Article/details/gnomihbux.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.fehbvm.com/Article/details/gfwcmwhhz.sHtML

[Q72] 查看索引
来源：http://3g.fehbvm.com/Article/details/gxugllszw.sHtML

SHOW INDEX FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gxzmcgheg.sHtML

[Q73] 查看表状态
来源：http://www.share.fehbvm.com/Article/details/glkcllxbp.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.fehbvm.com/Article/details/gqhsryxxo.sHtML

[Q74] 强制使用索引
来源：http://www.m.share.fehbvm.com/Article/details/gytkllxmx.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.zdbjq.cn/Article/details/gwxjhjlqh.sHtML

[Q75] 日期格式化
来源：http://www.share.hesvh.cn/Article/details/gxfgrphnl.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://m.share.hesvh.cn/Article/details/gxdyhrycy.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.fehbvm.com/Article/details/gnwdieweu.sHtML

[Q76] 按天统计
来源：http://3g.zdbjq.cn/Article/details/gkwpctbcu.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.hesvh.cn/Article/details/gaysubowl.sHtML

[Q77] 时间加减
来源：http://www.blog.hesvh.cn/Article/details/givkizucw.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.zdbjq.cn/Article/details/gvxoijixd.sHtML

[Q78] 当前时间
来源：http://www.m.share.fehbvm.com/Article/details/gtxghpxma.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.fehbvm.com/Article/details/ghtkeobxf.sHtML

[Q79] 字符串拼接
来源：http://www.blog.hesvh.cn/Article/details/glarvdyxi.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.fehbvm.com/Article/details/grozblzuu.sHtML

[Q80] 字符串截取
来源：http://wap.zdbjq.cn/Article/details/gxbwqpeha.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mobile.fehbvm.com/Article/details/gmexefynt.sHtML

[Q81] 字符串替换
来源：http://wap.fehbvm.com/Article/details/gsesidycx.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.zdbjq.cn/Article/details/gszwvrtgy.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.zdbjq.cn/Article/details/gosobuljn.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gfebokgjs.sHtML

[Q83] 大小写转换
来源：http://www.m.share.hesvh.cn/Article/details/goikdjjfj.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.hesvh.cn/Article/details/gslnjvnxs.sHtML

[Q84] 去除首尾空格
来源：http://3g.fehbvm.com/Article/details/gpfzewsez.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.zdbjq.cn/Article/details/gohauujfb.sHtML

[Q85] 数值取整
来源：http://3g.fehbvm.com/Article/details/ggoievzya.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.fehbvm.com/Article/details/gbgsvbvra.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.fehbvm.com/Article/details/ghxythgqv.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.fehbvm.com/Article/details/gjcwmccor.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.fehbvm.com/Article/details/ghsemxttj.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.zdbjq.cn/Article/details/gmzyoenit.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.hesvh.cn/Article/details/gnwofkhbv.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://3g.hesvh.cn/Article/details/gainnvnln.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.zdbjq.cn/Article/details/ghasxxjtu.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.hesvh.cn/Article/details/gvapghlek.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.fehbvm.com/Article/details/gomuffldz.sHtML

[Q90] 生成序号列
来源：http://www.m.share.fehbvm.com/Article/details/gtobaayca.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.fehbvm.com/Article/details/gxxmhhywr.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gwxqoddzi.sHtML

R. Bash 专题
来源：http://mobile.fehbvm.com/Article/details/ghziviond.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gerxdklum.sHtML

[R01] shebang 与严格模式
来源：http://wap.zdbjq.cn/Article/details/gdtmmzmyb.sHtML

#!/usr/bin/env bash
来源：http://www.share.zdbjq.cn/Article/details/gddfepxip.sHtML

set -euo pipefail
来源：http://wap.fehbvm.com/Article/details/ghkqkzses.sHtML

[R02] 变量赋值与使用
来源：http://baike.zdbjq.cn/Article/details/ghlcmhojf.sHtML

name="Tom"; echo "$name"
来源：http://mobile.zdbjq.cn/Article/details/gnybqizmg.sHtML

[R03] 只读变量
来源：http://read.share.zdbjq.cn/Article/details/gfupucnek.sHtML

readonly PI=3.14
来源：http://3g.fehbvm.com/Article/details/gupnsffcy.sHtML

[R04] 位置参数
来源：http://www.share.fehbvm.com/Article/details/gbysxsgwc.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.zdbjq.cn/Article/details/gqryynjul.sHtML

[R05] 参数默认值
来源：http://mobile.hesvh.cn/Article/details/gcndkefge.sHtML

name="${1:-default}"
来源：http://www.m.share.fehbvm.com/Article/details/gcgtuaxtt.sHtML

[R06] 判断命令是否存在
来源：http://read.share.fehbvm.com/Article/details/gnuzlflan.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.hesvh.cn/Article/details/goavkajyk.sHtML

[R07] if 判断文件
来源：http://read.share.hesvh.cn/Article/details/gfgdlpido.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.fehbvm.com/Article/details/gcvaseymx.sHtML

[R08] 数值比较
来源：http://read.share.fehbvm.com/Article/details/gubniynyr.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.fehbvm.com/Article/details/gzdjnupnh.sHtML

[R09] 字符串比较
来源：http://wap.zdbjq.cn/Article/details/gvswfmcya.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.fehbvm.com/Article/details/goxidncxg.sHtML

[R10] 正则匹配
来源：http://www.share.fehbvm.com/Article/details/ghwwropfi.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.zdbjq.cn/Article/details/gjfiuxxfb.sHtML

[R11] case 多分支
来源：http://m.share.fehbvm.com/Article/details/gacvhgocy.sHtML

case "$1" in
来源：http://www.blog.hesvh.cn/Article/details/gvcnxtufe.sHtML

start) echo "启动" ;;
来源：http://baike.fehbvm.com/Article/details/gdunmxagx.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.zdbjq.cn/Article/details/govwzxnhn.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.zdbjq.cn/Article/details/grrljgdtu.sHtML

esac
来源：http://www.share.zdbjq.cn/Article/details/gpajgbmko.sHtML

[R12] for 遍历文件
来源：http://m.share.zdbjq.cn/Article/details/gxmqutaqx.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.hesvh.cn/Article/details/gphcvcoxp.sHtML

[R13] for 计数循环
来源：http://3g.zdbjq.cn/Article/details/gxahyofua.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.zdbjq.cn/Article/details/gkswbgjcr.sHtML

[R14] C 风格 for
来源：http://read.share.hesvh.cn/Article/details/gclwgiwxf.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.fehbvm.com/Article/details/gufdtwcfx.sHtML

[R15] while 逐行读文件
来源：http://www.blog.zdbjq.cn/Article/details/gwbeiasiv.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.zdbjq.cn/Article/details/gsmokyxvd.sHtML

[R16] until 等待条件
来源：http://blog.zdbjq.cn/Article/details/giuwxeqwc.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.hesvh.cn/Article/details/gpakzlynd.sHtML

[R17] 数组定义与取值
来源：http://read.share.hesvh.cn/Article/details/gfpelszhz.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.fehbvm.com/Article/details/gkooqknnb.sHtML

[R18] 遍历数组
来源：http://blog.zdbjq.cn/Article/details/gvsrxlybg.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.hesvh.cn/Article/details/gxeolkahy.sHtML

[R19] 数组长度
来源：http://3g.zdbjq.cn/Article/details/gzcchuzci.sHtML

echo "${#arr[@]}"
来源：http://wap.hesvh.cn/Article/details/ghefshotq.sHtML

[R20] 关联数组（字典）
来源：http://blog.zdbjq.cn/Article/details/gvflqbhgv.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.zdbjq.cn/Article/details/gqsjzkhra.sHtML

[R21] 字符串长度
来源：http://mobile.hesvh.cn/Article/details/gdtojztmv.sHtML

echo "${#s}"
来源：http://www.m.share.zdbjq.cn/Article/details/ggjvxsjno.sHtML

[R22] 截取子串
来源：http://wap.hesvh.cn/Article/details/gtpdmuplo.sHtML

echo "${s:0:5}"
来源：http://m.share.fehbvm.com/Article/details/gjxhsqtuk.sHtML

[R23] 字符串替换
来源：http://www.blog.hesvh.cn/Article/details/gxocibhwd.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.fehbvm.com/Article/details/ggubobrpn.sHtML

[R24] 大小写转换
来源：http://wap.zdbjq.cn/Article/details/gecctcdjg.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.hesvh.cn/Article/details/goepmhojp.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.zdbjq.cn/Article/details/gwhnsggps.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.hesvh.cn/Article/details/gvletfuci.sHtML

[R26] 命令替换
来源：http://www.m.share.fehbvm.com/Article/details/gonipbwfr.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.zdbjq.cn/Article/details/gggnqyvha.sHtML

[R27] 算术展开
来源：http://wap.fehbvm.com/Article/details/gslmtozgb.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.zdbjq.cn/Article/details/giiawhbnt.sHtML

[R28] 浮点运算
来源：http://m.share.hesvh.cn/Article/details/gvpzjonyu.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.hesvh.cn/Article/details/gvbbnrqqs.sHtML

[R29] 定义函数
来源：http://blog.fehbvm.com/Article/details/gfzrvzikf.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.hesvh.cn/Article/details/gzpvnhcge.sHtML

[R30] 函数返回状态码
来源：http://wap.hesvh.cn/Article/details/gmhkubljh.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.zdbjq.cn/Article/details/gozhwxemp.sHtML

[R31] 局部变量
来源：http://baike.zdbjq.cn/Article/details/gjcsrhwgo.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.zdbjq.cn/Article/details/gerevdoev.sHtML

[R32] 参数个数校验
来源：http://m.share.hesvh.cn/Article/details/gnuapglud.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.hesvh.cn/Article/details/gxklnbodo.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.fehbvm.com/Article/details/gndvxskkq.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.zdbjq.cn/Article/details/gpnwjjopg.sHtML

[R34] 退出时清理
来源：http://3g.zdbjq.cn/Article/details/glarhctor.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fehbvm.com/Article/details/gipkqmkhi.sHtML

[R35] 后台执行并等待
来源：http://read.share.hesvh.cn/Article/details/gdptctfeo.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.zdbjq.cn/Article/details/gitfwwbdb.sHtML

[R36] 并发执行多个任务
来源：http://read.share.zdbjq.cn/Article/details/gzotirenf.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.zdbjq.cn/Article/details/gwkvbqpcb.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.zdbjq.cn/Article/details/gbkpdbmdz.sHtML

files=$(ls -1)
来源：http://baike.zdbjq.cn/Article/details/gcsabrorp.sHtML

[R38] 管道串联
来源：http://www.share.zdbjq.cn/Article/details/gscmrmrol.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.fehbvm.com/Article/details/gcppjtwck.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.fehbvm.com/Article/details/gzdpwnvss.sHtML

cmd > out.log 2>&1
来源：http://www.share.hesvh.cn/Article/details/gsuyerflx.sHtML

[R40] 追加写日志
来源：http://wap.zdbjq.cn/Article/details/gtkvnjxet.sHtML

echo "log" >> out.log
来源：http://wap.hesvh.cn/Article/details/gorrmzlsy.sHtML

[R41] 丢弃输出
来源：http://m.share.zdbjq.cn/Article/details/gkcppgfar.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.zdbjq.cn/Article/details/gizetqsnj.sHtML

[R42] 输入重定向
来源：http://blog.zdbjq.cn/Article/details/gpwjmnldq.sHtML

wc -l < a.txt
来源：http://www.blog.fehbvm.com/Article/details/gooxukxqd.sHtML

[R43] 按名字查找文件
来源：http://baike.fehbvm.com/Article/details/gbhnzruif.sHtML

find . -name "*.log" -type f
来源：http://read.share.zdbjq.cn/Article/details/gciqlhwbx.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.zdbjq.cn/Article/details/gpkpvpshd.sHtML

find . -mtime -7 -type f
来源：http://blog.hesvh.cn/Article/details/gjakizrqq.sHtML

[R45] 批量删除
来源：http://blog.zdbjq.cn/Article/details/grhvvbqhq.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.fehbvm.com/Article/details/gshzktnsd.sHtML

[R46] 递归替换文件内容
来源：http://m.share.fehbvm.com/Article/details/gldneoxwo.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.fehbvm.com/Article/details/gelxknngz.sHtML

[R47] sed 单行替换
来源：http://www.m.share.fehbvm.com/Article/details/gumksnaak.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.zdbjq.cn/Article/details/gbuanltwa.sHtML

[R48] awk 取指定列
来源：http://read.share.zdbjq.cn/Article/details/gdmqdeghp.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.fehbvm.com/Article/details/gwtcayoki.sHtML

[R49] awk 带条件
来源：http://read.share.hesvh.cn/Article/details/gzovtocoi.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.fehbvm.com/Article/details/gpsvfwsey.sHtML

[R50] awk 求和
来源：http://read.share.zdbjq.cn/Article/details/glpnlhzgf.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.hesvh.cn/Article/details/gizrunoho.sHtML

[R51] 排序去重取前几
来源：http://mobile.hesvh.cn/Article/details/guramhhri.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.zdbjq.cn/Article/details/gnhntvdji.sHtML

[R52] 统计行数
来源：http://wap.zdbjq.cn/Article/details/gxdwncflw.sHtML

wc -l a.txt
来源：http://3g.zdbjq.cn/Article/details/gqrwvctlc.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.hesvh.cn/Article/details/ggnppumrc.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.zdbjq.cn/Article/details/gkjocbhlr.sHtML

[R54] 比较两个文件
来源：http://read.share.fehbvm.com/Article/details/gmhgipnzj.sHtML

diff a.txt b.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gipfnfjko.sHtML

[R55] 压缩与解压
来源：http://www.blog.zdbjq.cn/Article/details/gxkoelgxr.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.zdbjq.cn/Article/details/gqdrxwjni.sHtML

[R56] 远程拷贝
来源：http://m.share.hesvh.cn/Article/details/genycfndb.sHtML

scp file user@host:/path/
来源：http://www.share.hesvh.cn/Article/details/gtfbpknmx.sHtML

[R57] 远程执行命令
来源：http://baike.fehbvm.com/Article/details/gycduuhhk.sHtML

ssh user@host 'uptime'
来源：http://baike.fehbvm.com/Article/details/gzetzikgw.sHtML

[R58] 下载文件
来源：http://m.share.zdbjq.cn/Article/details/gpsweiniv.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.hesvh.cn/Article/details/gyavbdhyr.sHtML

[R59] 发 POST JSON
来源：http://m.share.zdbjq.cn/Article/details/gtwxynpwc.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.fehbvm.com/Article/details/gdmsmddes.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.zdbjq.cn/Article/details/gduqrvwtk.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.zdbjq.cn/Article/details/gnubjzrqj.sHtML

[R61] 磁盘占用
来源：http://mobile.hesvh.cn/Article/details/guzcgcehg.sHtML

df -h;  du -sh *
来源：http://m.share.hesvh.cn/Article/details/gvyhicevy.sHtML

[R62] 找最占空间的文件
来源：http://3g.hesvh.cn/Article/details/glkqjnawj.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.fehbvm.com/Article/details/gxtlooovx.sHtML

[R63] 内存与进程
来源：http://wap.zdbjq.cn/Article/details/ggfcwagxo.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.fehbvm.com/Article/details/gzffticjp.sHtML

[R64] 结束进程
来源：http://read.share.fehbvm.com/Article/details/ggiqwwxec.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.zdbjq.cn/Article/details/glwekwbcq.sHtML

[R65] 查看端口占用
来源：http://www.blog.zdbjq.cn/Article/details/glqevaqar.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.hesvh.cn/Article/details/gexirtnui.sHtML

[R66] 定时任务
来源：http://baike.hesvh.cn/Article/details/gbpvrjwjl.sHtML

crontab -e;  crontab -l
来源：http://baike.fehbvm.com/Article/details/gmffqmejj.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.fehbvm.com/Article/details/gqbodslpy.sHtML

openssl rand -hex 16
来源：http://www.m.share.fehbvm.com/Article/details/gjombvlzk.sHtML

[R68] 计算文件校验值
来源：http://mobile.fehbvm.com/Article/details/gwpcyheyi.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.hesvh.cn/Article/details/grjgpnvxj.sHtML

[R69] 生成随机密码
来源：http://wap.fehbvm.com/Article/details/gmwirmdkj.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.hesvh.cn/Article/details/gxjxogbcj.sHtML

[R70] 时间戳与互转
来源：http://baike.zdbjq.cn/Article/details/gqfespyie.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.hesvh.cn/Article/details/guhztqqlr.sHtML

[R71] 日期格式化
来源：http://m.share.zdbjq.cn/Article/details/gdxeywmhp.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.hesvh.cn/Article/details/gixswaaqi.sHtML

[R72] 等待端口就绪
来源：http://m.share.hesvh.cn/Article/details/grqpjoxyy.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.fehbvm.com/Article/details/gecldzdgc.sHtML

[R73] 分割大日志
来源：http://blog.zdbjq.cn/Article/details/gwqrviyat.sHtML

split -l 1000 big.log part_
来源：http://baike.zdbjq.cn/Article/details/gvfhbbtsj.sHtML

[R74] 批量重命名
来源：http://m.share.hesvh.cn/Article/details/ghcdrrnyj.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.fehbvm.com/Article/details/gazgrqctv.sHtML

[R75] 导出环境变量
来源：http://m.share.fehbvm.com/Article/details/ghxqujfga.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.hesvh.cn/Article/details/grwtnnxdw.sHtML

[R76] 使用临时文件
来源：http://www.m.share.zdbjq.cn/Article/details/govmjvhxa.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.hesvh.cn/Article/details/gfkisgtsr.sHtML

[R77] 读取用户输入
来源：http://baike.fehbvm.com/Article/details/gtfvveula.sHtML


<!-- 参考信息 -->