代发 wailian999

[Q38] 全外连接（PostgreSQL）
来源：http://www.share.zdbjq.cn/Article/details/goonvcjcc.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.share.fehbvm.com/Article/details/gcdknkrqj.sHtML

[Q39] 自连接（查上下级）
来源：http://www.blog.hesvh.cn/Article/details/gmthcvuon.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.m.share.fehbvm.com/Article/details/goqauoesp.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.fehbvm.com/Article/details/gqunklmke.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://baike.hesvh.cn/Article/details/gwepcbhtv.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.share.hesvh.cn/Article/details/gbmzoszox.sHtML

[Q41] 多表连接
来源：http://www.m.share.hesvh.cn/Article/details/gtozhxnrl.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.share.zdbjq.cn/Article/details/gyxfrekfa.sHtML

JOIN users u ON u.id = o.user_id
来源：http://read.share.hesvh.cn/Article/details/gykppuebb.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://wap.hesvh.cn/Article/details/gncfigrrk.sHtML

[Q42] 连接条件附加过滤
来源：http://baike.zdbjq.cn/Article/details/gwjgjnkxa.sHtML

SELECT u.name, o.amount FROM users u
来源：http://read.share.hesvh.cn/Article/details/gxnfiwcgw.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://m.share.zdbjq.cn/Article/details/gjqtyqexu.sHtML

[Q43] 标量子查询
来源：http://mobile.hesvh.cn/Article/details/gudoreeot.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.hesvh.cn/Article/details/gmbjndgzx.sHtML

[Q44] IN 子查询
来源：http://mobile.fehbvm.com/Article/details/grqmqtfqe.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.zdbjq.cn/Article/details/gyuqqqsfk.sHtML

[Q45] EXISTS 判断存在
来源：http://m.share.zdbjq.cn/Article/details/grbyztoil.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.hesvh.cn/Article/details/gqssqrkza.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.share.zdbjq.cn/Article/details/gfdcbngyj.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.hesvh.cn/Article/details/ghnixtvge.sHtML

[Q47] 与平均值比较
来源：http://www.m.share.zdbjq.cn/Article/details/ghqywftik.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.share.zdbjq.cn/Article/details/gelfrqoms.sHtML

[Q48] CTE 公用表表达式
来源：http://baike.hesvh.cn/Article/details/gleuuwfcr.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.share.zdbjq.cn/Article/details/gzdyclhlc.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.hesvh.cn/Article/details/gefmigllo.sHtML

[Q49] 更新单行
来源：http://m.share.hesvh.cn/Article/details/gpoifluii.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.fehbvm.com/Article/details/gplprihws.sHtML

[Q50] 批量更新
来源：http://m.share.zdbjq.cn/Article/details/gusmeffqy.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.zdbjq.cn/Article/details/gdwwwtwqx.sHtML

[Q51] 用子查询更新
来源：http://3g.zdbjq.cn/Article/details/gnrefucxa.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gsobjdohz.sHtML

[Q52] 删除指定行
来源：http://mobile.zdbjq.cn/Article/details/gsdtkbcpr.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.fehbvm.com/Article/details/gdfmoeoxv.sHtML

[Q53] 按条件删除
来源：http://3g.fehbvm.com/Article/details/gejivawxh.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://m.share.zdbjq.cn/Article/details/ghxdhyzsx.sHtML

[Q54] 清空表
来源：http://www.blog.fehbvm.com/Article/details/goveescbv.sHtML

TRUNCATE TABLE logs;
来源：http://wap.zdbjq.cn/Article/details/gxlfbyklx.sHtML

[Q55] 排名（并列占位）
来源：http://www.share.hesvh.cn/Article/details/gbhqxrrti.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mobile.hesvh.cn/Article/details/gdysivohp.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.m.share.hesvh.cn/Article/details/glzsvejae.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.fehbvm.com/Article/details/gqxdgvlze.sHtML

