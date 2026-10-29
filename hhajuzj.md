代发 wailian999

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.fehbvm.com/Article/details/gulesmfev.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://blog.zdbjq.cn/Article/details/gbthwkkoc.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://3g.zdbjq.cn/Article/details/geupaylsq.sHtML

[Q41] 多表连接
来源：http://www.blog.fehbvm.com/Article/details/gzsmdgtzl.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.blog.zdbjq.cn/Article/details/guasyycjn.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.zdbjq.cn/Article/details/gkvbemuhp.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://read.share.zdbjq.cn/Article/details/glqdbspdo.sHtML

[Q42] 连接条件附加过滤
来源：http://baike.hesvh.cn/Article/details/gsaviraju.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.blog.zdbjq.cn/Article/details/glakkqawp.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.hesvh.cn/Article/details/gnktctuqg.sHtML

[Q43] 标量子查询
来源：http://m.share.fehbvm.com/Article/details/gbhxrxzdt.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.hesvh.cn/Article/details/gaqhqtepm.sHtML

[Q44] IN 子查询
来源：http://www.blog.hesvh.cn/Article/details/gcpjmidpi.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://read.share.hesvh.cn/Article/details/giprovrmn.sHtML

[Q45] EXISTS 判断存在
来源：http://www.blog.hesvh.cn/Article/details/gqofhveaa.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.fehbvm.com/Article/details/gxpezostz.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://3g.zdbjq.cn/Article/details/grqgullvs.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.hesvh.cn/Article/details/gcagayghg.sHtML

[Q47] 与平均值比较
来源：http://www.blog.hesvh.cn/Article/details/gyehwtoph.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mobile.hesvh.cn/Article/details/gghtelsus.sHtML

[Q48] CTE 公用表表达式
来源：http://www.share.fehbvm.com/Article/details/gxnjqaeya.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.share.hesvh.cn/Article/details/ggmkkowxy.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.fehbvm.com/Article/details/gpuvlluwu.sHtML

[Q49] 更新单行
来源：http://mobile.zdbjq.cn/Article/details/gwhwcauws.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://m.share.hesvh.cn/Article/details/guckfsytd.sHtML

[Q50] 批量更新
来源：http://mobile.fehbvm.com/Article/details/gmctmkqku.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.blog.fehbvm.com/Article/details/gewtrfsdy.sHtML

[Q51] 用子查询更新
来源：http://www.blog.hesvh.cn/Article/details/gnqtolsoc.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://3g.fehbvm.com/Article/details/gsfzffbsh.sHtML

[Q52] 删除指定行
来源：http://mobile.fehbvm.com/Article/details/gmguxwcoz.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.hesvh.cn/Article/details/gapwahwnr.sHtML

[Q53] 按条件删除
来源：http://www.blog.hesvh.cn/Article/details/gprfmmwll.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://3g.zdbjq.cn/Article/details/ghklgpofe.sHtML

[Q54] 清空表
来源：http://baike.hesvh.cn/Article/details/gchlqnnwb.sHtML

TRUNCATE TABLE logs;
来源：http://wap.hesvh.cn/Article/details/gtjfhlqsp.sHtML

[Q55] 排名（并列占位）
来源：http://blog.zdbjq.cn/Article/details/gesnkqupn.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mobile.fehbvm.com/Article/details/geoxqhpam.sHtML

[Q56] 密集排名（并列不占位）
来源：http://mobile.zdbjq.cn/Article/details/gjcospmey.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.blog.hesvh.cn/Article/details/girellhme.sHtML

[Q57] 行号
来源：http://3g.fehbvm.com/Article/details/gzphjrptx.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.fehbvm.com/Article/details/gadtkhsgs.sHtML

[Q58] 累计求和
来源：http://3g.hesvh.cn/Article/details/gkegxdxzz.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/gqywkedvd.sHtML

