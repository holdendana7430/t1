代发 wailian999

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://m.share.fanxiaobao.xyz/Article/details/gzlrbcgac.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://baike.fanxiaobao.xyz/Article/details/gxhwamgny.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://3g.fanxiaobao.xyz/Article/details/gdgrxdhbe.sHtML

[Q41] 多表连接
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdmnegudv.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.share.fanxiaobao.xyz/Article/details/grvuovfjn.sHtML

JOIN users u ON u.id = o.user_id
来源：http://wap.fanxiaobao.xyz/Article/details/ghkjlsoyj.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.fanxiaobao.xyz/Article/details/gjoabltox.sHtML

[Q42] 连接条件附加过滤
来源：http://www.share.fanxiaobao.xyz/Article/details/ghipbvjpz.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.blog.fanxiaobao.xyz/Article/details/giumehghn.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghgufbiwz.sHtML

[Q43] 标量子查询
来源：http://wap.fanxiaobao.xyz/Article/details/gqiqswvet.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://3g.fanxiaobao.xyz/Article/details/gtagaldqn.sHtML

[Q44] IN 子查询
来源：http://m.share.fanxiaobao.xyz/Article/details/gawkjgbux.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wap.fanxiaobao.xyz/Article/details/gpehqgisx.sHtML

[Q45] EXISTS 判断存在
来源：http://mobile.fanxiaobao.xyz/Article/details/gtxsprkps.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.fanxiaobao.xyz/Article/details/glyisvohg.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.fanxiaobao.xyz/Article/details/gwzblhivk.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.fanxiaobao.xyz/Article/details/gjdlvydad.sHtML

[Q47] 与平均值比较
来源：http://read.share.fanxiaobao.xyz/Article/details/gbnlczqog.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.share.fanxiaobao.xyz/Article/details/gunuefvry.sHtML

[Q48] CTE 公用表表达式
来源：http://3g.fanxiaobao.xyz/Article/details/geqrrxoji.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gftuernhw.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://mobile.fanxiaobao.xyz/Article/details/gqzcpmgiq.sHtML

[Q49] 更新单行
来源：http://m.share.fanxiaobao.xyz/Article/details/gcpphhmks.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://m.share.fanxiaobao.xyz/Article/details/gvbprrgzc.sHtML

[Q50] 批量更新
来源：http://wap.fanxiaobao.xyz/Article/details/gxyafbdas.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.fanxiaobao.xyz/Article/details/guxykcgjw.sHtML

[Q51] 用子查询更新
来源：http://m.share.fanxiaobao.xyz/Article/details/gkroqenor.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://blog.fanxiaobao.xyz/Article/details/gmwcwhqur.sHtML

[Q52] 删除指定行
来源：http://mobile.fanxiaobao.xyz/Article/details/glnbdvvpx.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.fanxiaobao.xyz/Article/details/gokesyogh.sHtML

[Q53] 按条件删除
来源：http://read.share.fanxiaobao.xyz/Article/details/gppivtmxs.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wap.fanxiaobao.xyz/Article/details/gpyjwqtdb.sHtML

[Q54] 清空表
来源：http://3g.fanxiaobao.xyz/Article/details/gesxmhwet.sHtML

TRUNCATE TABLE logs;
来源：http://wap.fanxiaobao.xyz/Article/details/gkemcztiq.sHtML

[Q55] 排名（并列占位）
来源：http://mobile.fanxiaobao.xyz/Article/details/gqznfhcmp.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.fanxiaobao.xyz/Article/details/gqmjtgfqs.sHtML

[Q56] 密集排名（并列不占位）
来源：http://wap.fanxiaobao.xyz/Article/details/gewmizcea.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mobile.fanxiaobao.xyz/Article/details/gkabjogiz.sHtML

[Q57] 行号
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzddgmtip.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/ggqjafmok.sHtML

[Q58] 累计求和
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxocphrrr.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wap.fanxiaobao.xyz/Article/details/gxedvzffv.sHtML

[Q59] 分组内累计
来源：http://blog.fanxiaobao.xyz/Article/details/gfbjqeqxa.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfqqgztgi.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.fanxiaobao.xyz/Article/details/ggtveucbr.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyqucrueb.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.share.fanxiaobao.xyz/Article/details/gmyaqaeck.sHtML

