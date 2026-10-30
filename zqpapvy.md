代发 wailian999

[Q36] 左连接
来源：http://www.m.share.zdbjq.cn/Article/details/gzvmbsddp.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mobile.hesvh.cn/Article/details/gpjkrarbj.sHtML

[Q37] 右连接
来源：http://mobile.fehbvm.com/Article/details/gihtuqwpq.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.share.zdbjq.cn/Article/details/goxfpmuym.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.share.hesvh.cn/Article/details/gqcmdtrdm.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.share.zdbjq.cn/Article/details/ghobsdzuy.sHtML

[Q39] 自连接（查上下级）
来源：http://m.share.hesvh.cn/Article/details/gxqzzqzwt.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.blog.zdbjq.cn/Article/details/gjsplchql.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.fehbvm.com/Article/details/gbqleitye.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://3g.fehbvm.com/Article/details/gwuwhodfg.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.hesvh.cn/Article/details/gtpzatunr.sHtML

[Q41] 多表连接
来源：http://m.share.hesvh.cn/Article/details/gtlycoodh.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://3g.hesvh.cn/Article/details/gqijuxzdc.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.hesvh.cn/Article/details/ghfdxfqpr.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.m.share.zdbjq.cn/Article/details/gjapnfrvl.sHtML

[Q42] 连接条件附加过滤
来源：http://wap.fehbvm.com/Article/details/gktkccbkf.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.share.hesvh.cn/Article/details/gduprhkaq.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://3g.fehbvm.com/Article/details/gadzhjozu.sHtML

[Q43] 标量子查询
来源：http://www.blog.fehbvm.com/Article/details/gjmjsebno.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://blog.hesvh.cn/Article/details/gqvcfgjem.sHtML

[Q44] IN 子查询
来源：http://wap.zdbjq.cn/Article/details/gzlgudlvk.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://baike.hesvh.cn/Article/details/guhzxsxkb.sHtML

[Q45] EXISTS 判断存在
来源：http://blog.zdbjq.cn/Article/details/gajukbtty.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.hesvh.cn/Article/details/gebuxhndk.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.m.share.zdbjq.cn/Article/details/groaztzag.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.hesvh.cn/Article/details/gjmneqijl.sHtML

[Q47] 与平均值比较
来源：http://www.share.hesvh.cn/Article/details/gsjqmfais.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.zdbjq.cn/Article/details/gwhpddoyh.sHtML

[Q48] CTE 公用表表达式
来源：http://wap.fehbvm.com/Article/details/ghdcsdnmr.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.blog.hesvh.cn/Article/details/gkvjnesfk.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.fehbvm.com/Article/details/gapavkdvj.sHtML

[Q49] 更新单行
来源：http://3g.zdbjq.cn/Article/details/gljztojli.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.zdbjq.cn/Article/details/gumtahkkj.sHtML

[Q50] 批量更新
来源：http://www.m.share.zdbjq.cn/Article/details/gfzolemys.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.share.hesvh.cn/Article/details/gbgvftjeb.sHtML

[Q51] 用子查询更新
来源：http://www.share.hesvh.cn/Article/details/gacjrgcub.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gcyhunzyl.sHtML

[Q52] 删除指定行
来源：http://baike.hesvh.cn/Article/details/geqlpifpq.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.fehbvm.com/Article/details/giyowaejo.sHtML

[Q53] 按条件删除
来源：http://m.share.hesvh.cn/Article/details/glhqnbixw.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wap.fehbvm.com/Article/details/gfoukpwko.sHtML

[Q54] 清空表
来源：http://www.share.zdbjq.cn/Article/details/gqppvjbak.sHtML

TRUNCATE TABLE logs;
来源：http://blog.fehbvm.com/Article/details/gubrnwqew.sHtML

[Q55] 排名（并列占位）
来源：http://www.m.share.hesvh.cn/Article/details/ggkrzdjpg.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.zdbjq.cn/Article/details/goiddjiev.sHtML

