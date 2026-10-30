代发 wailian999

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mobile.zdbjq.cn/Article/details/giiyibldg.sHtML

) t WHERE rn = 1;
来源：http://www.share.zdbjq.cn/Article/details/ggmoggaqi.sHtML

[Q35] 内连接
来源：http://mobile.fehbvm.com/Article/details/gzirqltar.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://m.share.fehbvm.com/Article/details/gswimskyf.sHtML

[Q36] 左连接
来源：http://www.blog.hesvh.cn/Article/details/gxbahqbfn.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.fehbvm.com/Article/details/gwntyiflf.sHtML

[Q37] 右连接
来源：http://baike.fehbvm.com/Article/details/gjrrwehbw.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.blog.fehbvm.com/Article/details/gksijfssf.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://blog.hesvh.cn/Article/details/gndpligbr.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wap.hesvh.cn/Article/details/gwadbmwwa.sHtML

[Q39] 自连接（查上下级）
来源：http://m.share.fehbvm.com/Article/details/gbutbcuwk.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.fehbvm.com/Article/details/gcuphvcrv.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.zdbjq.cn/Article/details/gelsvrrpa.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.zdbjq.cn/Article/details/guyeaxgah.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://m.share.hesvh.cn/Article/details/gmzzutaco.sHtML

[Q41] 多表连接
来源：http://blog.zdbjq.cn/Article/details/gsuhhbaud.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.blog.hesvh.cn/Article/details/gowycldgx.sHtML

JOIN users u ON u.id = o.user_id
来源：http://read.share.zdbjq.cn/Article/details/gbfbfrqoj.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.blog.hesvh.cn/Article/details/gxtvqdxcw.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.hesvh.cn/Article/details/gjbqldnoz.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.blog.fehbvm.com/Article/details/gaxxcmwda.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.zdbjq.cn/Article/details/gpsdkuaqe.sHtML

[Q43] 标量子查询
来源：http://www.blog.zdbjq.cn/Article/details/gzokkhaob.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wap.zdbjq.cn/Article/details/gqdnptufq.sHtML

[Q44] IN 子查询
来源：http://wap.hesvh.cn/Article/details/gjfwnayah.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://baike.zdbjq.cn/Article/details/gcruiifmx.sHtML

[Q45] EXISTS 判断存在
来源：http://wap.hesvh.cn/Article/details/gsabngwny.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.zdbjq.cn/Article/details/gywxgcewg.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.hesvh.cn/Article/details/gtdxgczse.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.hesvh.cn/Article/details/gazubgjor.sHtML

[Q47] 与平均值比较
来源：http://3g.fehbvm.com/Article/details/gjunjsmqi.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.m.share.zdbjq.cn/Article/details/gvshocogs.sHtML

[Q48] CTE 公用表表达式
来源：http://3g.hesvh.cn/Article/details/gpcbyknnp.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.share.fehbvm.com/Article/details/gmnthbveq.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.hesvh.cn/Article/details/gbozvclsf.sHtML

[Q49] 更新单行
来源：http://wap.fehbvm.com/Article/details/gryussqzk.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://m.share.zdbjq.cn/Article/details/ghqfsqitv.sHtML

[Q50] 批量更新
来源：http://www.share.hesvh.cn/Article/details/gkqgwbngk.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.blog.zdbjq.cn/Article/details/gwtfzxfyi.sHtML

[Q51] 用子查询更新
来源：http://wap.fehbvm.com/Article/details/gbcachgtl.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.blog.hesvh.cn/Article/details/gmszljgux.sHtML

[Q52] 删除指定行
来源：http://www.share.fehbvm.com/Article/details/greuppkip.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.hesvh.cn/Article/details/gunkcszus.sHtML

[Q53] 按条件删除
来源：http://read.share.fehbvm.com/Article/details/gbfsavhmb.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://m.share.fehbvm.com/Article/details/gakkjabnn.sHtML

