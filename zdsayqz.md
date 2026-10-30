代发 wailian999

SELECT u.name, o.amount FROM users u
来源：http://m.share.fanxiaobao.xyz/Article/details/gfeykmeao.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmlgsjgqy.sHtML

[Q43] 标量子查询
来源：http://wap.fanxiaobao.xyz/Article/details/gekndatwl.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wap.fanxiaobao.xyz/Article/details/gjcrrmjma.sHtML

[Q44] IN 子查询
来源：http://www.share.fanxiaobao.xyz/Article/details/gucaexdnr.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gekdxgxxr.sHtML

[Q45] EXISTS 判断存在
来源：http://wap.fanxiaobao.xyz/Article/details/gpqnzmqxn.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.fanxiaobao.xyz/Article/details/gsskuzrzo.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.fanxiaobao.xyz/Article/details/gcileehdk.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.fanxiaobao.xyz/Article/details/gmfmrsuah.sHtML

[Q47] 与平均值比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giarlhzig.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://baike.fanxiaobao.xyz/Article/details/gkwpcuznu.sHtML

[Q48] CTE 公用表表达式
来源：http://baike.fanxiaobao.xyz/Article/details/geqioiyow.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://3g.fanxiaobao.xyz/Article/details/giiiyamcy.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://wap.fanxiaobao.xyz/Article/details/gyvhlarzh.sHtML

[Q49] 更新单行
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxgmqyuis.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://3g.fanxiaobao.xyz/Article/details/gmwiljbwr.sHtML

[Q50] 批量更新
来源：http://3g.fanxiaobao.xyz/Article/details/gmbwtwnvu.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzxyjokbs.sHtML

[Q51] 用子查询更新
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gerwspngv.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/ginpaclqe.sHtML

[Q52] 删除指定行
来源：http://3g.fanxiaobao.xyz/Article/details/gjhgxuoli.sHtML

DELETE FROM users WHERE id = 10;
来源：http://blog.fanxiaobao.xyz/Article/details/gkbbbkyqc.sHtML

[Q53] 按条件删除
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geceribxu.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.fanxiaobao.xyz/Article/details/gekyliewh.sHtML

[Q54] 清空表
来源：http://3g.fanxiaobao.xyz/Article/details/grpstyxxn.sHtML

TRUNCATE TABLE logs;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfttlyndd.sHtML

[Q55] 排名（并列占位）
来源：http://3g.fanxiaobao.xyz/Article/details/gfvnnfeby.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmrludnuh.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.fanxiaobao.xyz/Article/details/guyzobbxl.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mobile.fanxiaobao.xyz/Article/details/gqjhuittn.sHtML

[Q57] 行号
来源：http://3g.fanxiaobao.xyz/Article/details/goynpjdto.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/govijmgfu.sHtML

[Q58] 累计求和
来源：http://read.share.fanxiaobao.xyz/Article/details/guihofifu.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wap.fanxiaobao.xyz/Article/details/gcbhxjwok.sHtML

[Q59] 分组内累计
来源：http://blog.fanxiaobao.xyz/Article/details/gxinyuots.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/gbtzsjqvl.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxhlmepbl.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wap.fanxiaobao.xyz/Article/details/gmzclxttd.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.fanxiaobao.xyz/Article/details/gbepsudsb.sHtML

[Q61] 移动平均
来源：http://mobile.fanxiaobao.xyz/Article/details/gxxchpgrg.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.fanxiaobao.xyz/Article/details/gsvmwvief.sHtML

[Q62] 分组占比
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbnjuuuig.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mobile.fanxiaobao.xyz/Article/details/gelamnkks.sHtML

[Q63] 开启事务
来源：http://m.share.fanxiaobao.xyz/Article/details/gfggfblwz.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://mobile.fanxiaobao.xyz/Article/details/grmnrigmv.sHtML

[Q64] 提交事务
来源：http://3g.fanxiaobao.xyz/Article/details/gbplkinam.sHtML

COMMIT;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghwaqktwb.sHtML

[Q65] 回滚事务
来源：http://read.share.fanxiaobao.xyz/Article/details/ghnafrvsg.sHtML

ROLLBACK;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glmtncyye.sHtML