[Q56] 密集排名（并列不占位）
来源：http://3g.hesvh.cn/Article/details/gdxzeymlw.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://blog.hesvh.cn/Article/details/gtlvcckcg.sHtML

[Q57] 行号
来源：http://www.blog.fehbvm.com/Article/details/grgengkxa.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/grccmxaao.sHtML

[Q58] 累计求和
来源：http://m.share.fehbvm.com/Article/details/govxmbqdk.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wap.zdbjq.cn/Article/details/gmndfbcoc.sHtML

[Q59] 分组内累计
来源：http://www.m.share.fehbvm.com/Article/details/gdplhviqu.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gqyrqdhxy.sHtML

[Q60] 取上一行 / 下一行
来源：http://wap.hesvh.cn/Article/details/gickckled.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.zdbjq.cn/Article/details/gkbcxblht.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/gzrlmidmi.sHtML

[Q61] 移动平均
来源：http://www.blog.hesvh.cn/Article/details/gblahnekh.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/gvqvwywkt.sHtML

[Q62] 分组占比
来源：http://www.blog.fehbvm.com/Article/details/gadzecgxa.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://baike.hesvh.cn/Article/details/ggehydsdr.sHtML

[Q63] 开启事务
来源：http://wap.hesvh.cn/Article/details/gbtllnrsg.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.zdbjq.cn/Article/details/gsuymqkbn.sHtML

[Q64] 提交事务
来源：http://www.m.share.hesvh.cn/Article/details/gegsffibk.sHtML

COMMIT;
来源：http://mobile.zdbjq.cn/Article/details/gvoqhlxev.sHtML

[Q65] 回滚事务
来源：http://blog.hesvh.cn/Article/details/gxtyaztjr.sHtML

ROLLBACK;
来源：http://3g.hesvh.cn/Article/details/gjdmgzihm.sHtML

[Q66] 行锁查询
来源：http://mobile.hesvh.cn/Article/details/gksblzril.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://baike.hesvh.cn/Article/details/growyyumx.sHtML

[Q67] 设置隔离级别
来源：http://wap.fehbvm.com/Article/details/gndirwyxe.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.m.share.fehbvm.com/Article/details/gkckwgssg.sHtML

[Q68] 保存点
来源：http://3g.hesvh.cn/Article/details/gohmbbjle.sHtML

SAVEPOINT sp1;
来源：http://wap.fehbvm.com/Article/details/gbremtrio.sHtML

ROLLBACK TO sp1;
来源：http://read.share.hesvh.cn/Article/details/gzaaklhrb.sHtML

[Q69] 查看执行计划
来源：http://baike.zdbjq.cn/Article/details/gtgtaobgz.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.hesvh.cn/Article/details/glpsiwmky.sHtML

[Q70] 更新统计信息
来源：http://3g.fehbvm.com/Article/details/grbyiotpe.sHtML

ANALYZE TABLE users;
来源：http://m.share.zdbjq.cn/Article/details/gwfsruaxf.sHtML

[Q71] 查看建表语句
来源：http://read.share.hesvh.cn/Article/details/gydjtvbuq.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.zdbjq.cn/Article/details/gzukohtyh.sHtML

[Q72] 查看索引
来源：http://blog.zdbjq.cn/Article/details/gxzmjwwlv.sHtML

SHOW INDEX FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gturnpmnm.sHtML

[Q73] 查看表状态
来源：http://blog.zdbjq.cn/Article/details/gybjkkhvm.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.zdbjq.cn/Article/details/gbawibssb.sHtML

[Q74] 强制使用索引
来源：http://read.share.zdbjq.cn/Article/details/gwbllimsg.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://read.share.hesvh.cn/Article/details/gbgvyiuja.sHtML

[Q75] 日期格式化
来源：http://www.share.hesvh.cn/Article/details/geohjzlnn.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.hesvh.cn/Article/details/gjgmtovhe.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.fehbvm.com/Article/details/gtnqkbmgr.sHtML