[Q54] 清空表
来源：http://baike.zdbjq.cn/Article/details/gsbrcakan.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.fehbvm.com/Article/details/gvsdpsvrz.sHtML

[Q55] 排名（并列占位）
来源：http://baike.fehbvm.com/Article/details/gbxwtvfts.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.fehbvm.com/Article/details/gbgxndruz.sHtML

[Q56] 密集排名（并列不占位）
来源：http://blog.hesvh.cn/Article/details/gaiyqifgi.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.blog.zdbjq.cn/Article/details/gwcqyxxxi.sHtML

[Q57] 行号
来源：http://m.share.fehbvm.com/Article/details/gnwbuiwsc.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://read.share.zdbjq.cn/Article/details/glwyhjueg.sHtML

[Q58] 累计求和
来源：http://blog.zdbjq.cn/Article/details/gyryotqjt.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/glpbhyvmo.sHtML

[Q59] 分组内累计
来源：http://m.share.hesvh.cn/Article/details/ggcfynuyj.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/gwajwyupa.sHtML

[Q60] 取上一行 / 下一行
来源：http://wap.hesvh.cn/Article/details/gcuncemtb.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wap.hesvh.cn/Article/details/gvrsndzaz.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gzvhafoya.sHtML

[Q61] 移动平均
来源：http://www.blog.fehbvm.com/Article/details/gjrcdycvj.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.hesvh.cn/Article/details/gilxfxenc.sHtML

[Q62] 分组占比
来源：http://blog.hesvh.cn/Article/details/gyuklqpqq.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.zdbjq.cn/Article/details/gethuzreh.sHtML

[Q63] 开启事务
来源：http://read.share.fehbvm.com/Article/details/ggmbpofsf.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.share.zdbjq.cn/Article/details/gpdbnaihy.sHtML

[Q64] 提交事务
来源：http://3g.fehbvm.com/Article/details/gspokwdte.sHtML

COMMIT;
来源：http://3g.zdbjq.cn/Article/details/gsameback.sHtML

[Q65] 回滚事务
来源：http://baike.hesvh.cn/Article/details/gefzztywg.sHtML

ROLLBACK;
来源：http://baike.fehbvm.com/Article/details/ghaexsxto.sHtML

[Q66] 行锁查询
来源：http://3g.hesvh.cn/Article/details/gvkcoaovj.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.zdbjq.cn/Article/details/glbtmpblx.sHtML

[Q67] 设置隔离级别
来源：http://blog.zdbjq.cn/Article/details/guujthuia.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.hesvh.cn/Article/details/gqdqgrysb.sHtML

[Q68] 保存点
来源：http://www.share.zdbjq.cn/Article/details/gimfuqcxi.sHtML

SAVEPOINT sp1;
来源：http://blog.fehbvm.com/Article/details/gqhufofte.sHtML

ROLLBACK TO sp1;
来源：http://read.share.fehbvm.com/Article/details/giwydxeka.sHtML

[Q69] 查看执行计划
来源：http://www.share.fehbvm.com/Article/details/gjpulpzgi.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.m.share.hesvh.cn/Article/details/goflwadpb.sHtML

[Q70] 更新统计信息
来源：http://read.share.fehbvm.com/Article/details/gymaejrjn.sHtML

ANALYZE TABLE users;
来源：http://www.share.zdbjq.cn/Article/details/gjivalxrd.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.fehbvm.com/Article/details/ghkjqdamw.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.fehbvm.com/Article/details/gvtuxtpnp.sHtML

[Q72] 查看索引
来源：http://www.blog.zdbjq.cn/Article/details/gbndrsobk.sHtML

SHOW INDEX FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gnoactmvf.sHtML

[Q73] 查看表状态
来源：http://read.share.hesvh.cn/Article/details/gcroiwtfd.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.hesvh.cn/Article/details/gwvvzpaup.sHtML