[Q57] 行号
来源：http://mobile.hesvh.cn/Article/details/gfgjjqqhs.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gaufabhjk.sHtML

[Q58] 累计求和
来源：http://baike.fehbvm.com/Article/details/ghnpwqeyg.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/ggaatlwxn.sHtML

[Q59] 分组内累计
来源：http://m.share.hesvh.cn/Article/details/gecrrswvy.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gqnldofxe.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.share.hesvh.cn/Article/details/gniupnplo.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.m.share.hesvh.cn/Article/details/gvqcnzhul.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/gxplxarqq.sHtML

[Q61] 移动平均
来源：http://baike.zdbjq.cn/Article/details/glhnvwyqp.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.zdbjq.cn/Article/details/gpczuvsxz.sHtML

[Q62] 分组占比
来源：http://blog.zdbjq.cn/Article/details/gbxqkzjcr.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.hesvh.cn/Article/details/gtdgvldng.sHtML

[Q63] 开启事务
来源：http://m.share.fehbvm.com/Article/details/gbquhyczt.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.zdbjq.cn/Article/details/gubkfgcnm.sHtML

[Q64] 提交事务
来源：http://wap.zdbjq.cn/Article/details/gkebbhppo.sHtML

COMMIT;
来源：http://baike.zdbjq.cn/Article/details/gnbjqblhp.sHtML

[Q65] 回滚事务
来源：http://baike.hesvh.cn/Article/details/gwixtxzne.sHtML

ROLLBACK;
来源：http://www.blog.hesvh.cn/Article/details/gvcxbwmzz.sHtML

[Q66] 行锁查询
来源：http://baike.hesvh.cn/Article/details/gtumietkh.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://baike.hesvh.cn/Article/details/ginyzyude.sHtML

[Q67] 设置隔离级别
来源：http://www.m.share.zdbjq.cn/Article/details/gsyvglmte.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.fehbvm.com/Article/details/gxhgeiomy.sHtML

[Q68] 保存点
来源：http://3g.zdbjq.cn/Article/details/gddkrplog.sHtML

SAVEPOINT sp1;
来源：http://mobile.hesvh.cn/Article/details/gzmggeztp.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.hesvh.cn/Article/details/gdmwzarik.sHtML

[Q69] 查看执行计划
来源：http://www.blog.hesvh.cn/Article/details/gghhcuhvd.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.fehbvm.com/Article/details/gnrwhihku.sHtML

[Q70] 更新统计信息
来源：http://baike.hesvh.cn/Article/details/gmwrspmrj.sHtML

ANALYZE TABLE users;
来源：http://www.share.fehbvm.com/Article/details/gtptdldes.sHtML

[Q71] 查看建表语句
来源：http://3g.zdbjq.cn/Article/details/gisahfmcg.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.zdbjq.cn/Article/details/gjiblkepj.sHtML

[Q72] 查看索引
来源：http://wap.zdbjq.cn/Article/details/gcdbgtixo.sHtML

SHOW INDEX FROM users;
来源：http://www.share.fehbvm.com/Article/details/gmgqsvzxx.sHtML

[Q73] 查看表状态
来源：http://read.share.hesvh.cn/Article/details/gjroooyfs.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.hesvh.cn/Article/details/gbziqjybh.sHtML

[Q74] 强制使用索引
来源：http://m.share.fehbvm.com/Article/details/gmwuzopgm.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.hesvh.cn/Article/details/gibmdyctw.sHtML

[Q75] 日期格式化
来源：http://www.blog.zdbjq.cn/Article/details/gebdcxyjn.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/ggexovxpo.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.blog.fehbvm.com/Article/details/goqsthpkg.sHtML

[Q76] 按天统计
来源：http://mobile.fehbvm.com/Article/details/gpakiomfi.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.zdbjq.cn/Article/details/gngazjboy.sHtML