[Q59] 分组内累计
来源：http://www.blog.hesvh.cn/Article/details/ghcggkyfm.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/ganijfqbf.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.hesvh.cn/Article/details/glzoacxjq.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.fehbvm.com/Article/details/grnniamlv.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.hesvh.cn/Article/details/grcbozngj.sHtML

[Q61] 移动平均
来源：http://baike.hesvh.cn/Article/details/guoulbdgz.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://blog.zdbjq.cn/Article/details/giusikuom.sHtML

[Q62] 分组占比
来源：http://baike.zdbjq.cn/Article/details/gtfkihple.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.zdbjq.cn/Article/details/gecdopdua.sHtML

[Q63] 开启事务
来源：http://read.share.hesvh.cn/Article/details/gxmuzkoor.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://3g.hesvh.cn/Article/details/gtcpyqwwd.sHtML

[Q64] 提交事务
来源：http://m.share.zdbjq.cn/Article/details/gysvszoql.sHtML

COMMIT;
来源：http://mobile.zdbjq.cn/Article/details/grsivmifg.sHtML

[Q65] 回滚事务
来源：http://blog.zdbjq.cn/Article/details/gqhkzjqoh.sHtML

ROLLBACK;
来源：http://3g.hesvh.cn/Article/details/gifkbgrum.sHtML

[Q66] 行锁查询
来源：http://blog.hesvh.cn/Article/details/gwdovtxeu.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.blog.hesvh.cn/Article/details/gbgpgsfuk.sHtML

[Q67] 设置隔离级别
来源：http://wap.fehbvm.com/Article/details/gndctkcag.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.zdbjq.cn/Article/details/gwplggyjz.sHtML

[Q68] 保存点
来源：http://m.share.hesvh.cn/Article/details/gtzftlhni.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.fehbvm.com/Article/details/gfkojnuux.sHtML

ROLLBACK TO sp1;
来源：http://m.share.fehbvm.com/Article/details/gsxseesfu.sHtML

[Q69] 查看执行计划
来源：http://wap.hesvh.cn/Article/details/gliwatlsh.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.share.hesvh.cn/Article/details/gawrrvswd.sHtML

[Q70] 更新统计信息
来源：http://baike.zdbjq.cn/Article/details/gxfoozuwh.sHtML

ANALYZE TABLE users;
来源：http://3g.zdbjq.cn/Article/details/gehczesyj.sHtML

[Q71] 查看建表语句
来源：http://www.share.zdbjq.cn/Article/details/gzkvlywes.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.hesvh.cn/Article/details/gekwfkchg.sHtML

[Q72] 查看索引
来源：http://www.m.share.fehbvm.com/Article/details/gvybbftwq.sHtML

SHOW INDEX FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gpyxwjkiz.sHtML

[Q73] 查看表状态
来源：http://www.m.share.hesvh.cn/Article/details/gqcriktdx.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://read.share.fehbvm.com/Article/details/gmrtqizro.sHtML

[Q74] 强制使用索引
来源：http://m.share.zdbjq.cn/Article/details/gliuzotam.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.zdbjq.cn/Article/details/gqybcnwza.sHtML

[Q75] 日期格式化
来源：http://m.share.hesvh.cn/Article/details/gdmqdbebr.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://m.share.fehbvm.com/Article/details/gdexkvacp.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.blog.zdbjq.cn/Article/details/grptmhzts.sHtML

[Q76] 按天统计
来源：http://www.m.share.fehbvm.com/Article/details/gfngzxhru.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.hesvh.cn/Article/details/gxaqxxfpq.sHtML

[Q77] 时间加减
来源：http://blog.hesvh.cn/Article/details/gglqzwlhy.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.hesvh.cn/Article/details/gdbezdiqk.sHtML

[Q78] 当前时间
来源：http://www.m.share.fehbvm.com/Article/details/gmgpirrcs.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.zdbjq.cn/Article/details/gtlsfocus.sHtML