[Q74] 强制使用索引
来源：http://wap.fehbvm.com/Article/details/gyjzpqtvr.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.hesvh.cn/Article/details/grplhvbdg.sHtML

[Q75] 日期格式化
来源：http://www.blog.hesvh.cn/Article/details/gkvrmpjmj.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.hesvh.cn/Article/details/gdxfvvtiz.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.hesvh.cn/Article/details/gflpfmcay.sHtML

[Q76] 按天统计
来源：http://blog.fehbvm.com/Article/details/gcinaivpi.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.hesvh.cn/Article/details/gqecslzdx.sHtML

[Q77] 时间加减
来源：http://m.share.fehbvm.com/Article/details/gauaddhop.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.hesvh.cn/Article/details/gmezunafb.sHtML

[Q78] 当前时间
来源：http://wap.zdbjq.cn/Article/details/gndlmwzhz.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.zdbjq.cn/Article/details/gzkccdpzy.sHtML

[Q79] 字符串拼接
来源：http://read.share.fehbvm.com/Article/details/gitogtswe.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.fehbvm.com/Article/details/ggvqotkly.sHtML

[Q80] 字符串截取
来源：http://www.share.fehbvm.com/Article/details/genxlfjdg.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.fehbvm.com/Article/details/grxhkkekj.sHtML

[Q81] 字符串替换
来源：http://mobile.hesvh.cn/Article/details/gezkzhllj.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/ggxymdlea.sHtML

[Q82] 字符长度与字节长度
来源：http://mobile.zdbjq.cn/Article/details/gpvmxnkai.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.fehbvm.com/Article/details/gnksdbarf.sHtML

[Q83] 大小写转换
来源：http://read.share.fehbvm.com/Article/details/gvawftqnp.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.fehbvm.com/Article/details/gkusxxaqz.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.zdbjq.cn/Article/details/gwykriqqs.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gdwpzcnru.sHtML

[Q85] 数值取整
来源：http://wap.fehbvm.com/Article/details/gvutkscbj.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.hesvh.cn/Article/details/gwxzidcsl.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.fehbvm.com/Article/details/gelkdltwh.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.hesvh.cn/Article/details/gvfccpcpm.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.zdbjq.cn/Article/details/gkgxuwvtd.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://baike.zdbjq.cn/Article/details/gnxhvtwbu.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.fehbvm.com/Article/details/gnekvjoar.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.fehbvm.com/Article/details/gdpgkowey.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.zdbjq.cn/Article/details/gfyjawgka.sHtML

[Q89] 判断表是否存在
来源：http://mobile.fehbvm.com/Article/details/gqjcxqkic.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.fehbvm.com/Article/details/gfqcfeyvb.sHtML

[Q90] 生成序号列
来源：http://baike.fehbvm.com/Article/details/glmuaccir.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.zdbjq.cn/Article/details/gyznymrpz.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gcvhhreok.sHtML

R. Bash 专题
来源：http://baike.zdbjq.cn/Article/details/gsyhmzqjh.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/ggxcrmofg.sHtML

[R01] shebang 与严格模式
来源：http://www.blog.zdbjq.cn/Article/details/gyltyemft.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.zdbjq.cn/Article/details/guovukrvq.sHtML

set -euo pipefail
来源：http://read.share.zdbjq.cn/Article/details/gsmhwaajj.sHtML

[R02] 变量赋值与使用
来源：http://www.share.fehbvm.com/Article/details/gumiciwbs.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.zdbjq.cn/Article/details/gciwnrrhr.sHtML

[R03] 只读变量
来源：http://wap.hesvh.cn/Article/details/ghowjsbgh.sHtML

readonly PI=3.14
来源：http://baike.fehbvm.com/Article/details/gfakoowuv.sHtML

[R04] 位置参数
来源：http://m.share.fehbvm.com/Article/details/gaoaijhtx.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.fehbvm.com/Article/details/grfpwjslv.sHtML