[Q66] 行锁查询
来源：http://wap.fanxiaobao.xyz/Article/details/gczbjguvo.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wap.fanxiaobao.xyz/Article/details/gbifqvjik.sHtML

[Q67] 设置隔离级别
来源：http://m.share.fanxiaobao.xyz/Article/details/ghedpmczk.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.fanxiaobao.xyz/Article/details/gfhohaeku.sHtML

[Q68] 保存点
来源：http://m.share.fanxiaobao.xyz/Article/details/gvinbsgcp.sHtML

SAVEPOINT sp1;
来源：http://3g.fanxiaobao.xyz/Article/details/gcrjmuhqo.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzlbeenbv.sHtML

[Q69] 查看执行计划
来源：http://www.share.fanxiaobao.xyz/Article/details/gndwcydme.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.fanxiaobao.xyz/Article/details/gjpgpidak.sHtML

[Q70] 更新统计信息
来源：http://m.share.fanxiaobao.xyz/Article/details/gowauruqd.sHtML

ANALYZE TABLE users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gxbzbwltz.sHtML

[Q71] 查看建表语句
来源：http://www.share.fanxiaobao.xyz/Article/details/gukitddgk.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gphjylyvk.sHtML

[Q72] 查看索引
来源：http://baike.fanxiaobao.xyz/Article/details/ghvsonudm.sHtML

SHOW INDEX FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gutlwzkhw.sHtML

[Q73] 查看表状态
来源：http://mobile.fanxiaobao.xyz/Article/details/giemudjjv.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyuhdofmy.sHtML

[Q74] 强制使用索引
来源：http://wap.fanxiaobao.xyz/Article/details/gamezshmx.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://baike.fanxiaobao.xyz/Article/details/gyzeclpwd.sHtML

[Q75] 日期格式化
来源：http://blog.fanxiaobao.xyz/Article/details/giprvpcln.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/gwiruoibb.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.fanxiaobao.xyz/Article/details/gptdukadt.sHtML

[Q76] 按天统计
来源：http://www.share.fanxiaobao.xyz/Article/details/gzdmctfzc.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.fanxiaobao.xyz/Article/details/gztsqxrca.sHtML

[Q77] 时间加减
来源：http://blog.fanxiaobao.xyz/Article/details/gnhyubfxe.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.fanxiaobao.xyz/Article/details/ganvkqowo.sHtML

[Q78] 当前时间
来源：http://baike.fanxiaobao.xyz/Article/details/gzpermthz.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.fanxiaobao.xyz/Article/details/gdlaufptx.sHtML

[Q79] 字符串拼接
来源：http://www.share.fanxiaobao.xyz/Article/details/giqfkqcct.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.fanxiaobao.xyz/Article/details/gxburagnj.sHtML

[Q80] 字符串截取
来源：http://m.share.fanxiaobao.xyz/Article/details/gzqgsblmk.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gxxlemsvv.sHtML

[Q81] 字符串替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gqkepzcly.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/griyqpoxd.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.fanxiaobao.xyz/Article/details/gqxpoxiiw.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gybqpxwbc.sHtML

[Q83] 大小写转换
来源：http://baike.fanxiaobao.xyz/Article/details/gmhcmjfvr.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gxrbqlbbx.sHtML

[Q84] 去除首尾空格
来源：http://mobile.fanxiaobao.xyz/Article/details/gnehpdrqr.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvpfyrmfy.sHtML

[Q85] 数值取整
来源：http://www.blog.fanxiaobao.xyz/Article/details/gruccvvte.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.fanxiaobao.xyz/Article/details/gzfzvsajl.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.fanxiaobao.xyz/Article/details/gvaworhsf.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wap.fanxiaobao.xyz/Article/details/gyuuirrzr.sHtML

[Q87] JSON 字段做条件
来源：http://wap.fanxiaobao.xyz/Article/details/gzmtszsun.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.fanxiaobao.xyz/Article/details/gkbzkyxfm.sHtML

[Q88] 行转列（条件聚合）
来源：http://m.share.fanxiaobao.xyz/Article/details/gwguumjqc.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnerqxclj.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gigpvujxr.sHtML