[Q79] 字符串拼接
来源：http://baike.fehbvm.com/Article/details/giugshpkm.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.zdbjq.cn/Article/details/gcbzrckjp.sHtML

[Q80] 字符串截取
来源：http://www.share.zdbjq.cn/Article/details/gcgujjkas.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/ghahwhgof.sHtML

[Q81] 字符串替换
来源：http://3g.hesvh.cn/Article/details/grjzxcdwa.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gjacazmxl.sHtML

[Q82] 字符长度与字节长度
来源：http://mobile.hesvh.cn/Article/details/gexfpgssq.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wap.hesvh.cn/Article/details/gqxguyyqk.sHtML

[Q83] 大小写转换
来源：http://www.blog.zdbjq.cn/Article/details/gkfcuneqx.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gykcudrup.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.zdbjq.cn/Article/details/gbqlvaafq.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.hesvh.cn/Article/details/gbmzqmpav.sHtML

[Q85] 数值取整
来源：http://mobile.zdbjq.cn/Article/details/grtipigax.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.fehbvm.com/Article/details/gfxoqmqgr.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.zdbjq.cn/Article/details/gufnwznah.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.fehbvm.com/Article/details/gfnpahlpu.sHtML

[Q87] JSON 字段做条件
来源：http://3g.hesvh.cn/Article/details/ghfrntlrx.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.zdbjq.cn/Article/details/gemzvwhrr.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.fehbvm.com/Article/details/gnkntbmse.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://3g.zdbjq.cn/Article/details/grmcetlkh.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.hesvh.cn/Article/details/gnpzormom.sHtML

[Q89] 判断表是否存在
来源：http://baike.hesvh.cn/Article/details/gbvswexuz.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.fehbvm.com/Article/details/gevrzmnze.sHtML

[Q90] 生成序号列
来源：http://read.share.hesvh.cn/Article/details/gyvbygaze.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.zdbjq.cn/Article/details/gwqysjwpd.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gkddvdbti.sHtML

R. Bash 专题
来源：http://www.blog.fehbvm.com/Article/details/gthhbavjz.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gnpvshxyl.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.zdbjq.cn/Article/details/gszdcpdvv.sHtML

#!/usr/bin/env bash
来源：http://www.blog.zdbjq.cn/Article/details/grosslmvu.sHtML

set -euo pipefail
来源：http://www.m.share.fehbvm.com/Article/details/gjkplsqks.sHtML

[R02] 变量赋值与使用
来源：http://wap.zdbjq.cn/Article/details/gekoirxgg.sHtML

name="Tom"; echo "$name"
来源：http://3g.fehbvm.com/Article/details/guemcfluf.sHtML

[R03] 只读变量
来源：http://wap.fehbvm.com/Article/details/gfqztiqid.sHtML

readonly PI=3.14
来源：http://wap.zdbjq.cn/Article/details/gmzlgsvbg.sHtML

[R04] 位置参数
来源：http://3g.zdbjq.cn/Article/details/galhfemnp.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.zdbjq.cn/Article/details/gyheubidm.sHtML

[R05] 参数默认值
来源：http://www.blog.fehbvm.com/Article/details/gavrbkgyl.sHtML

name="${1:-default}"
来源：http://3g.hesvh.cn/Article/details/gvoqvmkar.sHtML

[R06] 判断命令是否存在
来源：http://3g.hesvh.cn/Article/details/gdekfxfev.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.m.share.fehbvm.com/Article/details/gshfntzro.sHtML

[R07] if 判断文件
来源：http://www.share.zdbjq.cn/Article/details/gbcohfamf.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.fehbvm.com/Article/details/gjsflqlfo.sHtML

[R08] 数值比较
来源：http://wap.fehbvm.com/Article/details/gkmjrihdb.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.zdbjq.cn/Article/details/giuaayoev.sHtML