[Q77] 时间加减
来源：http://m.share.fehbvm.com/Article/details/gujrqzhgi.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.hesvh.cn/Article/details/gmfjgecab.sHtML

[Q78] 当前时间
来源：http://blog.zdbjq.cn/Article/details/guazpznzb.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.fehbvm.com/Article/details/gjwsbyerq.sHtML

[Q79] 字符串拼接
来源：http://www.blog.zdbjq.cn/Article/details/gvvruwdab.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.hesvh.cn/Article/details/gkvgppiiu.sHtML

[Q80] 字符串截取
来源：http://m.share.hesvh.cn/Article/details/gbmqhxtkq.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.fehbvm.com/Article/details/gvmbhvyos.sHtML

[Q81] 字符串替换
来源：http://mobile.fehbvm.com/Article/details/gsyeffkao.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.zdbjq.cn/Article/details/ggieqtpcj.sHtML

[Q82] 字符长度与字节长度
来源：http://m.share.hesvh.cn/Article/details/ggqilgjni.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.hesvh.cn/Article/details/gzitregzi.sHtML

[Q83] 大小写转换
来源：http://wap.fehbvm.com/Article/details/gftpywdno.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.zdbjq.cn/Article/details/gpdedoboy.sHtML

[Q84] 去除首尾空格
来源：http://www.blog.zdbjq.cn/Article/details/gmfftfzgz.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.hesvh.cn/Article/details/gjyifuprl.sHtML

[Q85] 数值取整
来源：http://www.blog.hesvh.cn/Article/details/ghspzehzw.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.hesvh.cn/Article/details/gxfqarqtk.sHtML

[Q86] 读取 JSON 字段
来源：http://blog.fehbvm.com/Article/details/gvnnkhgrz.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.fehbvm.com/Article/details/gzofadwxx.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.hesvh.cn/Article/details/gltagpyur.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.fehbvm.com/Article/details/gfolvhmvc.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.share.hesvh.cn/Article/details/gwaizjlgx.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.hesvh.cn/Article/details/gjagrnpkx.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://m.share.zdbjq.cn/Article/details/giteqbxzo.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.hesvh.cn/Article/details/gwpphhomr.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.zdbjq.cn/Article/details/gniatzcvf.sHtML

[Q90] 生成序号列
来源：http://blog.hesvh.cn/Article/details/gqbyrtiqt.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.hesvh.cn/Article/details/gwnzokcna.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gupsvmkac.sHtML

R. Bash 专题
来源：http://3g.fehbvm.com/Article/details/ghwjpfeer.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gxjqkhkhb.sHtML

[R01] shebang 与严格模式
来源：http://blog.zdbjq.cn/Article/details/gddhanzmg.sHtML

#!/usr/bin/env bash
来源：http://read.share.hesvh.cn/Article/details/gqvvtqkev.sHtML

set -euo pipefail
来源：http://www.m.share.hesvh.cn/Article/details/gvpjtkvcv.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.fehbvm.com/Article/details/gqjzpeaqj.sHtML

name="Tom"; echo "$name"
来源：http://baike.hesvh.cn/Article/details/geocikzsc.sHtML

[R03] 只读变量
来源：http://wap.zdbjq.cn/Article/details/gdgtpfkkn.sHtML

readonly PI=3.14
来源：http://www.m.share.fehbvm.com/Article/details/gyhlxhpvt.sHtML

[R04] 位置参数
来源：http://www.m.share.hesvh.cn/Article/details/gwqxwpiqz.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.hesvh.cn/Article/details/gusnwrfjp.sHtML

[R05] 参数默认值
来源：http://3g.zdbjq.cn/Article/details/geoivcjea.sHtML

name="${1:-default}"
来源：http://mobile.zdbjq.cn/Article/details/gqtablkeh.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.fehbvm.com/Article/details/glkcsjxnp.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.hesvh.cn/Article/details/gpcypbezk.sHtML