[Q76] 按天统计
来源：http://blog.fehbvm.com/Article/details/gobfgqrsi.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.zdbjq.cn/Article/details/gkmrgiori.sHtML

[Q77] 时间加减
来源：http://www.m.share.zdbjq.cn/Article/details/gynbrcoqc.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.zdbjq.cn/Article/details/ghgxdqakz.sHtML

[Q78] 当前时间
来源：http://mobile.fehbvm.com/Article/details/gcmcwjmjt.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.hesvh.cn/Article/details/gzesdwghc.sHtML

[Q79] 字符串拼接
来源：http://www.blog.hesvh.cn/Article/details/gxoglrqdk.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.hesvh.cn/Article/details/gjnnusmjs.sHtML

[Q80] 字符串截取
来源：http://www.blog.hesvh.cn/Article/details/gflmjfhoa.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mobile.fehbvm.com/Article/details/gpxxlrrus.sHtML

[Q81] 字符串替换
来源：http://www.m.share.zdbjq.cn/Article/details/glzvpsrqz.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.hesvh.cn/Article/details/gncnwwdfw.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.zdbjq.cn/Article/details/ggwhuqsum.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gnplylijx.sHtML

[Q83] 大小写转换
来源：http://baike.fehbvm.com/Article/details/gvbmrzmtg.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.hesvh.cn/Article/details/gcbwjxicz.sHtML

[Q84] 去除首尾空格
来源：http://m.share.hesvh.cn/Article/details/gcwnskrsw.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.fehbvm.com/Article/details/ggovdbcrs.sHtML

[Q85] 数值取整
来源：http://m.share.zdbjq.cn/Article/details/gzawtufqi.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.fehbvm.com/Article/details/gyrmolfff.sHtML

[Q86] 读取 JSON 字段
来源：http://www.m.share.hesvh.cn/Article/details/gednvrjkv.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.zdbjq.cn/Article/details/gtspxuoap.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.fehbvm.com/Article/details/gggxcsrop.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.hesvh.cn/Article/details/gpdgvoscr.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.hesvh.cn/Article/details/gucefujsn.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.zdbjq.cn/Article/details/gsapppids.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.zdbjq.cn/Article/details/gisjufxkr.sHtML

[Q89] 判断表是否存在
来源：http://blog.hesvh.cn/Article/details/gmjaxelie.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.hesvh.cn/Article/details/gvfmkhwdd.sHtML

[Q90] 生成序号列
来源：http://www.share.fehbvm.com/Article/details/gkjfubdat.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.zdbjq.cn/Article/details/gmacmnfcf.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/grtmdyfcn.sHtML

R. Bash 专题
来源：http://baike.fehbvm.com/Article/details/gdtvwepei.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gtqoagdcz.sHtML

[R01] shebang 与严格模式
来源：http://www.share.hesvh.cn/Article/details/gqrcyadrx.sHtML

#!/usr/bin/env bash
来源：http://www.blog.zdbjq.cn/Article/details/gxjcoeryk.sHtML

set -euo pipefail
来源：http://www.blog.fehbvm.com/Article/details/gzeltrvbx.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.zdbjq.cn/Article/details/ghhwpjpba.sHtML

name="Tom"; echo "$name"
来源：http://wap.fehbvm.com/Article/details/gphqusorj.sHtML

[R03] 只读变量
来源：http://baike.zdbjq.cn/Article/details/gvgngnzhp.sHtML

readonly PI=3.14
来源：http://www.blog.fehbvm.com/Article/details/gceodenks.sHtML

[R04] 位置参数
来源：http://mobile.zdbjq.cn/Article/details/grxsetyda.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.fehbvm.com/Article/details/gmgekevzh.sHtML

[R05] 参数默认值
来源：http://www.m.share.zdbjq.cn/Article/details/gsueodovc.sHtML

name="${1:-default}"
来源：http://www.blog.hesvh.cn/Article/details/gnqypwlin.sHtML