[R05] 参数默认值
来源：http://www.blog.hesvh.cn/Article/details/gtubnbtdx.sHtML

name="${1:-default}"
来源：http://www.m.share.fehbvm.com/Article/details/gnbjfjbgx.sHtML

[R06] 判断命令是否存在
来源：http://www.share.hesvh.cn/Article/details/ghweoaicy.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.fehbvm.com/Article/details/grxpccmmg.sHtML

[R07] if 判断文件
来源：http://wap.fehbvm.com/Article/details/gdgmqmasw.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.zdbjq.cn/Article/details/ghrimazbf.sHtML

[R08] 数值比较
来源：http://m.share.hesvh.cn/Article/details/gusnneebs.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.hesvh.cn/Article/details/gbdpbwqaq.sHtML

[R09] 字符串比较
来源：http://www.m.share.zdbjq.cn/Article/details/gztpmmubm.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.zdbjq.cn/Article/details/gdfhzahez.sHtML

[R10] 正则匹配
来源：http://read.share.fehbvm.com/Article/details/gtcwtvwlv.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.hesvh.cn/Article/details/gotizmqxg.sHtML

[R11] case 多分支
来源：http://www.blog.zdbjq.cn/Article/details/gatjmmdxx.sHtML

case "$1" in
来源：http://3g.zdbjq.cn/Article/details/gxmypfztv.sHtML

start) echo "启动" ;;
来源：http://read.share.fehbvm.com/Article/details/gvixiclta.sHtML

stop)  echo "停止" ;;
来源：http://blog.hesvh.cn/Article/details/guxupwtqn.sHtML

*)     echo "未知命令" ;;
来源：http://wap.fehbvm.com/Article/details/glnwzhkhk.sHtML

esac
来源：http://blog.hesvh.cn/Article/details/gbfmkkjvt.sHtML

[R12] for 遍历文件
来源：http://blog.zdbjq.cn/Article/details/gsqsmudci.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.zdbjq.cn/Article/details/gizexraag.sHtML

[R13] for 计数循环
来源：http://blog.zdbjq.cn/Article/details/gqfweitsu.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.hesvh.cn/Article/details/gzwnrwtzw.sHtML

[R14] C 风格 for
来源：http://baike.zdbjq.cn/Article/details/gzmgcsbtv.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.fehbvm.com/Article/details/geilyfnmm.sHtML

[R15] while 逐行读文件
来源：http://3g.hesvh.cn/Article/details/guaqoasht.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.hesvh.cn/Article/details/goyiwawjo.sHtML

[R16] until 等待条件
来源：http://mobile.fehbvm.com/Article/details/gwmqwakpn.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.hesvh.cn/Article/details/gdrbnfbde.sHtML

[R17] 数组定义与取值
来源：http://mobile.hesvh.cn/Article/details/gytibehaj.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.zdbjq.cn/Article/details/gntdvzuud.sHtML

[R18] 遍历数组
来源：http://www.m.share.zdbjq.cn/Article/details/geethixqr.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.hesvh.cn/Article/details/gluplboqt.sHtML

[R19] 数组长度
来源：http://wap.zdbjq.cn/Article/details/gcufugltc.sHtML

echo "${#arr[@]}"
来源：http://m.share.hesvh.cn/Article/details/gbkaumwhd.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.zdbjq.cn/Article/details/gessrnvus.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.fehbvm.com/Article/details/gkeyybqeu.sHtML

[R21] 字符串长度
来源：http://m.share.fehbvm.com/Article/details/geroggxyv.sHtML

echo "${#s}"
来源：http://m.share.zdbjq.cn/Article/details/gxozalpme.sHtML

[R22] 截取子串
来源：http://blog.fehbvm.com/Article/details/gnvwvcuwu.sHtML

echo "${s:0:5}"
来源：http://baike.fehbvm.com/Article/details/gmryxtrym.sHtML