[Q89] 判断表是否存在
来源：http://www.share.fanxiaobao.xyz/Article/details/gahcqjyvl.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjogwmebh.sHtML

[Q90] 生成序号列
来源：http://blog.fanxiaobao.xyz/Article/details/gwriynukk.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqgsdhcok.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gnwzuibbp.sHtML

R. Bash 专题
来源：http://blog.fanxiaobao.xyz/Article/details/ghldxotru.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/grabdzuud.sHtML

[R01] shebang 与严格模式
来源：http://wap.fanxiaobao.xyz/Article/details/glcrtrfin.sHtML

#!/usr/bin/env bash
来源：http://3g.fanxiaobao.xyz/Article/details/grabvhlth.sHtML

set -euo pipefail
来源：http://wap.fanxiaobao.xyz/Article/details/gtfkcmrnz.sHtML

[R02] 变量赋值与使用
来源：http://read.share.fanxiaobao.xyz/Article/details/gdsjvrhqv.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzupiygjh.sHtML

[R03] 只读变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/glopvqlfq.sHtML

readonly PI=3.14
来源：http://read.share.fanxiaobao.xyz/Article/details/gkjqseaex.sHtML

[R04] 位置参数
来源：http://www.share.fanxiaobao.xyz/Article/details/gblkgyglv.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.fanxiaobao.xyz/Article/details/gkaquyqvr.sHtML

[R05] 参数默认值
来源：http://3g.fanxiaobao.xyz/Article/details/gjocrcdtl.sHtML

name="${1:-default}"
来源：http://blog.fanxiaobao.xyz/Article/details/gyczjblda.sHtML

[R06] 判断命令是否存在
来源：http://baike.fanxiaobao.xyz/Article/details/ghrdvolom.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.fanxiaobao.xyz/Article/details/goeecdecj.sHtML

[R07] if 判断文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gjxzvqnll.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.fanxiaobao.xyz/Article/details/gnkuohqki.sHtML

[R08] 数值比较
来源：http://m.share.fanxiaobao.xyz/Article/details/golluossa.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdqwndtxy.sHtML

[R09] 字符串比较
来源：http://www.share.fanxiaobao.xyz/Article/details/gzbhqdnyc.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpqujajig.sHtML

[R10] 正则匹配
来源：http://mobile.fanxiaobao.xyz/Article/details/govkvpyrw.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.fanxiaobao.xyz/Article/details/glbaoyijf.sHtML

[R11] case 多分支
来源：http://www.blog.fanxiaobao.xyz/Article/details/grqjvcbfl.sHtML

case "$1" in
来源：http://wap.fanxiaobao.xyz/Article/details/guzycwnjy.sHtML

start) echo "启动" ;;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gydwbqsun.sHtML

stop)  echo "停止" ;;
来源：http://baike.fanxiaobao.xyz/Article/details/gejktxpcm.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.fanxiaobao.xyz/Article/details/gkiyfdcgn.sHtML

esac
来源：http://wap.fanxiaobao.xyz/Article/details/gkqmfidue.sHtML

[R12] for 遍历文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gdntteqck.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxwdmtowq.sHtML

[R13] for 计数循环
来源：http://read.share.fanxiaobao.xyz/Article/details/gvbcmguvp.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghlimyzvq.sHtML

[R14] C 风格 for
来源：http://wap.fanxiaobao.xyz/Article/details/gbhksrgel.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gaqqwwbbb.sHtML

[R15] while 逐行读文件
来源：http://wap.fanxiaobao.xyz/Article/details/gifalbqfp.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gknzsumjp.sHtML

[R16] until 等待条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbfwdhmhp.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsmifvlei.sHtML

[R17] 数组定义与取值
来源：http://wap.fanxiaobao.xyz/Article/details/gtxrwcfga.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.fanxiaobao.xyz/Article/details/gyaiklrhv.sHtML

[R18] 遍历数组
来源：http://mobile.fanxiaobao.xyz/Article/details/gnsqnptbu.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gvsjtbawq.sHtML

[R19] 数组长度
来源：http://3g.fanxiaobao.xyz/Article/details/gykdprabj.sHtML

echo "${#arr[@]}"
来源：http://3g.fanxiaobao.xyz/Article/details/gokwqxbon.sHtML