[R07] if 判断文件
来源：http://blog.fehbvm.com/Article/details/gbsyngkwx.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.fehbvm.com/Article/details/gvghxpmvk.sHtML

[R08] 数值比较
来源：http://baike.hesvh.cn/Article/details/giiguzmzt.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.fehbvm.com/Article/details/gpsqipkwm.sHtML

[R09] 字符串比较
来源：http://blog.hesvh.cn/Article/details/ggwzxrdsn.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.hesvh.cn/Article/details/gdplgdexc.sHtML

[R10] 正则匹配
来源：http://www.m.share.zdbjq.cn/Article/details/gpwstsdlm.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.fehbvm.com/Article/details/gtzpxpdvo.sHtML

[R11] case 多分支
来源：http://www.blog.zdbjq.cn/Article/details/gdjwlyarr.sHtML

case "$1" in
来源：http://www.m.share.zdbjq.cn/Article/details/glfmdojuy.sHtML

start) echo "启动" ;;
来源：http://baike.zdbjq.cn/Article/details/gaambnuyn.sHtML

stop)  echo "停止" ;;
来源：http://blog.zdbjq.cn/Article/details/gogovpamy.sHtML

*)     echo "未知命令" ;;
来源：http://wap.fehbvm.com/Article/details/gfuqufgbr.sHtML

esac
来源：http://wap.zdbjq.cn/Article/details/gojglcaph.sHtML

[R12] for 遍历文件
来源：http://m.share.hesvh.cn/Article/details/gztmsbgdc.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.zdbjq.cn/Article/details/gzdjtsfwm.sHtML

[R13] for 计数循环
来源：http://mobile.fehbvm.com/Article/details/gvrgqzknp.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.hesvh.cn/Article/details/ggzmbehjm.sHtML

[R14] C 风格 for
来源：http://3g.zdbjq.cn/Article/details/ggleqdyap.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.hesvh.cn/Article/details/gdsscvkax.sHtML

[R15] while 逐行读文件
来源：http://read.share.zdbjq.cn/Article/details/gwbifeqly.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.fehbvm.com/Article/details/gfntoxvmc.sHtML

[R16] until 等待条件
来源：http://wap.zdbjq.cn/Article/details/gajjvxlmf.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.fehbvm.com/Article/details/ghhweawhf.sHtML

[R17] 数组定义与取值
来源：http://wap.zdbjq.cn/Article/details/gykqwuiae.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.zdbjq.cn/Article/details/gzbcmjfxh.sHtML

[R18] 遍历数组
来源：http://3g.zdbjq.cn/Article/details/gyaidrmcw.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.zdbjq.cn/Article/details/gfhaviolr.sHtML

[R19] 数组长度
来源：http://baike.zdbjq.cn/Article/details/gsewafrgu.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.hesvh.cn/Article/details/guwaigcns.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.hesvh.cn/Article/details/ggpicblkp.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.fehbvm.com/Article/details/gbpevejmf.sHtML

[R21] 字符串长度
来源：http://www.m.share.fehbvm.com/Article/details/gxgwkybrw.sHtML

echo "${#s}"
来源：http://m.share.fehbvm.com/Article/details/gbnrrwjal.sHtML

[R22] 截取子串
来源：http://read.share.fehbvm.com/Article/details/gogvvcgyq.sHtML

echo "${s:0:5}"
来源：http://www.m.share.zdbjq.cn/Article/details/gkivjdinf.sHtML

[R23] 字符串替换
来源：http://baike.hesvh.cn/Article/details/gjqjnxaqo.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.fehbvm.com/Article/details/gydjjglbk.sHtML

[R24] 大小写转换
来源：http://www.share.zdbjq.cn/Article/details/gakuvdguv.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.fehbvm.com/Article/details/ggxogzucs.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.fehbvm.com/Article/details/gawfkksei.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.zdbjq.cn/Article/details/gknypoomu.sHtML