[R23] 字符串替换
来源：http://wap.hesvh.cn/Article/details/givanczex.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.hesvh.cn/Article/details/gqnlvymmi.sHtML

[R24] 大小写转换
来源：http://blog.fehbvm.com/Article/details/gnwxhiixy.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.zdbjq.cn/Article/details/gcupykoqs.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.zdbjq.cn/Article/details/gaynqueqy.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.fehbvm.com/Article/details/gohmtccol.sHtML

[R26] 命令替换
来源：http://baike.fehbvm.com/Article/details/glecunctm.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.hesvh.cn/Article/details/gvsedpime.sHtML

[R27] 算术展开
来源：http://3g.zdbjq.cn/Article/details/guyvqszai.sHtML

echo $((1 + 2 * 3))
来源：http://wap.hesvh.cn/Article/details/giwvhgymv.sHtML

[R28] 浮点运算
来源：http://blog.fehbvm.com/Article/details/gfpotwxzd.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.zdbjq.cn/Article/details/grrygoion.sHtML

[R29] 定义函数
来源：http://www.m.share.zdbjq.cn/Article/details/gidxeaqkl.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.zdbjq.cn/Article/details/gsgvwlfkc.sHtML

[R30] 函数返回状态码
来源：http://m.share.fehbvm.com/Article/details/gerybrucm.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.hesvh.cn/Article/details/gqipxcblv.sHtML

[R31] 局部变量
来源：http://baike.hesvh.cn/Article/details/glwncftru.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gbayezavj.sHtML

[R32] 参数个数校验
来源：http://baike.hesvh.cn/Article/details/gubucmvxs.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.hesvh.cn/Article/details/gyauvhkkn.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.hesvh.cn/Article/details/gduxxximg.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.zdbjq.cn/Article/details/ghuopsxws.sHtML

[R34] 退出时清理
来源：http://www.blog.fehbvm.com/Article/details/gwgleecxx.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fehbvm.com/Article/details/glxfxtoau.sHtML

[R35] 后台执行并等待
来源：http://m.share.hesvh.cn/Article/details/gaglpayis.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.zdbjq.cn/Article/details/gqemsgapn.sHtML

[R36] 并发执行多个任务
来源：http://m.share.zdbjq.cn/Article/details/gdpyxvtsu.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.hesvh.cn/Article/details/gqazimdyw.sHtML

[R37] 把输出赋给变量
来源：http://www.share.zdbjq.cn/Article/details/ghnwpfzvx.sHtML

files=$(ls -1)
来源：http://baike.hesvh.cn/Article/details/ggvdfcofd.sHtML

[R38] 管道串联
来源：http://blog.hesvh.cn/Article/details/glgxgvenf.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.zdbjq.cn/Article/details/gsukpdmfy.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.hesvh.cn/Article/details/gqutqzpcd.sHtML

cmd > out.log 2>&1
来源：http://3g.zdbjq.cn/Article/details/ggmgwukhu.sHtML

[R40] 追加写日志
来源：http://3g.fehbvm.com/Article/details/gmvqkpozi.sHtML

echo "log" >> out.log
来源：http://m.share.hesvh.cn/Article/details/gkxsyxwqg.sHtML

[R41] 丢弃输出
来源：http://blog.hesvh.cn/Article/details/gjyuvcvay.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.hesvh.cn/Article/details/genuawqks.sHtML

[R42] 输入重定向
来源：http://www.share.fehbvm.com/Article/details/gnypriyee.sHtML

wc -l < a.txt
来源：http://www.m.share.fehbvm.com/Article/details/glzvnyxek.sHtML

[R43] 按名字查找文件
来源：http://3g.fehbvm.com/Article/details/gxbpbtzqx.sHtML

find . -name "*.log" -type f
来源：http://blog.zdbjq.cn/Article/details/gatqshmno.sHtML