[R06] 判断命令是否存在
来源：http://wap.zdbjq.cn/Article/details/gbufanxey.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.fehbvm.com/Article/details/gfehlcmus.sHtML

[R07] if 判断文件
来源：http://m.share.hesvh.cn/Article/details/grdqzwotj.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.zdbjq.cn/Article/details/gfqdspqlh.sHtML

[R08] 数值比较
来源：http://baike.hesvh.cn/Article/details/ghcapghjq.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://mobile.fehbvm.com/Article/details/gcbkubtbd.sHtML

[R09] 字符串比较
来源：http://baike.fehbvm.com/Article/details/gnycqiakh.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.hesvh.cn/Article/details/glnawcmtc.sHtML

[R10] 正则匹配
来源：http://3g.zdbjq.cn/Article/details/gzclvqlso.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.zdbjq.cn/Article/details/gmwexevtd.sHtML

[R11] case 多分支
来源：http://read.share.zdbjq.cn/Article/details/gduxuteol.sHtML

case "$1" in
来源：http://wap.hesvh.cn/Article/details/gkpcxijkc.sHtML

start) echo "启动" ;;
来源：http://read.share.zdbjq.cn/Article/details/gfrkabujp.sHtML

stop)  echo "停止" ;;
来源：http://mobile.zdbjq.cn/Article/details/ggzwstcwf.sHtML

*)     echo "未知命令" ;;
来源：http://baike.zdbjq.cn/Article/details/gtmafrnmv.sHtML

esac
来源：http://www.m.share.fehbvm.com/Article/details/ggywqileq.sHtML

[R12] for 遍历文件
来源：http://baike.fehbvm.com/Article/details/gsaurjalf.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.zdbjq.cn/Article/details/gfduvysla.sHtML

[R13] for 计数循环
来源：http://www.blog.hesvh.cn/Article/details/gotmexlla.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.zdbjq.cn/Article/details/gwqwirnwn.sHtML

[R14] C 风格 for
来源：http://wap.fehbvm.com/Article/details/gponjvyqj.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.hesvh.cn/Article/details/ggqqrfiyw.sHtML

[R15] while 逐行读文件
来源：http://blog.fehbvm.com/Article/details/gwwerfexp.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.fehbvm.com/Article/details/guwhakift.sHtML

[R16] until 等待条件
来源：http://www.blog.zdbjq.cn/Article/details/gkcvieslq.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.zdbjq.cn/Article/details/gjxirunrz.sHtML

[R17] 数组定义与取值
来源：http://read.share.hesvh.cn/Article/details/gnicpybsf.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.zdbjq.cn/Article/details/gfwgwxhgy.sHtML

[R18] 遍历数组
来源：http://blog.fehbvm.com/Article/details/gurknqbkx.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.hesvh.cn/Article/details/gcfnjdpkm.sHtML

[R19] 数组长度
来源：http://www.blog.zdbjq.cn/Article/details/gpxwtgpgz.sHtML

echo "${#arr[@]}"
来源：http://m.share.zdbjq.cn/Article/details/gknniqwbn.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.zdbjq.cn/Article/details/gqlxtzned.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.zdbjq.cn/Article/details/gubcrmicv.sHtML

[R21] 字符串长度
来源：http://wap.fehbvm.com/Article/details/gsqphfxpq.sHtML

echo "${#s}"
来源：http://www.share.hesvh.cn/Article/details/gsyxlxsfm.sHtML

[R22] 截取子串
来源：http://www.share.fehbvm.com/Article/details/gqmxtjkfs.sHtML

echo "${s:0:5}"
来源：http://3g.hesvh.cn/Article/details/ghnkasgoi.sHtML

[R23] 字符串替换
来源：http://read.share.hesvh.cn/Article/details/gtpgkxpay.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.hesvh.cn/Article/details/gdqppzizs.sHtML