[Q61] 移动平均
来源：http://www.share.fanxiaobao.xyz/Article/details/gvsepxqyy.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://3g.fanxiaobao.xyz/Article/details/gxhypzbgn.sHtML

[Q62] 分组占比
来源：http://wap.fanxiaobao.xyz/Article/details/giyjkrhmk.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkprxbqyh.sHtML

[Q63] 开启事务
来源：http://m.share.fanxiaobao.xyz/Article/details/glaxajbho.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.fanxiaobao.xyz/Article/details/gzpsliiqw.sHtML

[Q64] 提交事务
来源：http://mobile.fanxiaobao.xyz/Article/details/galdebsqo.sHtML

COMMIT;
来源：http://wap.fanxiaobao.xyz/Article/details/grqyjhhjo.sHtML

[Q65] 回滚事务
来源：http://read.share.fanxiaobao.xyz/Article/details/gbyqllbkw.sHtML

ROLLBACK;
来源：http://baike.fanxiaobao.xyz/Article/details/gnywfpucw.sHtML

[Q66] 行锁查询
来源：http://m.share.fanxiaobao.xyz/Article/details/gynhaymhg.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.fanxiaobao.xyz/Article/details/gycltvirh.sHtML

[Q67] 设置隔离级别
来源：http://www.share.fanxiaobao.xyz/Article/details/ghxwfnocx.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://3g.fanxiaobao.xyz/Article/details/ghhzrnqor.sHtML

[Q68] 保存点
来源：http://www.share.fanxiaobao.xyz/Article/details/gsipvygjr.sHtML

SAVEPOINT sp1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqkhassip.sHtML

ROLLBACK TO sp1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gwnqlyslr.sHtML

[Q69] 查看执行计划
来源：http://3g.fanxiaobao.xyz/Article/details/gkawbgxnb.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.fanxiaobao.xyz/Article/details/grtuqzohj.sHtML

[Q70] 更新统计信息
来源：http://mobile.fanxiaobao.xyz/Article/details/gvzenfirm.sHtML

ANALYZE TABLE users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gxmayeudd.sHtML

[Q71] 查看建表语句
来源：http://blog.fanxiaobao.xyz/Article/details/govlqbgpg.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdlprjzvp.sHtML

[Q72] 查看索引
来源：http://baike.fanxiaobao.xyz/Article/details/gugtkbbtw.sHtML

SHOW INDEX FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gpqzozlun.sHtML

[Q73] 查看表状态
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grnbultmz.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://wap.fanxiaobao.xyz/Article/details/gsdzlvaek.sHtML

[Q74] 强制使用索引
来源：http://www.blog.fanxiaobao.xyz/Article/details/glhocsxzn.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.fanxiaobao.xyz/Article/details/gnjinefyz.sHtML

[Q75] 日期格式化
来源：http://3g.fanxiaobao.xyz/Article/details/ggnmeulaf.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.fanxiaobao.xyz/Article/details/gqnhznzxf.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.blog.fanxiaobao.xyz/Article/details/galwzhsmt.sHtML

[Q76] 按天统计
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glwnyccel.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guqmzvrcb.sHtML

[Q77] 时间加减
来源：http://wap.fanxiaobao.xyz/Article/details/gksgyjcun.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://baike.fanxiaobao.xyz/Article/details/girikjlmh.sHtML

[Q78] 当前时间
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggfqkfwba.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.fanxiaobao.xyz/Article/details/glyxzpoop.sHtML

[Q79] 字符串拼接
来源：http://www.share.fanxiaobao.xyz/Article/details/ggxalfkyp.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.fanxiaobao.xyz/Article/details/gstmoawih.sHtML

[Q80] 字符串截取
来源：http://wap.fanxiaobao.xyz/Article/details/gveemhwhc.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjsakpovt.sHtML

[Q81] 字符串替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gntwnhidx.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gjshqbjlb.sHtML

[Q82] 字符长度与字节长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gxwudlujo.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gwekzcllr.sHtML

[Q83] 大小写转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyiiklsps.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gccuddsrs.sHtML

[Q84] 去除首尾空格
来源：http://mobile.fanxiaobao.xyz/Article/details/gwgrlynsi.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gyzpgomhj.sHtML