[R26] 命令替换
来源：http://m.share.hesvh.cn/Article/details/gicswqelg.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.fehbvm.com/Article/details/gxkghbxjr.sHtML

[R27] 算术展开
来源：http://www.share.zdbjq.cn/Article/details/gjlxfvjvo.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.fehbvm.com/Article/details/gjvfslogz.sHtML

[R28] 浮点运算
来源：http://m.share.zdbjq.cn/Article/details/ghzsyfrbn.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.hesvh.cn/Article/details/gcstrtywj.sHtML

[R29] 定义函数
来源：http://read.share.fehbvm.com/Article/details/gzztcdeka.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.hesvh.cn/Article/details/gklfpzkou.sHtML

[R30] 函数返回状态码
来源：http://www.share.zdbjq.cn/Article/details/glbfrypgh.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.hesvh.cn/Article/details/ghlduzwzv.sHtML

[R31] 局部变量
来源：http://wap.hesvh.cn/Article/details/gxfimjohr.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.fehbvm.com/Article/details/ggehmrmoi.sHtML

[R32] 参数个数校验
来源：http://www.m.share.hesvh.cn/Article/details/gxwpnoxzv.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.hesvh.cn/Article/details/golblkova.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.fehbvm.com/Article/details/gqptqxzrf.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.fehbvm.com/Article/details/ggxjfaizo.sHtML

[R34] 退出时清理
来源：http://www.share.fehbvm.com/Article/details/gscemrtkm.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.share.hesvh.cn/Article/details/gtpiziwpe.sHtML

[R35] 后台执行并等待
来源：http://www.blog.fehbvm.com/Article/details/gyhvcsavk.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.zdbjq.cn/Article/details/gbmviohdx.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.fehbvm.com/Article/details/glrtagvry.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.zdbjq.cn/Article/details/gbjdapzwm.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.zdbjq.cn/Article/details/gndjdfqid.sHtML

files=$(ls -1)
来源：http://3g.fehbvm.com/Article/details/gsokauqet.sHtML

[R38] 管道串联
来源：http://www.share.fehbvm.com/Article/details/gkfzzevza.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.hesvh.cn/Article/details/gruwkrzyq.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.zdbjq.cn/Article/details/gxtdmfjdx.sHtML

cmd > out.log 2>&1
来源：http://baike.zdbjq.cn/Article/details/gmyniinkk.sHtML

[R40] 追加写日志
来源：http://www.m.share.fehbvm.com/Article/details/gxmjjvvbk.sHtML

echo "log" >> out.log
来源：http://3g.zdbjq.cn/Article/details/gcorgbkri.sHtML

[R41] 丢弃输出
来源：http://mobile.zdbjq.cn/Article/details/gavuvjkqt.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.hesvh.cn/Article/details/ggxvzjise.sHtML

[R42] 输入重定向
来源：http://blog.fehbvm.com/Article/details/guldulice.sHtML

wc -l < a.txt
来源：http://m.share.hesvh.cn/Article/details/grcjcaeis.sHtML

[R43] 按名字查找文件
来源：http://mobile.fehbvm.com/Article/details/gzdfoenjb.sHtML

find . -name "*.log" -type f
来源：http://m.share.fehbvm.com/Article/details/gmveeeivv.sHtML

[R44] 按修改时间查找
来源：http://baike.zdbjq.cn/Article/details/gnfijgmav.sHtML

find . -mtime -7 -type f
来源：http://mobile.zdbjq.cn/Article/details/gxgbuvioc.sHtML

[R45] 批量删除
来源：http://3g.fehbvm.com/Article/details/gsuxgwvxo.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.zdbjq.cn/Article/details/gundvxpdz.sHtML

[R46] 递归替换文件内容
来源：http://mobile.zdbjq.cn/Article/details/guwizhqbd.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.fehbvm.com/Article/details/gnbkncwmt.sHtML

[R47] sed 单行替换
来源：http://blog.hesvh.cn/Article/details/gkjzltasm.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.zdbjq.cn/Article/details/gbcvzsmwl.sHtML