[R24] 大小写转换
来源：http://read.share.fehbvm.com/Article/details/gipmpxyga.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.hesvh.cn/Article/details/gjfzxyecd.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.hesvh.cn/Article/details/gswquezeq.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.hesvh.cn/Article/details/gdabqwxnl.sHtML

[R26] 命令替换
来源：http://www.m.share.zdbjq.cn/Article/details/gmimkztkt.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.fehbvm.com/Article/details/gjvgfkmlt.sHtML

[R27] 算术展开
来源：http://www.share.fehbvm.com/Article/details/gfeoldujc.sHtML

echo $((1 + 2 * 3))
来源：http://3g.hesvh.cn/Article/details/gdnrcwcqh.sHtML

[R28] 浮点运算
来源：http://baike.zdbjq.cn/Article/details/gyzhxpskv.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.fehbvm.com/Article/details/gwzwabnir.sHtML

[R29] 定义函数
来源：http://mobile.hesvh.cn/Article/details/guvkezbff.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.fehbvm.com/Article/details/gzpcilenw.sHtML

[R30] 函数返回状态码
来源：http://www.blog.zdbjq.cn/Article/details/gfxsocvgp.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.zdbjq.cn/Article/details/gzuqmwoum.sHtML

[R31] 局部变量
来源：http://read.share.hesvh.cn/Article/details/gzfvpeeds.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.fehbvm.com/Article/details/gjintkzmq.sHtML

[R32] 参数个数校验
来源：http://m.share.hesvh.cn/Article/details/ggrtegvhm.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.hesvh.cn/Article/details/gaxkbvlzw.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.hesvh.cn/Article/details/gipfhmkxw.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.zdbjq.cn/Article/details/ghiwjrjuo.sHtML

[R34] 退出时清理
来源：http://mobile.zdbjq.cn/Article/details/gqdpvuvno.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.zdbjq.cn/Article/details/gdzlrdawt.sHtML

[R35] 后台执行并等待
来源：http://www.share.fehbvm.com/Article/details/gheblnlqq.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.hesvh.cn/Article/details/gqrtafkvm.sHtML

[R36] 并发执行多个任务
来源：http://baike.zdbjq.cn/Article/details/gedpfbohm.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.fehbvm.com/Article/details/glpxldxrt.sHtML

[R37] 把输出赋给变量
来源：http://wap.zdbjq.cn/Article/details/ggacjulmc.sHtML

files=$(ls -1)
来源：http://wap.fehbvm.com/Article/details/gklaagcvh.sHtML

[R38] 管道串联
来源：http://www.m.share.fehbvm.com/Article/details/guteweyve.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.fehbvm.com/Article/details/gdoykpgfs.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.hesvh.cn/Article/details/gdpdacots.sHtML

cmd > out.log 2>&1
来源：http://3g.zdbjq.cn/Article/details/gsgtxeemj.sHtML

[R40] 追加写日志
来源：http://m.share.fehbvm.com/Article/details/guwwucpdz.sHtML

echo "log" >> out.log
来源：http://3g.zdbjq.cn/Article/details/gzurrviwa.sHtML

[R41] 丢弃输出
来源：http://blog.zdbjq.cn/Article/details/gpjokiron.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.zdbjq.cn/Article/details/gmwumtljm.sHtML

[R42] 输入重定向
来源：http://mobile.zdbjq.cn/Article/details/gvauafszn.sHtML

wc -l < a.txt
来源：http://mobile.hesvh.cn/Article/details/gwkohuxzn.sHtML

[R43] 按名字查找文件
来源：http://mobile.zdbjq.cn/Article/details/gklbbglhp.sHtML

find . -name "*.log" -type f
来源：http://blog.zdbjq.cn/Article/details/glkgoyfhr.sHtML

[R44] 按修改时间查找
来源：http://read.share.hesvh.cn/Article/details/gkfxbhtej.sHtML

find . -mtime -7 -type f
来源：http://mobile.fehbvm.com/Article/details/ghwqzffnt.sHtML