[Q85] 数值取整
来源：http://www.share.fanxiaobao.xyz/Article/details/gnkzqfgxo.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.fanxiaobao.xyz/Article/details/gpiaenyfc.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.fanxiaobao.xyz/Article/details/gmzdsyayr.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.fanxiaobao.xyz/Article/details/gixmzlceo.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gciofskda.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://baike.fanxiaobao.xyz/Article/details/gfhgpflkv.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.share.fanxiaobao.xyz/Article/details/gbzeguwuq.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goxpyzsmo.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gowvsqeka.sHtML

[Q89] 判断表是否存在
来源：http://blog.fanxiaobao.xyz/Article/details/gjnwenvet.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.fanxiaobao.xyz/Article/details/ggncabzuu.sHtML

[Q90] 生成序号列
来源：http://m.share.fanxiaobao.xyz/Article/details/ggzcrlwlb.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.fanxiaobao.xyz/Article/details/grdjtgbck.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gnlwiyife.sHtML

R. Bash 专题
来源：http://blog.fanxiaobao.xyz/Article/details/gwcvvgazl.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gbuqfvosw.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcyichhoc.sHtML

#!/usr/bin/env bash
来源：http://3g.fanxiaobao.xyz/Article/details/gojfiwhxq.sHtML

set -euo pipefail
来源：http://wap.fanxiaobao.xyz/Article/details/goaybezgk.sHtML

[R02] 变量赋值与使用
来源：http://baike.fanxiaobao.xyz/Article/details/gfemwjvhd.sHtML

name="Tom"; echo "$name"
来源：http://mobile.fanxiaobao.xyz/Article/details/gzmfvkqye.sHtML

[R03] 只读变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtbmyaagz.sHtML

readonly PI=3.14
来源：http://wap.fanxiaobao.xyz/Article/details/gmkxlwrgm.sHtML

[R04] 位置参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnxptodzp.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.fanxiaobao.xyz/Article/details/gpixynbgs.sHtML

[R05] 参数默认值
来源：http://mobile.fanxiaobao.xyz/Article/details/gvbwecrho.sHtML

name="${1:-default}"
来源：http://baike.fanxiaobao.xyz/Article/details/gpqnrvwvu.sHtML

[R06] 判断命令是否存在
来源：http://read.share.fanxiaobao.xyz/Article/details/gmdumzrjd.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.fanxiaobao.xyz/Article/details/ganlotfjo.sHtML

[R07] if 判断文件
来源：http://3g.fanxiaobao.xyz/Article/details/gyakxscww.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwqhyjvco.sHtML

[R08] 数值比较
来源：http://baike.fanxiaobao.xyz/Article/details/gyabsknvh.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.fanxiaobao.xyz/Article/details/glkueubkk.sHtML

[R09] 字符串比较
来源：http://mobile.fanxiaobao.xyz/Article/details/gvajxydei.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.fanxiaobao.xyz/Article/details/gwapltsnq.sHtML

[R10] 正则匹配
来源：http://baike.fanxiaobao.xyz/Article/details/gqopewkcc.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.fanxiaobao.xyz/Article/details/gljevyyve.sHtML

[R11] case 多分支
来源：http://blog.fanxiaobao.xyz/Article/details/gxxfheumo.sHtML

case "$1" in
来源：http://www.blog.fanxiaobao.xyz/Article/details/ginhcnyye.sHtML

start) echo "启动" ;;
来源：http://mobile.fanxiaobao.xyz/Article/details/gmgrhigqz.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxxmyxjea.sHtML

*)     echo "未知命令" ;;
来源：http://3g.fanxiaobao.xyz/Article/details/gaepvmjfc.sHtML

esac
来源：http://wap.fanxiaobao.xyz/Article/details/grjdtsncu.sHtML

[R12] for 遍历文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gwkmuiysc.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gbfvoqvuv.sHtML

[R13] for 计数循环
来源：http://3g.fanxiaobao.xyz/Article/details/gkzzbsfig.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gtqjvjkrg.sHtML

[R14] C 风格 for
来源：http://wap.fanxiaobao.xyz/Article/details/gkktzpexc.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gjwewtjcp.sHtML

[R15] while 逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gtzbereoq.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gzxefruyw.sHtML