[R48] awk 取指定列
来源：http://www.blog.fehbvm.com/Article/details/gqmbqdfaq.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.fehbvm.com/Article/details/gcayoybgj.sHtML

[R49] awk 带条件
来源：http://m.share.fehbvm.com/Article/details/gsczcdebl.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.zdbjq.cn/Article/details/gfbevuush.sHtML

[R50] awk 求和
来源：http://3g.hesvh.cn/Article/details/gawfuokad.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.zdbjq.cn/Article/details/grhmyvnbx.sHtML

[R51] 排序去重取前几
来源：http://m.share.zdbjq.cn/Article/details/glxirbppj.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.hesvh.cn/Article/details/gwxusqilr.sHtML

[R52] 统计行数
来源：http://blog.zdbjq.cn/Article/details/gfzwhjzer.sHtML

wc -l a.txt
来源：http://www.blog.fehbvm.com/Article/details/gcvtevymk.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.hesvh.cn/Article/details/guryowtpu.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.hesvh.cn/Article/details/gbmzmiqqw.sHtML

[R54] 比较两个文件
来源：http://wap.hesvh.cn/Article/details/grcfgqbdm.sHtML

diff a.txt b.txt
来源：http://blog.hesvh.cn/Article/details/gntbqgenk.sHtML

[R55] 压缩与解压
来源：http://blog.zdbjq.cn/Article/details/gmbgpmobj.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.zdbjq.cn/Article/details/ggrwpgbpr.sHtML

[R56] 远程拷贝
来源：http://3g.fehbvm.com/Article/details/ggojvtsrj.sHtML

scp file user@host:/path/
来源：http://mobile.fehbvm.com/Article/details/giumpjwft.sHtML

[R57] 远程执行命令
来源：http://www.blog.zdbjq.cn/Article/details/gymtkwuth.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.fehbvm.com/Article/details/gksjaipip.sHtML

[R58] 下载文件
来源：http://mobile.hesvh.cn/Article/details/googdvswi.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.fehbvm.com/Article/details/gdhchztcf.sHtML

[R59] 发 POST JSON
来源：http://m.share.fehbvm.com/Article/details/gxbnedhjd.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.fehbvm.com/Article/details/gabuvkxps.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.zdbjq.cn/Article/details/gnstzzilj.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.fehbvm.com/Article/details/gfvkclafz.sHtML

[R61] 磁盘占用
来源：http://www.share.hesvh.cn/Article/details/gooduwjxc.sHtML

df -h;  du -sh *
来源：http://wap.fehbvm.com/Article/details/grqepudrc.sHtML

[R62] 找最占空间的文件
来源：http://read.share.zdbjq.cn/Article/details/gfysjbzjm.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.hesvh.cn/Article/details/gzksmdhcj.sHtML

[R63] 内存与进程
来源：http://baike.zdbjq.cn/Article/details/gvrhyaivg.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.fehbvm.com/Article/details/gohyrkswn.sHtML

[R64] 结束进程
来源：http://3g.zdbjq.cn/Article/details/gwosfiqsn.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.fehbvm.com/Article/details/gfyntvqgg.sHtML

[R65] 查看端口占用
来源：http://blog.hesvh.cn/Article/details/gejugvfyy.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.fehbvm.com/Article/details/gqwzsfaoa.sHtML

[R66] 定时任务
来源：http://www.blog.zdbjq.cn/Article/details/gtzpobrdc.sHtML

crontab -e;  crontab -l
来源：http://wap.hesvh.cn/Article/details/gnxmaghlk.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.fehbvm.com/Article/details/gkivrkhcu.sHtML

openssl rand -hex 16
来源：http://blog.hesvh.cn/Article/details/gqhlbhses.sHtML

[R68] 计算文件校验值
来源：http://mobile.hesvh.cn/Article/details/gbhfvhxiu.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/glxpeasxe.sHtML