[R09] 字符串比较
来源：http://www.m.share.fehbvm.com/Article/details/gbvqtngxj.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.hesvh.cn/Article/details/gbwmpbwzg.sHtML

[R10] 正则匹配
来源：http://www.share.hesvh.cn/Article/details/giwbvpejc.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.zdbjq.cn/Article/details/gswxynjge.sHtML

[R11] case 多分支
来源：http://www.blog.zdbjq.cn/Article/details/gbcqhkdhe.sHtML

case "$1" in
来源：http://3g.fehbvm.com/Article/details/gwhycrufj.sHtML

start) echo "启动" ;;
来源：http://wap.zdbjq.cn/Article/details/ggqrkqxpy.sHtML

stop)  echo "停止" ;;
来源：http://blog.hesvh.cn/Article/details/gywvhwsxy.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.zdbjq.cn/Article/details/gnvawipoq.sHtML

esac
来源：http://www.blog.fehbvm.com/Article/details/gctonabde.sHtML

[R12] for 遍历文件
来源：http://wap.fehbvm.com/Article/details/gixytgqyx.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.hesvh.cn/Article/details/gtolxqxxb.sHtML

[R13] for 计数循环
来源：http://baike.hesvh.cn/Article/details/gghdqschd.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.fehbvm.com/Article/details/ggoygwzmk.sHtML

[R14] C 风格 for
来源：http://www.m.share.fehbvm.com/Article/details/gkyslktdy.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.fehbvm.com/Article/details/gxgnyehzk.sHtML

[R15] while 逐行读文件
来源：http://baike.hesvh.cn/Article/details/gljjvwfzw.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.fehbvm.com/Article/details/gnwgfodyi.sHtML

[R16] until 等待条件
来源：http://m.share.zdbjq.cn/Article/details/gbszhjmfi.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.fehbvm.com/Article/details/grhtqycop.sHtML

[R17] 数组定义与取值
来源：http://read.share.fehbvm.com/Article/details/gguuphxmi.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.hesvh.cn/Article/details/gvflamnfd.sHtML

[R18] 遍历数组
来源：http://www.blog.zdbjq.cn/Article/details/gegyapjis.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.hesvh.cn/Article/details/gvtdbjetw.sHtML

[R19] 数组长度
来源：http://wap.zdbjq.cn/Article/details/gdsawnhnw.sHtML

echo "${#arr[@]}"
来源：http://blog.fehbvm.com/Article/details/gcteqdvgc.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.fehbvm.com/Article/details/gpmqlmyot.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.hesvh.cn/Article/details/glqgpxztr.sHtML

[R21] 字符串长度
来源：http://baike.fehbvm.com/Article/details/gkddxjknf.sHtML

echo "${#s}"
来源：http://mobile.hesvh.cn/Article/details/guuyubpyx.sHtML

[R22] 截取子串
来源：http://read.share.hesvh.cn/Article/details/gvktrskhk.sHtML

echo "${s:0:5}"
来源：http://m.share.zdbjq.cn/Article/details/gyvvytegb.sHtML

[R23] 字符串替换
来源：http://baike.fehbvm.com/Article/details/gissbggxy.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.hesvh.cn/Article/details/gmovhmybn.sHtML

[R24] 大小写转换
来源：http://m.share.hesvh.cn/Article/details/gfybsvxht.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.fehbvm.com/Article/details/gebwirwkn.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.hesvh.cn/Article/details/glxqffusa.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.hesvh.cn/Article/details/gqwsfuieg.sHtML

[R26] 命令替换
来源：http://www.share.hesvh.cn/Article/details/gxznamvtj.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.hesvh.cn/Article/details/gpvcvbrra.sHtML

[R27] 算术展开
来源：http://www.blog.fehbvm.com/Article/details/gsllbxpcp.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.hesvh.cn/Article/details/glkrfufdl.sHtML