[R16] until 等待条件
来源：http://read.share.fanxiaobao.xyz/Article/details/gghevnhbz.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gxpfmpnei.sHtML

[R17] 数组定义与取值
来源：http://blog.fanxiaobao.xyz/Article/details/gzqewoaht.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.fanxiaobao.xyz/Article/details/gcsxssvav.sHtML

[R18] 遍历数组
来源：http://mobile.fanxiaobao.xyz/Article/details/grqzvocgg.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtjrikswv.sHtML

[R19] 数组长度
来源：http://blog.fanxiaobao.xyz/Article/details/gcfaejlfv.sHtML

echo "${#arr[@]}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gfwzgrtjt.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gujpjovvg.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.fanxiaobao.xyz/Article/details/gorpajfco.sHtML

[R21] 字符串长度
来源：http://blog.fanxiaobao.xyz/Article/details/gxhrqmxep.sHtML

echo "${#s}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guavkcvfz.sHtML

[R22] 截取子串
来源：http://3g.fanxiaobao.xyz/Article/details/gpojvljhc.sHtML

echo "${s:0:5}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnvakgrfa.sHtML

[R23] 字符串替换
来源：http://3g.fanxiaobao.xyz/Article/details/gawmrwqis.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.fanxiaobao.xyz/Article/details/grrnhmeuh.sHtML

[R24] 大小写转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnqlggbur.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.fanxiaobao.xyz/Article/details/guazyfinr.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goqjhxqvj.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gsjmpwoen.sHtML

[R26] 命令替换
来源：http://mobile.fanxiaobao.xyz/Article/details/ghlnzmcrt.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.fanxiaobao.xyz/Article/details/gcuudulcf.sHtML

[R27] 算术展开
来源：http://3g.fanxiaobao.xyz/Article/details/gsdxmlpac.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtiniugvm.sHtML

[R28] 浮点运算
来源：http://wap.fanxiaobao.xyz/Article/details/gjvjjpeag.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.fanxiaobao.xyz/Article/details/gasdvevlc.sHtML

[R29] 定义函数
来源：http://baike.fanxiaobao.xyz/Article/details/gwavkjvbk.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.fanxiaobao.xyz/Article/details/gifbqstki.sHtML

[R30] 函数返回状态码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gttvzsylq.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.fanxiaobao.xyz/Article/details/gecvsegrc.sHtML

[R31] 局部变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gwtahibrv.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gujluupwe.sHtML

[R32] 参数个数校验
来源：http://read.share.fanxiaobao.xyz/Article/details/gtnydggzq.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gnqkvvwkc.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.fanxiaobao.xyz/Article/details/gifdfzxgg.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.fanxiaobao.xyz/Article/details/gwbicbhgj.sHtML

[R34] 退出时清理
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmsuwgizh.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fanxiaobao.xyz/Article/details/gmenotqsu.sHtML

[R35] 后台执行并等待
来源：http://read.share.fanxiaobao.xyz/Article/details/gwygjzhtp.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.fanxiaobao.xyz/Article/details/gbsajadky.sHtML

[R36] 并发执行多个任务
来源：http://mobile.fanxiaobao.xyz/Article/details/gipqutxem.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzsrfaevs.sHtML

[R37] 把输出赋给变量
来源：http://mobile.fanxiaobao.xyz/Article/details/godkhcbxt.sHtML

files=$(ls -1)
来源：http://baike.fanxiaobao.xyz/Article/details/gyxxzqzaq.sHtML

[R38] 管道串联
来源：http://baike.fanxiaobao.xyz/Article/details/gqtkmxnns.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.fanxiaobao.xyz/Article/details/gauetmnjl.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.fanxiaobao.xyz/Article/details/giypnlqhr.sHtML

cmd > out.log 2>&1
来源：http://blog.fanxiaobao.xyz/Article/details/gdkegubnv.sHtML

[R40] 追加写日志
来源：http://read.share.fanxiaobao.xyz/Article/details/gyhrpkbyd.sHtML

echo "log" >> out.log
来源：http://3g.fanxiaobao.xyz/Article/details/gexbzigzt.sHtML