[R20] 关联数组（字典）
来源：http://mobile.fanxiaobao.xyz/Article/details/ggpvyhkgx.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.fanxiaobao.xyz/Article/details/gqtveepup.sHtML

[R21] 字符串长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxmtfpdej.sHtML

echo "${#s}"
来源：http://wap.fanxiaobao.xyz/Article/details/gchmzjkbl.sHtML

[R22] 截取子串
来源：http://m.share.fanxiaobao.xyz/Article/details/gitolksrs.sHtML

echo "${s:0:5}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geiounrgc.sHtML

[R23] 字符串替换
来源：http://blog.fanxiaobao.xyz/Article/details/gpqkeyndz.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gctrzayfa.sHtML

[R24] 大小写转换
来源：http://www.share.fanxiaobao.xyz/Article/details/gjzuugkqt.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.fanxiaobao.xyz/Article/details/gbarcngde.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.fanxiaobao.xyz/Article/details/gucfmlren.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.fanxiaobao.xyz/Article/details/gobfbldjt.sHtML

[R26] 命令替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxbwhilzf.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.fanxiaobao.xyz/Article/details/gkxyuhgzu.sHtML

[R27] 算术展开
来源：http://www.share.fanxiaobao.xyz/Article/details/gdmxaxgdu.sHtML

echo $((1 + 2 * 3))
来源：http://3g.fanxiaobao.xyz/Article/details/gqhnlwndt.sHtML

[R28] 浮点运算
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqyuynobr.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.fanxiaobao.xyz/Article/details/gwxjvyata.sHtML

[R29] 定义函数
来源：http://blog.fanxiaobao.xyz/Article/details/gzuuyhotu.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.fanxiaobao.xyz/Article/details/gcatlqtol.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmtcqrhme.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.fanxiaobao.xyz/Article/details/gywkvlmjx.sHtML

[R31] 局部变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gadhjgfhm.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gmuczabro.sHtML

[R32] 参数个数校验
来源：http://www.share.fanxiaobao.xyz/Article/details/gqkibyawf.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.fanxiaobao.xyz/Article/details/gsjawlcdm.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.fanxiaobao.xyz/Article/details/ghoqmkwgp.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyvjvccol.sHtML

[R34] 退出时清理
来源：http://www.share.fanxiaobao.xyz/Article/details/glcijapnh.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gevopfzkf.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghuzzvxwm.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.fanxiaobao.xyz/Article/details/gnlfhcoak.sHtML

[R36] 并发执行多个任务
来源：http://mobile.fanxiaobao.xyz/Article/details/ghihpousv.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvdxkfnft.sHtML

[R37] 把输出赋给变量
来源：http://m.share.fanxiaobao.xyz/Article/details/guabgteok.sHtML