[R45] 批量删除
来源：http://baike.zdbjq.cn/Article/details/gfahinsly.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.zdbjq.cn/Article/details/gguojyjho.sHtML

[R46] 递归替换文件内容
来源：http://www.share.hesvh.cn/Article/details/gvoogkzuh.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.hesvh.cn/Article/details/gnpagnolj.sHtML

[R47] sed 单行替换
来源：http://3g.zdbjq.cn/Article/details/gvmdzrbwe.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.fehbvm.com/Article/details/gjuuyfivq.sHtML

[R48] awk 取指定列
来源：http://read.share.fehbvm.com/Article/details/gxwwxvvvw.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.zdbjq.cn/Article/details/gcqhigzpd.sHtML

[R49] awk 带条件
来源：http://www.share.zdbjq.cn/Article/details/gqfdhawqt.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.zdbjq.cn/Article/details/gfcywxtmi.sHtML

[R50] awk 求和
来源：http://blog.hesvh.cn/Article/details/gubauqqdf.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.hesvh.cn/Article/details/ghjkeokrk.sHtML

[R51] 排序去重取前几
来源：http://baike.fehbvm.com/Article/details/gkdrqmzxe.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.zdbjq.cn/Article/details/gwyqdnjap.sHtML

[R52] 统计行数
来源：http://read.share.fehbvm.com/Article/details/gjingfwoa.sHtML

wc -l a.txt
来源：http://wap.fehbvm.com/Article/details/gnjqlxnjq.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.zdbjq.cn/Article/details/gajdhojup.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.zdbjq.cn/Article/details/gsuabbrwc.sHtML

[R54] 比较两个文件
来源：http://www.m.share.hesvh.cn/Article/details/gubqvitms.sHtML

diff a.txt b.txt
来源：http://read.share.fehbvm.com/Article/details/gzklksxof.sHtML

[R55] 压缩与解压
来源：http://m.share.zdbjq.cn/Article/details/gnigfrpfk.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.fehbvm.com/Article/details/gioslrmur.sHtML

[R56] 远程拷贝
来源：http://www.blog.fehbvm.com/Article/details/gvaswassk.sHtML

scp file user@host:/path/
来源：http://mobile.fehbvm.com/Article/details/gcwrrrzhu.sHtML

[R57] 远程执行命令
来源：http://mobile.hesvh.cn/Article/details/gsxehfhqr.sHtML

ssh user@host 'uptime'
来源：http://3g.fehbvm.com/Article/details/gkaypuenh.sHtML

[R58] 下载文件
来源：http://www.share.zdbjq.cn/Article/details/gcjfpebru.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.fehbvm.com/Article/details/gahzaojkn.sHtML

[R59] 发 POST JSON
来源：http://m.share.hesvh.cn/Article/details/gskzpkucd.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.fehbvm.com/Article/details/gufoavgqm.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.fehbvm.com/Article/details/goppcdziv.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.fehbvm.com/Article/details/gewpnyddr.sHtML

[R61] 磁盘占用
来源：http://www.blog.zdbjq.cn/Article/details/gsvfeucbs.sHtML

df -h;  du -sh *
来源：http://www.share.fehbvm.com/Article/details/gptcjuock.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.hesvh.cn/Article/details/gzogzoxwg.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.zdbjq.cn/Article/details/gsacbejrj.sHtML

[R63] 内存与进程
来源：http://baike.zdbjq.cn/Article/details/giukecubt.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.hesvh.cn/Article/details/gmpuspeil.sHtML

[R64] 结束进程
来源：http://blog.fehbvm.com/Article/details/goqvmubtc.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.zdbjq.cn/Article/details/gsoerzxsg.sHtML

[R65] 查看端口占用
来源：http://www.share.zdbjq.cn/Article/details/gvkozjmvu.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.fehbvm.com/Article/details/gumwjxdvl.sHtML

[R66] 定时任务
来源：http://read.share.hesvh.cn/Article/details/gfvywohdb.sHtML