[R69] 生成随机密码
来源：http://blog.hesvh.cn/Article/details/gsgzeakuc.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.hesvh.cn/Article/details/gxjhiatbk.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.fehbvm.com/Article/details/goffcrssx.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.fehbvm.com/Article/details/gptcvvbxp.sHtML

[R71] 日期格式化
来源：http://wap.hesvh.cn/Article/details/gwplyrfib.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.fehbvm.com/Article/details/gffnjvukp.sHtML

[R72] 等待端口就绪
来源：http://mobile.hesvh.cn/Article/details/gzmguazpm.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.fehbvm.com/Article/details/gctzhgeit.sHtML

[R73] 分割大日志
来源：http://www.share.hesvh.cn/Article/details/gffrytawj.sHtML

split -l 1000 big.log part_
来源：http://baike.zdbjq.cn/Article/details/gdpxlwfuz.sHtML

[R74] 批量重命名
来源：http://3g.fehbvm.com/Article/details/gjpryxmpf.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.hesvh.cn/Article/details/gbukwmjbi.sHtML

[R75] 导出环境变量
来源：http://www.share.hesvh.cn/Article/details/gkiltsrvb.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.fehbvm.com/Article/details/gixjgvelp.sHtML

[R76] 使用临时文件
来源：http://www.share.zdbjq.cn/Article/details/guwqwbiyb.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.hesvh.cn/Article/details/gduwgzrrq.sHtML

[R77] 读取用户输入
来源：http://3g.fehbvm.com/Article/details/gqufdhebh.sHtML

read -rp "请输入: " ans
来源：http://mobile.fehbvm.com/Article/details/gmbutcghe.sHtML

[R78] 交互式菜单
来源：http://m.share.fehbvm.com/Article/details/glasrfmlf.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.zdbjq.cn/Article/details/gqetgtntt.sHtML

[R79] 解析命令行选项
来源：http://baike.zdbjq.cn/Article/details/gdzcmsizu.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.hesvh.cn/Article/details/gjqwpnqot.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.fehbvm.com/Article/details/gbfpfldzb.sHtML

time ./run.sh
来源：http://mobile.zdbjq.cn/Article/details/gabadmmpd.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/ghoqtqfvt.sHtML

S. C / C++ 专题
来源：http://www.share.fehbvm.com/Article/details/gjnyhoals.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gphfdfwaf.sHtML

[S01] C：Hello World
来源：http://wap.fehbvm.com/Article/details/gyitqegxs.sHtML

#include <stdio.h>
来源：http://wap.zdbjq.cn/Article/details/gipgxjplm.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.zdbjq.cn/Article/details/gcqqwjaro.sHtML

[S02] C：变量与格式化输出
来源：http://wap.fehbvm.com/Article/details/ggbvxtnuo.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.fehbvm.com/Article/details/gkjtjxxav.sHtML

[S03] C：读入整数
来源：http://www.m.share.fehbvm.com/Article/details/ggtofbvyj.sHtML

int x; scanf("%d", &x);
来源：http://blog.hesvh.cn/Article/details/gusztpleh.sHtML

[S04] C：字符串复制
来源：http://www.share.zdbjq.cn/Article/details/goofkeyip.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.zdbjq.cn/Article/details/gvdwdlrji.sHtML

[S05] C：字符串长度
来源：http://mobile.zdbjq.cn/Article/details/gslkhpdsk.sHtML

strlen(s)
来源：http://blog.fehbvm.com/Article/details/goachirhj.sHtML

[S06] C：字符串比较
来源：http://www.share.hesvh.cn/Article/details/gfmszftvx.sHtML

strcmp(a, b) == 0
来源：http://mobile.hesvh.cn/Article/details/gdykejbuj.sHtML

[S07] C：数组遍历求和
来源：http://3g.hesvh.cn/Article/details/gymdawfji.sHtML


<!-- 参考信息 -->