[R41] 丢弃输出
来源：http://read.share.fanxiaobao.xyz/Article/details/gximqsdub.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.fanxiaobao.xyz/Article/details/gylpwtzqu.sHtML

[R42] 输入重定向
来源：http://mobile.fanxiaobao.xyz/Article/details/gtmiikjou.sHtML

wc -l < a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gcjzymiep.sHtML

[R43] 按名字查找文件
来源：http://blog.fanxiaobao.xyz/Article/details/gwjsnngzo.sHtML

find . -name "*.log" -type f
来源：http://www.share.fanxiaobao.xyz/Article/details/gngduohzl.sHtML

[R44] 按修改时间查找
来源：http://baike.fanxiaobao.xyz/Article/details/geddivxju.sHtML

find . -mtime -7 -type f
来源：http://wap.fanxiaobao.xyz/Article/details/guozgxdko.sHtML

[R45] 批量删除
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyvbfhupk.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.fanxiaobao.xyz/Article/details/gztwhfgha.sHtML

[R46] 递归替换文件内容
来源：http://read.share.fanxiaobao.xyz/Article/details/gawynrdji.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.fanxiaobao.xyz/Article/details/gwaqtfcjq.sHtML

[R47] sed 单行替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gwzgiwjfq.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gtyhomjiz.sHtML

[R48] awk 取指定列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gginkfooi.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsbgysvxb.sHtML

[R49] awk 带条件
来源：http://baike.fanxiaobao.xyz/Article/details/gyuxmnstg.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.fanxiaobao.xyz/Article/details/gjnrftmzj.sHtML

[R50] awk 求和
来源：http://m.share.fanxiaobao.xyz/Article/details/gmwfltlyw.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gfnjympil.sHtML

[R51] 排序去重取前几
来源：http://blog.fanxiaobao.xyz/Article/details/gbmcerete.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.fanxiaobao.xyz/Article/details/gsddkbajp.sHtML

[R52] 统计行数
来源：http://m.share.fanxiaobao.xyz/Article/details/gsqakixde.sHtML

wc -l a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcgdsttys.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.fanxiaobao.xyz/Article/details/gtcdzqbma.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.fanxiaobao.xyz/Article/details/gkakswcoo.sHtML

[R54] 比较两个文件
来源：http://baike.fanxiaobao.xyz/Article/details/gstxtjrjf.sHtML

diff a.txt b.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gprcjzdkw.sHtML

[R55] 压缩与解压
来源：http://read.share.fanxiaobao.xyz/Article/details/gcocexafz.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.fanxiaobao.xyz/Article/details/guzprlzfk.sHtML

[R56] 远程拷贝
来源：http://read.share.fanxiaobao.xyz/Article/details/gkabvmrbn.sHtML

scp file user@host:/path/
来源：http://mobile.fanxiaobao.xyz/Article/details/ggpgygupg.sHtML

[R57] 远程执行命令
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghulyynld.sHtML

ssh user@host 'uptime'
来源：http://blog.fanxiaobao.xyz/Article/details/gtfhwdivr.sHtML

[R58] 下载文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gnkfldbud.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.fanxiaobao.xyz/Article/details/glfydrhih.sHtML

[R59] 发 POST JSON
来源：http://m.share.fanxiaobao.xyz/Article/details/gxrswqcpb.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.fanxiaobao.xyz/Article/details/gcixinmls.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.fanxiaobao.xyz/Article/details/gdwbftowy.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.fanxiaobao.xyz/Article/details/ggorwjgon.sHtML

[R61] 磁盘占用
来源：http://read.share.fanxiaobao.xyz/Article/details/ggqohhuze.sHtML

df -h;  du -sh *
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfrufpaff.sHtML

[R62] 找最占空间的文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gvlnjtaer.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.fanxiaobao.xyz/Article/details/ggjjtcxwo.sHtML

[R63] 内存与进程
来源：http://m.share.fanxiaobao.xyz/Article/details/geufpgxzc.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.fanxiaobao.xyz/Article/details/geksrxuko.sHtML

[R64] 结束进程
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzgywlpyn.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.fanxiaobao.xyz/Article/details/gbozotsoq.sHtML

[R65] 查看端口占用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcdwbrajg.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.fanxiaobao.xyz/Article/details/gpbzvfgvk.sHtML