crontab -e;  crontab -l
来源：http://blog.hesvh.cn/Article/details/gnusqzlez.sHtML

[R67] 生成随机十六进制串
来源：http://wap.hesvh.cn/Article/details/gcnevkzgi.sHtML

openssl rand -hex 16
来源：http://www.blog.zdbjq.cn/Article/details/gdsryfozd.sHtML

[R68] 计算文件校验值
来源：http://read.share.hesvh.cn/Article/details/ggnzfprjc.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.hesvh.cn/Article/details/giqfijixc.sHtML

[R69] 生成随机密码
来源：http://3g.zdbjq.cn/Article/details/gfgmqrnxm.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.fehbvm.com/Article/details/gsiwtntoh.sHtML

[R70] 时间戳与互转
来源：http://blog.hesvh.cn/Article/details/gjmcmgixv.sHtML

date +%s;  date -d @1700000000
来源：http://blog.hesvh.cn/Article/details/gktqrhqcw.sHtML

[R71] 日期格式化
来源：http://3g.fehbvm.com/Article/details/gxpnolpli.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.hesvh.cn/Article/details/gxndpbsfu.sHtML

[R72] 等待端口就绪
来源：http://m.share.hesvh.cn/Article/details/gcqejnbqs.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.zdbjq.cn/Article/details/gmwmdtxmr.sHtML

[R73] 分割大日志
来源：http://m.share.hesvh.cn/Article/details/glvidmfrc.sHtML

split -l 1000 big.log part_
来源：http://m.share.hesvh.cn/Article/details/gszhtzaoy.sHtML

[R74] 批量重命名
来源：http://www.blog.zdbjq.cn/Article/details/grwgrkndm.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.zdbjq.cn/Article/details/gtwtvidet.sHtML

[R75] 导出环境变量
来源：http://www.share.hesvh.cn/Article/details/ghhgbppid.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.fehbvm.com/Article/details/gansxkakd.sHtML

[R76] 使用临时文件
来源：http://m.share.hesvh.cn/Article/details/gcxjoczvw.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.hesvh.cn/Article/details/gbntkkine.sHtML

[R77] 读取用户输入
来源：http://www.m.share.fehbvm.com/Article/details/gvnpgcsjr.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.hesvh.cn/Article/details/giyjdysde.sHtML

[R78] 交互式菜单
来源：http://m.share.hesvh.cn/Article/details/gzazcrwca.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.zdbjq.cn/Article/details/guczpmchv.sHtML

[R79] 解析命令行选项
来源：http://m.share.zdbjq.cn/Article/details/gjnfozuvl.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.zdbjq.cn/Article/details/gcaftyhti.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.hesvh.cn/Article/details/gcwtaasdd.sHtML

time ./run.sh
来源：http://m.share.hesvh.cn/Article/details/gtiyzulop.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gvfdabprv.sHtML

S. C / C++ 专题
来源：http://blog.hesvh.cn/Article/details/gabnezeed.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gmnhhhnko.sHtML

[S01] C：Hello World
来源：http://3g.fehbvm.com/Article/details/gnirscyhn.sHtML

#include <stdio.h>
来源：http://www.m.share.zdbjq.cn/Article/details/ghyfjegzg.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.fehbvm.com/Article/details/glbzipoov.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.hesvh.cn/Article/details/gzoslqdag.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.hesvh.cn/Article/details/giuzitamq.sHtML

[S03] C：读入整数
来源：http://blog.hesvh.cn/Article/details/gpfnfghyi.sHtML

int x; scanf("%d", &x);
来源：http://read.share.zdbjq.cn/Article/details/gdsbiwolw.sHtML

[S04] C：字符串复制
来源：http://www.m.share.hesvh.cn/Article/details/gzajmiexb.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.fehbvm.com/Article/details/gxdfisscq.sHtML

[S05] C：字符串长度
来源：http://3g.hesvh.cn/Article/details/gmehqiwtn.sHtML


<!-- 参考信息 -->