[R28] 浮点运算
来源：http://wap.fehbvm.com/Article/details/gmtcvqeqb.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.zdbjq.cn/Article/details/ghrxekyov.sHtML

[R29] 定义函数
来源：http://baike.hesvh.cn/Article/details/goytphfof.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.zdbjq.cn/Article/details/gfdtvxaxy.sHtML

[R30] 函数返回状态码
来源：http://read.share.hesvh.cn/Article/details/gvlgsidvt.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.hesvh.cn/Article/details/gbgbtlanv.sHtML

[R31] 局部变量
来源：http://baike.zdbjq.cn/Article/details/gqlifdlgt.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.zdbjq.cn/Article/details/gigtuygao.sHtML

[R32] 参数个数校验
来源：http://wap.fehbvm.com/Article/details/gskrrcses.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.fehbvm.com/Article/details/godbxpusq.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.hesvh.cn/Article/details/gquaznhkt.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.fehbvm.com/Article/details/gkjkhyinq.sHtML

[R34] 退出时清理
来源：http://read.share.hesvh.cn/Article/details/gynoqvupk.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.hesvh.cn/Article/details/ghvirtqew.sHtML

[R35] 后台执行并等待
来源：http://mobile.fehbvm.com/Article/details/gqpmccmvf.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.fehbvm.com/Article/details/gyfocdacm.sHtML

[R36] 并发执行多个任务
来源：http://mobile.fehbvm.com/Article/details/gysookijv.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.hesvh.cn/Article/details/gjcewuttk.sHtML

[R37] 把输出赋给变量
来源：http://blog.hesvh.cn/Article/details/gzaomqecw.sHtML

files=$(ls -1)
来源：http://www.m.share.hesvh.cn/Article/details/gqpxqzwde.sHtML

[R38] 管道串联
来源：http://3g.zdbjq.cn/Article/details/gvqyxcfmv.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.zdbjq.cn/Article/details/gyqowtkfj.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.zdbjq.cn/Article/details/gltmvchjf.sHtML

cmd > out.log 2>&1
来源：http://3g.zdbjq.cn/Article/details/gmyoqzaqr.sHtML

[R40] 追加写日志
来源：http://mobile.zdbjq.cn/Article/details/guzwakykk.sHtML

echo "log" >> out.log
来源：http://m.share.zdbjq.cn/Article/details/glkrwhwlb.sHtML

[R41] 丢弃输出
来源：http://www.m.share.zdbjq.cn/Article/details/gsahfoslk.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.zdbjq.cn/Article/details/gcuwokngm.sHtML

[R42] 输入重定向
来源：http://www.blog.hesvh.cn/Article/details/grhahwiha.sHtML

wc -l < a.txt
来源：http://read.share.fehbvm.com/Article/details/grjzduevu.sHtML

[R43] 按名字查找文件
来源：http://www.share.hesvh.cn/Article/details/gixkkhges.sHtML

find . -name "*.log" -type f
来源：http://read.share.fehbvm.com/Article/details/gvybjdwgf.sHtML

[R44] 按修改时间查找
来源：http://wap.fehbvm.com/Article/details/gnnohfanb.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.zdbjq.cn/Article/details/grxdnmllk.sHtML

[R45] 批量删除
来源：http://read.share.zdbjq.cn/Article/details/geaepccnh.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.fehbvm.com/Article/details/ghqpmvrgd.sHtML

[R46] 递归替换文件内容
来源：http://3g.zdbjq.cn/Article/details/gebjelgvz.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.hesvh.cn/Article/details/goxxxmepy.sHtML

[R47] sed 单行替换
来源：http://www.blog.fehbvm.com/Article/details/gqeqagsbj.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.fehbvm.com/Article/details/gubxxhnau.sHtML

[R48] awk 取指定列
来源：http://www.share.hesvh.cn/Article/details/gcvibtuhl.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.hesvh.cn/Article/details/gqqverpkx.sHtML