[R66] 定时任务
来源：http://m.share.fanxiaobao.xyz/Article/details/gnadffpwj.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grbjqmlmf.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkjstlddv.sHtML

openssl rand -hex 16
来源：http://m.share.fanxiaobao.xyz/Article/details/gsifmiiad.sHtML

[R68] 计算文件校验值
来源：http://m.share.fanxiaobao.xyz/Article/details/guuishetd.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfjvcpiee.sHtML

[R69] 生成随机密码
来源：http://blog.fanxiaobao.xyz/Article/details/gsetvjbyh.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.fanxiaobao.xyz/Article/details/gvgdccaov.sHtML

[R70] 时间戳与互转
来源：http://read.share.fanxiaobao.xyz/Article/details/gikzfevlv.sHtML

date +%s;  date -d @1700000000
来源：http://wap.fanxiaobao.xyz/Article/details/gnntfejpa.sHtML

[R71] 日期格式化
来源：http://mobile.fanxiaobao.xyz/Article/details/gaqkfmert.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbabjbicl.sHtML

[R72] 等待端口就绪
来源：http://3g.fanxiaobao.xyz/Article/details/gnicmyzqy.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.fanxiaobao.xyz/Article/details/gomznahck.sHtML

[R73] 分割大日志
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glurrelhu.sHtML

split -l 1000 big.log part_
来源：http://blog.fanxiaobao.xyz/Article/details/gcmqmmkgk.sHtML

[R74] 批量重命名
来源：http://3g.fanxiaobao.xyz/Article/details/ggyddvtjp.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gpposnniv.sHtML

[R75] 导出环境变量
来源：http://3g.fanxiaobao.xyz/Article/details/gpgeoolws.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.fanxiaobao.xyz/Article/details/gjeqywlmt.sHtML

[R76] 使用临时文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gaaqrziln.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.fanxiaobao.xyz/Article/details/gzpeeybvm.sHtML

[R77] 读取用户输入
来源：http://www.share.fanxiaobao.xyz/Article/details/gbdttcfpj.sHtML

read -rp "请输入: " ans
来源：http://mobile.fanxiaobao.xyz/Article/details/gxdxhmeqr.sHtML

[R78] 交互式菜单
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtswszapy.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gbchqctct.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gadzokpsn.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmfqccmkb.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.fanxiaobao.xyz/Article/details/glqprhtlm.sHtML

time ./run.sh
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvwntglbg.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gahsobynf.sHtML

S. C / C++ 专题
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gorjrnrdw.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfmzsdzxg.sHtML

[S01] C：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/grethddru.sHtML

#include <stdio.h>
来源：http://read.share.fanxiaobao.xyz/Article/details/gavsvjaha.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.fanxiaobao.xyz/Article/details/gqiatvojk.sHtML

[S02] C：变量与格式化输出
来源：http://blog.fanxiaobao.xyz/Article/details/gaxhbluld.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.fanxiaobao.xyz/Article/details/gwiqcarrp.sHtML

[S03] C：读入整数
来源：http://wap.fanxiaobao.xyz/Article/details/gidsoqmnl.sHtML

int x; scanf("%d", &x);
来源：http://mobile.fanxiaobao.xyz/Article/details/gqnpscmbk.sHtML

[S04] C：字符串复制
来源：http://wap.fanxiaobao.xyz/Article/details/gwoggydku.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkayzikec.sHtML

[S05] C：字符串长度
来源：http://baike.fanxiaobao.xyz/Article/details/gisrdkjhv.sHtML

strlen(s)
来源：http://3g.fanxiaobao.xyz/Article/details/gclwpsrdo.sHtML

[S06] C：字符串比较
来源：http://baike.fanxiaobao.xyz/Article/details/gsstleqbw.sHtML

strcmp(a, b) == 0
来源：http://3g.fanxiaobao.xyz/Article/details/gfeppymek.sHtML

[S07] C：数组遍历求和
来源：http://mobile.fanxiaobao.xyz/Article/details/grhivblaj.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdaphdgps.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.fanxiaobao.xyz/Article/details/gmhnzygwn.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.fanxiaobao.xyz/Article/details/gyopjbfuj.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.fanxiaobao.xyz/Article/details/gkhjbupik.sHtML


<!-- 参考信息 -->