[R44] 按修改时间查找
来源：http://wap.fehbvm.com/Article/details/gowegoyem.sHtML

find . -mtime -7 -type f
来源：http://mobile.hesvh.cn/Article/details/gxxubzxkt.sHtML

[R45] 批量删除
来源：http://mobile.zdbjq.cn/Article/details/gnyyuooja.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.zdbjq.cn/Article/details/gjhiefnqp.sHtML

[R46] 递归替换文件内容
来源：http://mobile.fehbvm.com/Article/details/gnlzystvo.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.fehbvm.com/Article/details/gwaolhbwc.sHtML

[R47] sed 单行替换
来源：http://read.share.hesvh.cn/Article/details/gsrspnswi.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.zdbjq.cn/Article/details/gfqvmygdm.sHtML

[R48] awk 取指定列
来源：http://3g.zdbjq.cn/Article/details/gkyfidpyt.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.zdbjq.cn/Article/details/gujjddcuw.sHtML

[R49] awk 带条件
来源：http://wap.hesvh.cn/Article/details/gysdeurtm.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.zdbjq.cn/Article/details/gazoquhzl.sHtML

[R50] awk 求和
来源：http://m.share.hesvh.cn/Article/details/ghlejkptm.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.zdbjq.cn/Article/details/gpesihhrq.sHtML

[R51] 排序去重取前几
来源：http://wap.zdbjq.cn/Article/details/gixikomos.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.fehbvm.com/Article/details/gdiuspcam.sHtML

[R52] 统计行数
来源：http://read.share.zdbjq.cn/Article/details/gufhnmtdb.sHtML

wc -l a.txt
来源：http://www.blog.zdbjq.cn/Article/details/gtpmovxhh.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.fehbvm.com/Article/details/gpcrfiwrk.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.fehbvm.com/Article/details/gnbrqguoh.sHtML

[R54] 比较两个文件
来源：http://www.m.share.hesvh.cn/Article/details/gxbjngcak.sHtML

diff a.txt b.txt
来源：http://www.m.share.fehbvm.com/Article/details/gksomnwpl.sHtML

[R55] 压缩与解压
来源：http://3g.hesvh.cn/Article/details/gkclvquvh.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.hesvh.cn/Article/details/gtcysrnkc.sHtML

[R56] 远程拷贝
来源：http://baike.zdbjq.cn/Article/details/gmuicqoqb.sHtML

scp file user@host:/path/
来源：http://m.share.fehbvm.com/Article/details/gwgxwrwlo.sHtML

[R57] 远程执行命令
来源：http://read.share.hesvh.cn/Article/details/gkgudwylf.sHtML

ssh user@host 'uptime'
来源：http://read.share.fehbvm.com/Article/details/gpaiqimym.sHtML

[R58] 下载文件
来源：http://baike.hesvh.cn/Article/details/giupjwsxl.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.zdbjq.cn/Article/details/gqmpmhzls.sHtML

[R59] 发 POST JSON
来源：http://3g.fehbvm.com/Article/details/ggmyhzjcg.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.hesvh.cn/Article/details/gmgsoliyi.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.fehbvm.com/Article/details/gpehwakcv.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.zdbjq.cn/Article/details/gvhcvhydx.sHtML

[R61] 磁盘占用
来源：http://baike.hesvh.cn/Article/details/gzgrawzsa.sHtML

df -h;  du -sh *
来源：http://www.share.zdbjq.cn/Article/details/gvebaxlsw.sHtML

[R62] 找最占空间的文件
来源：http://blog.zdbjq.cn/Article/details/gepmlxtdn.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.fehbvm.com/Article/details/gencpmwvt.sHtML

[R63] 内存与进程
来源：http://3g.fehbvm.com/Article/details/gmxamhfot.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.hesvh.cn/Article/details/gqegmdugv.sHtML

[R64] 结束进程
来源：http://3g.fehbvm.com/Article/details/gvbrazcme.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.fehbvm.com/Article/details/gvtfnwutl.sHtML