files=$(ls -1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gzoayipet.sHtML

[R38] 管道串联
来源：http://read.share.fanxiaobao.xyz/Article/details/gkvocmsjv.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.fanxiaobao.xyz/Article/details/gusrawsnd.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpjycnmsk.sHtML

cmd > out.log 2>&1
来源：http://baike.fanxiaobao.xyz/Article/details/gqhesjreq.sHtML

[R40] 追加写日志
来源：http://baike.fanxiaobao.xyz/Article/details/gikyvwckd.sHtML

echo "log" >> out.log
来源：http://wap.fanxiaobao.xyz/Article/details/gahuqsihz.sHtML

[R41] 丢弃输出
来源：http://m.share.fanxiaobao.xyz/Article/details/grhxanzjo.sHtML

cmd >/dev/null 2>&1
来源：http://blog.fanxiaobao.xyz/Article/details/gcijzfdbg.sHtML

[R42] 输入重定向
来源：http://3g.fanxiaobao.xyz/Article/details/gakhcztap.sHtML

wc -l < a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gcscrzbei.sHtML

[R43] 按名字查找文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gwlbumuhd.sHtML

find . -name "*.log" -type f
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzwzfrape.sHtML

[R44] 按修改时间查找
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdyftbtqf.sHtML

find . -mtime -7 -type f
来源：http://3g.fanxiaobao.xyz/Article/details/gpbzsiruz.sHtML

[R45] 批量删除
来源：http://www.blog.fanxiaobao.xyz/Article/details/gionoaxgm.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.fanxiaobao.xyz/Article/details/gahlnzxyd.sHtML

[R46] 递归替换文件内容
来源：http://wap.fanxiaobao.xyz/Article/details/gyuuarehq.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.fanxiaobao.xyz/Article/details/grujifemp.sHtML

[R47] sed 单行替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gakzzxlur.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/giguepbiq.sHtML

[R48] awk 取指定列
来源：http://3g.fanxiaobao.xyz/Article/details/gnswrinfn.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gaxziglyz.sHtML

[R49] awk 带条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmmkczvvn.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.fanxiaobao.xyz/Article/details/ginvxrjyk.sHtML

[R50] awk 求和
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbamxxfjp.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gglguoswb.sHtML

[R51] 排序去重取前几
来源：http://mobile.fanxiaobao.xyz/Article/details/giennpcug.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.fanxiaobao.xyz/Article/details/gwymkwzxy.sHtML

[R52] 统计行数
来源：http://blog.fanxiaobao.xyz/Article/details/gpvxzxwdr.sHtML

wc -l a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gvovrxmva.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.fanxiaobao.xyz/Article/details/gisjeuojy.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjigylvlq.sHtML

[R54] 比较两个文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gorrjwnob.sHtML

diff a.txt b.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/giyjesyyh.sHtML

[R55] 压缩与解压
来源：http://www.share.fanxiaobao.xyz/Article/details/gzafcrkts.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.fanxiaobao.xyz/Article/details/gymawofpx.sHtML

[R56] 远程拷贝
来源：http://baike.fanxiaobao.xyz/Article/details/gbnrcyjuy.sHtML

scp file user@host:/path/
来源：http://baike.fanxiaobao.xyz/Article/details/gplzjcaal.sHtML

[R57] 远程执行命令
来源：http://baike.fanxiaobao.xyz/Article/details/gmazwegfw.sHtML

ssh user@host 'uptime'
来源：http://wap.fanxiaobao.xyz/Article/details/gvvlvsixx.sHtML

[R58] 下载文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gydubhovm.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.fanxiaobao.xyz/Article/details/gepumfuhu.sHtML

[R59] 发 POST JSON
来源：http://m.share.fanxiaobao.xyz/Article/details/glursgnou.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.fanxiaobao.xyz/Article/details/gfsofueai.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.fanxiaobao.xyz/Article/details/gojrnjlsx.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.fanxiaobao.xyz/Article/details/glkxlajbx.sHtML

[R61] 磁盘占用
来源：http://wap.fanxiaobao.xyz/Article/details/ghrgnyiin.sHtML

df -h;  du -sh *
来源：http://mobile.fanxiaobao.xyz/Article/details/gaovuewfq.sHtML

[R62] 找最占空间的文件
来源：http://3g.fanxiaobao.xyz/Article/details/gxizoozfj.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqsmjazql.sHtML

[R63] 内存与进程
来源：http://mobile.fanxiaobao.xyz/Article/details/gxspxwgbu.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.fanxiaobao.xyz/Article/details/gvbirzgbg.sHtML

[R64] 结束进程
来源：http://3g.fanxiaobao.xyz/Article/details/glsyrkyfn.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.fanxiaobao.xyz/Article/details/gczbhchhw.sHtML

[R65] 查看端口占用
来源：http://www.share.fanxiaobao.xyz/Article/details/gfwxqxezw.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.fanxiaobao.xyz/Article/details/glycrihky.sHtML

[R66] 定时任务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjuqrwkwl.sHtML

crontab -e;  crontab -l
来源：http://3g.fanxiaobao.xyz/Article/details/gdacggmsx.sHtML

[R67] 生成随机十六进制串
来源：http://baike.fanxiaobao.xyz/Article/details/gprsufeta.sHtML

openssl rand -hex 16
来源：http://wap.fanxiaobao.xyz/Article/details/ghquskzpn.sHtML

[R68] 计算文件校验值
来源：http://read.share.fanxiaobao.xyz/Article/details/gxejmsikw.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gfwlzzgun.sHtML

[R69] 生成随机密码
来源：http://blog.fanxiaobao.xyz/Article/details/gjrtjdvsg.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.fanxiaobao.xyz/Article/details/gxaevhvzn.sHtML

[R70] 时间戳与互转
来源：http://baike.fanxiaobao.xyz/Article/details/gtfiyznah.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmsjggzvt.sHtML

[R71] 日期格式化
来源：http://3g.fanxiaobao.xyz/Article/details/gzagrszvo.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaecfaalk.sHtML

[R72] 等待端口就绪
来源：http://wap.fanxiaobao.xyz/Article/details/gpnmjcoab.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.fanxiaobao.xyz/Article/details/ghtjuxiog.sHtML

[R73] 分割大日志
来源：http://mobile.fanxiaobao.xyz/Article/details/gravyarww.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaonamkth.sHtML

[R74] 批量重命名
来源：http://3g.fanxiaobao.xyz/Article/details/gytjpwmlk.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gsqgamlxl.sHtML

[R75] 导出环境变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmobzmzvq.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.fanxiaobao.xyz/Article/details/gavwlcwiy.sHtML

[R76] 使用临时文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gntytlznn.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbmtbyjjd.sHtML

[R77] 读取用户输入
来源：http://mobile.fanxiaobao.xyz/Article/details/gzgrcyszj.sHtML

read -rp "请输入: " ans
来源：http://wap.fanxiaobao.xyz/Article/details/gklnmninr.sHtML

[R78] 交互式菜单
来源：http://m.share.fanxiaobao.xyz/Article/details/gtdjiydjj.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gdjigadif.sHtML

[R79] 解析命令行选项
来源：http://baike.fanxiaobao.xyz/Article/details/gyctdmymj.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.fanxiaobao.xyz/Article/details/gnjlhudtw.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.fanxiaobao.xyz/Article/details/gswfxxqtq.sHtML

time ./run.sh
来源：http://mobile.fanxiaobao.xyz/Article/details/gtsprutxn.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gvmkpnhmy.sHtML

S. C / C++ 专题
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjfirerqo.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/giiwoubyb.sHtML

[S01] C：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/glaqyznif.sHtML

#include <stdio.h>
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyzmpjeyl.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.fanxiaobao.xyz/Article/details/gibpdarec.sHtML

[S02] C：变量与格式化输出
来源：http://3g.fanxiaobao.xyz/Article/details/gqhxoidpf.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.fanxiaobao.xyz/Article/details/glavvsrvk.sHtML

[S03] C：读入整数
来源：http://mobile.fanxiaobao.xyz/Article/details/gfzpgpztr.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gedcoscgd.sHtML

[S04] C：字符串复制
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtkdwooga.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.fanxiaobao.xyz/Article/details/gbonbzgcr.sHtML

[S05] C：字符串长度
来源：http://wap.fanxiaobao.xyz/Article/details/gaeyjrcii.sHtML

strlen(s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gefoqbcmu.sHtML

[S06] C：字符串比较
来源：http://wap.fanxiaobao.xyz/Article/details/gipyecgpo.sHtML

strcmp(a, b) == 0
来源：http://www.share.fanxiaobao.xyz/Article/details/gnboctwmk.sHtML

[S07] C：数组遍历求和
来源：http://3g.fanxiaobao.xyz/Article/details/gguclupqk.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.fanxiaobao.xyz/Article/details/gzflrykrs.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.fanxiaobao.xyz/Article/details/guakapatn.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gawtpwibf.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.fanxiaobao.xyz/Article/details/gbpadffbq.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.fanxiaobao.xyz/Article/details/gdaluaqch.sHtML

[S10] C：指针与解引用
来源：http://wap.fanxiaobao.xyz/Article/details/gxzxuilxk.sHtML

int *p = &a;  *p = 5;
来源：http://3g.fanxiaobao.xyz/Article/details/gnitsxcxe.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjiqfvlxe.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.fanxiaobao.xyz/Article/details/gqlvoggrx.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.fanxiaobao.xyz/Article/details/gagwanrzp.sHtML

fclose(f);
来源：http://read.share.fanxiaobao.xyz/Article/details/gydnsqqek.sHtML

[S12] C：写文件
来源：http://3g.fanxiaobao.xyz/Article/details/glhxibkjk.sHtML


<!-- 参考信息 -->