[R49] awk 带条件
来源：http://3g.hesvh.cn/Article/details/gconheknq.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.hesvh.cn/Article/details/ghqpvxmdz.sHtML

[R50] awk 求和
来源：http://mobile.zdbjq.cn/Article/details/gglbodxhf.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.fehbvm.com/Article/details/getmxxneg.sHtML

[R51] 排序去重取前几
来源：http://www.blog.hesvh.cn/Article/details/gvfzlfzpf.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.hesvh.cn/Article/details/gltjejhgs.sHtML

[R52] 统计行数
来源：http://m.share.fehbvm.com/Article/details/gpyjmsowa.sHtML

wc -l a.txt
来源：http://wap.fehbvm.com/Article/details/gusdyzzgn.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.fehbvm.com/Article/details/gepnvfokb.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.fehbvm.com/Article/details/gswojohwr.sHtML

[R54] 比较两个文件
来源：http://wap.fehbvm.com/Article/details/gazqyqzua.sHtML

diff a.txt b.txt
来源：http://baike.zdbjq.cn/Article/details/geafvnyhb.sHtML

[R55] 压缩与解压
来源：http://www.blog.zdbjq.cn/Article/details/ggjohaljd.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.zdbjq.cn/Article/details/gylzspfvi.sHtML

[R56] 远程拷贝
来源：http://wap.fehbvm.com/Article/details/giwoegnhu.sHtML

scp file user@host:/path/
来源：http://baike.fehbvm.com/Article/details/gmkdvdlrx.sHtML

[R57] 远程执行命令
来源：http://www.share.hesvh.cn/Article/details/gzbrsabzd.sHtML

ssh user@host 'uptime'
来源：http://wap.hesvh.cn/Article/details/gcgeiftfg.sHtML

[R58] 下载文件
来源：http://wap.zdbjq.cn/Article/details/gkpdcwfya.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.hesvh.cn/Article/details/gwrerdteo.sHtML

[R59] 发 POST JSON
来源：http://mobile.fehbvm.com/Article/details/goplhlzbi.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.fehbvm.com/Article/details/gozkcwswz.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.fehbvm.com/Article/details/geqzqyeax.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.zdbjq.cn/Article/details/ghaxjjcxq.sHtML

[R61] 磁盘占用
来源：http://baike.fehbvm.com/Article/details/grglmtpxt.sHtML

df -h;  du -sh *
来源：http://mobile.hesvh.cn/Article/details/gprkjfomw.sHtML

[R62] 找最占空间的文件
来源：http://m.share.fehbvm.com/Article/details/gupopatgn.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.hesvh.cn/Article/details/gwvoqzedx.sHtML

[R63] 内存与进程
来源：http://m.share.zdbjq.cn/Article/details/gsrqxdcod.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.fehbvm.com/Article/details/gmljilisn.sHtML

[R64] 结束进程
来源：http://baike.fehbvm.com/Article/details/gjulpnrqw.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.fehbvm.com/Article/details/gdjwzhnyk.sHtML

[R65] 查看端口占用
来源：http://www.blog.hesvh.cn/Article/details/gtdsjfejq.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.fehbvm.com/Article/details/gprnydjzb.sHtML

[R66] 定时任务
来源：http://www.share.zdbjq.cn/Article/details/gusapjdir.sHtML

crontab -e;  crontab -l
来源：http://3g.hesvh.cn/Article/details/gqyubaqmq.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.hesvh.cn/Article/details/gcgbnpmxm.sHtML

openssl rand -hex 16
来源：http://baike.zdbjq.cn/Article/details/gempwvznc.sHtML

[R68] 计算文件校验值
来源：http://mobile.fehbvm.com/Article/details/ggjsohmtc.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.zdbjq.cn/Article/details/gwjkwnuvy.sHtML

[R69] 生成随机密码
来源：http://www.m.share.fehbvm.com/Article/details/gwrbetnva.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.fehbvm.com/Article/details/grjnlfvda.sHtML