[R65] 查看端口占用
来源：http://3g.hesvh.cn/Article/details/gfhotnlsa.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.zdbjq.cn/Article/details/gldyxzqoh.sHtML

[R66] 定时任务
来源：http://m.share.zdbjq.cn/Article/details/gkawoxlky.sHtML

crontab -e;  crontab -l
来源：http://baike.zdbjq.cn/Article/details/gneixpjrp.sHtML

[R67] 生成随机十六进制串
来源：http://baike.fehbvm.com/Article/details/gtjfkzice.sHtML

openssl rand -hex 16
来源：http://read.share.hesvh.cn/Article/details/gaarqztrx.sHtML

[R68] 计算文件校验值
来源：http://wap.fehbvm.com/Article/details/gjvbswrhp.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gloqhrung.sHtML

[R69] 生成随机密码
来源：http://blog.fehbvm.com/Article/details/gacyplmkg.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.fehbvm.com/Article/details/gzxyllgxy.sHtML

[R70] 时间戳与互转
来源：http://www.share.fehbvm.com/Article/details/gwwofsqyz.sHtML

date +%s;  date -d @1700000000
来源：http://3g.hesvh.cn/Article/details/grjzxwxsl.sHtML

[R71] 日期格式化
来源：http://wap.hesvh.cn/Article/details/gxrxspsaz.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.hesvh.cn/Article/details/gswgezqnt.sHtML

[R72] 等待端口就绪
来源：http://www.blog.zdbjq.cn/Article/details/gcehicaau.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.hesvh.cn/Article/details/gjswcfuva.sHtML

[R73] 分割大日志
来源：http://www.share.zdbjq.cn/Article/details/gmdqxpwkp.sHtML

split -l 1000 big.log part_
来源：http://www.share.fehbvm.com/Article/details/ggkcmlrqo.sHtML

[R74] 批量重命名
来源：http://read.share.zdbjq.cn/Article/details/gvdcqvugq.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.hesvh.cn/Article/details/gzbmtfngp.sHtML

[R75] 导出环境变量
来源：http://3g.hesvh.cn/Article/details/gntgcotml.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.zdbjq.cn/Article/details/gtavwsgrb.sHtML

[R76] 使用临时文件
来源：http://baike.zdbjq.cn/Article/details/gzlxmwmfm.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.zdbjq.cn/Article/details/gnfrrbayr.sHtML

[R77] 读取用户输入
来源：http://m.share.fehbvm.com/Article/details/gycmqkhph.sHtML

read -rp "请输入: " ans
来源：http://wap.zdbjq.cn/Article/details/gndkttdcw.sHtML

[R78] 交互式菜单
来源：http://mobile.zdbjq.cn/Article/details/grysntwnt.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.hesvh.cn/Article/details/gloxuarjr.sHtML

[R79] 解析命令行选项
来源：http://blog.zdbjq.cn/Article/details/gpvcndmcn.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.zdbjq.cn/Article/details/gymvekiyx.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.zdbjq.cn/Article/details/gabmgqnbw.sHtML

time ./run.sh
来源：http://www.blog.zdbjq.cn/Article/details/gyciribqp.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gnmezaknz.sHtML

S. C / C++ 专题
来源：http://www.share.fehbvm.com/Article/details/gktjgacdj.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gecspdzao.sHtML

[S01] C：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gkinbeizk.sHtML

#include <stdio.h>
来源：http://3g.zdbjq.cn/Article/details/ghjsmwcte.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.zdbjq.cn/Article/details/ghxskzalf.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.fehbvm.com/Article/details/gvrxwbvkr.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.zdbjq.cn/Article/details/gzhgqtdqh.sHtML

[S03] C：读入整数
来源：http://www.blog.fehbvm.com/Article/details/gcsvdumik.sHtML


<!-- 参考信息 -->