[R70] 时间戳与互转
来源：http://www.blog.hesvh.cn/Article/details/gtrhbcjbx.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.zdbjq.cn/Article/details/gnvmqxsjf.sHtML

[R71] 日期格式化
来源：http://www.blog.hesvh.cn/Article/details/gbvexqdah.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.zdbjq.cn/Article/details/gdttssolc.sHtML

[R72] 等待端口就绪
来源：http://read.share.zdbjq.cn/Article/details/gxxozhmza.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.zdbjq.cn/Article/details/gbdgqzoqh.sHtML

[R73] 分割大日志
来源：http://m.share.hesvh.cn/Article/details/gqhgdvxuj.sHtML

split -l 1000 big.log part_
来源：http://3g.zdbjq.cn/Article/details/gbxtodrbl.sHtML

[R74] 批量重命名
来源：http://www.share.zdbjq.cn/Article/details/gpqcuawmv.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.hesvh.cn/Article/details/gjsmssgzf.sHtML

[R75] 导出环境变量
来源：http://wap.zdbjq.cn/Article/details/gmbsdfvbz.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.hesvh.cn/Article/details/gqxhgbteh.sHtML

[R76] 使用临时文件
来源：http://mobile.fehbvm.com/Article/details/grepjkrhh.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.zdbjq.cn/Article/details/gpexlygpf.sHtML

[R77] 读取用户输入
来源：http://m.share.fehbvm.com/Article/details/gcqbiuhgb.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.zdbjq.cn/Article/details/gamhltxpy.sHtML

[R78] 交互式菜单
来源：http://wap.fehbvm.com/Article/details/gyzkhexyd.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.hesvh.cn/Article/details/gkzmiehoc.sHtML

[R79] 解析命令行选项
来源：http://3g.hesvh.cn/Article/details/geymeyxhj.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.zdbjq.cn/Article/details/gjixyrbhk.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.zdbjq.cn/Article/details/grwddvhse.sHtML

time ./run.sh
来源：http://blog.fehbvm.com/Article/details/gemucdduf.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gervupjok.sHtML

S. C / C++ 专题
来源：http://wap.zdbjq.cn/Article/details/gqhgnhnjj.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gvihkphgl.sHtML

[S01] C：Hello World
来源：http://www.share.fehbvm.com/Article/details/gerwhgtjx.sHtML

#include <stdio.h>
来源：http://m.share.zdbjq.cn/Article/details/gnbuvjesl.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.hesvh.cn/Article/details/gihceezlz.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.hesvh.cn/Article/details/gxgcybqtc.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.hesvh.cn/Article/details/geqzrocem.sHtML

[S03] C：读入整数
来源：http://baike.zdbjq.cn/Article/details/gledzrluf.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.fehbvm.com/Article/details/grstrsfab.sHtML

[S04] C：字符串复制
来源：http://www.blog.fehbvm.com/Article/details/ghqtsbbxa.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.zdbjq.cn/Article/details/gstldhdyu.sHtML

[S05] C：字符串长度
来源：http://blog.zdbjq.cn/Article/details/gcawiqmqi.sHtML

strlen(s)
来源：http://baike.hesvh.cn/Article/details/gshvdpfnn.sHtML

[S06] C：字符串比较
来源：http://3g.hesvh.cn/Article/details/grdqudupq.sHtML

strcmp(a, b) == 0
来源：http://blog.fehbvm.com/Article/details/ghzyxdhdg.sHtML

[S07] C：数组遍历求和
来源：http://m.share.zdbjq.cn/Article/details/gaytrqcux.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.zdbjq.cn/Article/details/gmpwzwfic.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.hesvh.cn/Article/details/gnfyjxakw.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.fehbvm.com/Article/details/gehvmnyrb.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.fehbvm.com/Article/details/gighprvsw.sHtML


<!-- 参考信息 -->