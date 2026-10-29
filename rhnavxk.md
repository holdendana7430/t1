代发 wailian999

[Q36] 左连接
来源：http://www.m.share.zdbjq.cn/Article/details/gnjhxfdhv.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://3g.fehbvm.com/Article/details/gpfsltpoj.sHtML

[Q37] 右连接
来源：http://www.m.share.fehbvm.com/Article/details/gbmyoozks.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://m.share.fehbvm.com/Article/details/gshqvharr.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.hesvh.cn/Article/details/gobhtowte.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://read.share.hesvh.cn/Article/details/gghltuovi.sHtML

[Q39] 自连接（查上下级）
来源：http://mobile.fehbvm.com/Article/details/gsnxyxwkc.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.zdbjq.cn/Article/details/gxyebuvbu.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://baike.hesvh.cn/Article/details/gyaurgppm.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.blog.zdbjq.cn/Article/details/gueupeovy.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.fehbvm.com/Article/details/gzaqhufjq.sHtML

[Q41] 多表连接
来源：http://www.m.share.fehbvm.com/Article/details/gibbovfct.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://read.share.fehbvm.com/Article/details/golmopmri.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.share.fehbvm.com/Article/details/gcxvzpfqk.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://mobile.hesvh.cn/Article/details/gnszspgjb.sHtML

[Q42] 连接条件附加过滤
来源：http://mobile.zdbjq.cn/Article/details/guvppznfq.sHtML

SELECT u.name, o.amount FROM users u
来源：http://baike.zdbjq.cn/Article/details/gyxwmmvte.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.fehbvm.com/Article/details/gfrioqrov.sHtML

[Q43] 标量子查询
来源：http://wap.fehbvm.com/Article/details/gfgpejqhh.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wap.fehbvm.com/Article/details/gaqsyavqm.sHtML

[Q44] IN 子查询
来源：http://3g.fehbvm.com/Article/details/gdfketwvq.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.blog.hesvh.cn/Article/details/gaperlmcr.sHtML

[Q45] EXISTS 判断存在
来源：http://wap.fehbvm.com/Article/details/gdburkbpk.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.fehbvm.com/Article/details/ghvmoevvi.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.m.share.fehbvm.com/Article/details/gmbictwgp.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.hesvh.cn/Article/details/gmjtsxmkl.sHtML

[Q47] 与平均值比较
来源：http://wap.fehbvm.com/Article/details/gyfxufchk.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://baike.zdbjq.cn/Article/details/gavcikuua.sHtML

[Q48] CTE 公用表表达式
来源：http://3g.hesvh.cn/Article/details/gndjqovry.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://m.share.zdbjq.cn/Article/details/goxitovnv.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.m.share.fehbvm.com/Article/details/gxofhvfsp.sHtML

[Q49] 更新单行
来源：http://www.blog.zdbjq.cn/Article/details/gohnoxoma.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.blog.fehbvm.com/Article/details/gavqqzpcy.sHtML

[Q50] 批量更新
来源：http://wap.fehbvm.com/Article/details/gosvlzdtv.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.share.fehbvm.com/Article/details/gfvtzaymr.sHtML

[Q51] 用子查询更新
来源：http://3g.zdbjq.cn/Article/details/ghowocbti.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wap.zdbjq.cn/Article/details/geyjrhtqr.sHtML

[Q52] 删除指定行
来源：http://m.share.fehbvm.com/Article/details/goacmxzim.sHtML

DELETE FROM users WHERE id = 10;
来源：http://blog.hesvh.cn/Article/details/gcdgyygvu.sHtML

[Q53] 按条件删除
来源：http://baike.hesvh.cn/Article/details/gmumkxqdj.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.blog.fehbvm.com/Article/details/glzixhcsn.sHtML

[Q54] 清空表
来源：http://read.share.fehbvm.com/Article/details/gxuwucjgi.sHtML

TRUNCATE TABLE logs;
来源：http://wap.zdbjq.cn/Article/details/gduxbffea.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.zdbjq.cn/Article/details/ghxfzxebd.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.share.hesvh.cn/Article/details/grdypixrw.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.m.share.zdbjq.cn/Article/details/glvjdibfq.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.zdbjq.cn/Article/details/gwrivokdi.sHtML

[Q57] 行号
来源：http://mobile.fehbvm.com/Article/details/ghtfppncu.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://m.share.fehbvm.com/Article/details/ghszahvls.sHtML

[Q58] 累计求和
来源：http://read.share.zdbjq.cn/Article/details/goaicsghi.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/gjnwtpowu.sHtML

[Q59] 分组内累计
来源：http://m.share.fehbvm.com/Article/details/gwgydxjpu.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://m.share.hesvh.cn/Article/details/gnxlggoye.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.hesvh.cn/Article/details/gkuecpjhz.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.hesvh.cn/Article/details/gifhmvwul.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.hesvh.cn/Article/details/gzbeveteh.sHtML

[Q61] 移动平均
来源：http://3g.hesvh.cn/Article/details/gyjqmntne.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wap.zdbjq.cn/Article/details/giahlktue.sHtML

[Q62] 分组占比
来源：http://www.blog.zdbjq.cn/Article/details/gjctvgnpv.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.hesvh.cn/Article/details/guwenochf.sHtML

[Q63] 开启事务
来源：http://blog.hesvh.cn/Article/details/gbauzakwf.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://3g.fehbvm.com/Article/details/gcyuhlati.sHtML

[Q64] 提交事务
来源：http://wap.hesvh.cn/Article/details/grrbaulkf.sHtML

COMMIT;
来源：http://3g.zdbjq.cn/Article/details/gbvxahzjw.sHtML

[Q65] 回滚事务
来源：http://www.blog.zdbjq.cn/Article/details/gwfcqerat.sHtML

ROLLBACK;
来源：http://www.share.fehbvm.com/Article/details/giyezpsyo.sHtML

[Q66] 行锁查询
来源：http://www.share.hesvh.cn/Article/details/gmtrefkrf.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mobile.fehbvm.com/Article/details/geasyynoh.sHtML

[Q67] 设置隔离级别
来源：http://read.share.fehbvm.com/Article/details/gujlthlxd.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.zdbjq.cn/Article/details/gdxemnets.sHtML

[Q68] 保存点
来源：http://blog.hesvh.cn/Article/details/gglblyvbs.sHtML

SAVEPOINT sp1;
来源：http://mobile.zdbjq.cn/Article/details/gvbzklwup.sHtML

ROLLBACK TO sp1;
来源：http://wap.hesvh.cn/Article/details/gywglhupd.sHtML

[Q69] 查看执行计划
来源：http://wap.hesvh.cn/Article/details/gshqrfeyv.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.zdbjq.cn/Article/details/gmdqazjqr.sHtML

[Q70] 更新统计信息
来源：http://www.m.share.fehbvm.com/Article/details/gvkqwuhbo.sHtML

ANALYZE TABLE users;
来源：http://www.blog.hesvh.cn/Article/details/gtamejxea.sHtML

[Q71] 查看建表语句
来源：http://m.share.zdbjq.cn/Article/details/gsxynqxmt.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wap.fehbvm.com/Article/details/gjyzvelzw.sHtML

[Q72] 查看索引
来源：http://www.share.fehbvm.com/Article/details/gjhshqclb.sHtML

SHOW INDEX FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/godekdrei.sHtML

[Q73] 查看表状态
来源：http://m.share.zdbjq.cn/Article/details/grqljvyyo.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.fehbvm.com/Article/details/gezevwlaa.sHtML

[Q74] 强制使用索引
来源：http://3g.fehbvm.com/Article/details/gbjdsvbgr.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.zdbjq.cn/Article/details/gdkjchbub.sHtML

[Q75] 日期格式化
来源：http://www.blog.fehbvm.com/Article/details/gcqcxzkir.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/gtnpsxgra.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.blog.hesvh.cn/Article/details/gbichusxn.sHtML

[Q76] 按天统计
来源：http://www.blog.hesvh.cn/Article/details/guacfenjf.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.fehbvm.com/Article/details/gejtlninv.sHtML

[Q77] 时间加减
来源：http://www.share.fehbvm.com/Article/details/gmpnnkmgr.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.zdbjq.cn/Article/details/gzfeehjkj.sHtML

[Q78] 当前时间
来源：http://blog.zdbjq.cn/Article/details/grrhstlqo.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.zdbjq.cn/Article/details/gwmocqoia.sHtML

[Q79] 字符串拼接
来源：http://read.share.fehbvm.com/Article/details/gmghdwsym.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.hesvh.cn/Article/details/gnuqwxidl.sHtML

[Q80] 字符串截取
来源：http://www.m.share.fehbvm.com/Article/details/gcphqbehu.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gudfeyadi.sHtML

[Q81] 字符串替换
来源：http://www.share.hesvh.cn/Article/details/goaljvjxi.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.hesvh.cn/Article/details/gzvkzhibj.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.hesvh.cn/Article/details/gecfqeofh.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gnlkjglng.sHtML

[Q83] 大小写转换
来源：http://mobile.zdbjq.cn/Article/details/giymtxpyo.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gwrrgnvxt.sHtML

[Q84] 去除首尾空格
来源：http://m.share.zdbjq.cn/Article/details/gwnxaptbi.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gvrxgjjoa.sHtML

[Q85] 数值取整
来源：http://baike.hesvh.cn/Article/details/gsrvpqjpq.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.hesvh.cn/Article/details/gdbskvcvc.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.fehbvm.com/Article/details/ggfvijhjw.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.hesvh.cn/Article/details/gkncajpzr.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.hesvh.cn/Article/details/gstcomdgw.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.zdbjq.cn/Article/details/gsblsclca.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.zdbjq.cn/Article/details/gflkmajxq.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://3g.fehbvm.com/Article/details/gnzxxymzu.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.fehbvm.com/Article/details/gusuqijae.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.hesvh.cn/Article/details/gntnafxul.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.fehbvm.com/Article/details/gzksfqmdu.sHtML

[Q90] 生成序号列
来源：http://www.blog.zdbjq.cn/Article/details/gxpsyaxkf.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.zdbjq.cn/Article/details/gulltqexd.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gycmebadw.sHtML

R. Bash 专题
来源：http://www.share.zdbjq.cn/Article/details/gtpzwvmph.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gqszfnhvj.sHtML

[R01] shebang 与严格模式
来源：http://www.blog.hesvh.cn/Article/details/gwidadwfz.sHtML

#!/usr/bin/env bash
来源：http://mobile.fehbvm.com/Article/details/gkxwrtkih.sHtML

set -euo pipefail
来源：http://m.share.hesvh.cn/Article/details/gntucmxqa.sHtML

[R02] 变量赋值与使用
来源：http://mobile.fehbvm.com/Article/details/gajgloncd.sHtML

name="Tom"; echo "$name"
来源：http://www.share.fehbvm.com/Article/details/gbxduycdz.sHtML

[R03] 只读变量
来源：http://read.share.fehbvm.com/Article/details/gxfgezhsb.sHtML

readonly PI=3.14
来源：http://blog.hesvh.cn/Article/details/glodtrlzl.sHtML

[R04] 位置参数
来源：http://3g.fehbvm.com/Article/details/gkubviyuo.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.fehbvm.com/Article/details/ghaybgvms.sHtML

[R05] 参数默认值
来源：http://www.blog.hesvh.cn/Article/details/gpxatqhhc.sHtML

name="${1:-default}"
来源：http://m.share.zdbjq.cn/Article/details/guvqkzwot.sHtML

[R06] 判断命令是否存在
来源：http://read.share.zdbjq.cn/Article/details/gxzwfxech.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.zdbjq.cn/Article/details/gmihfwdip.sHtML

[R07] if 判断文件
来源：http://wap.fehbvm.com/Article/details/ggggxbrpj.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.fehbvm.com/Article/details/gxhveuspm.sHtML

[R08] 数值比较
来源：http://blog.fehbvm.com/Article/details/gjjurvcqj.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://mobile.fehbvm.com/Article/details/gclggyjwm.sHtML

[R09] 字符串比较
来源：http://m.share.fehbvm.com/Article/details/ginydikxc.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.fehbvm.com/Article/details/gknnptdqe.sHtML

[R10] 正则匹配
来源：http://baike.zdbjq.cn/Article/details/gxwobancx.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.zdbjq.cn/Article/details/ghjwqaswn.sHtML

[R11] case 多分支
来源：http://wap.zdbjq.cn/Article/details/gjmkayuzv.sHtML

case "$1" in
来源：http://www.blog.zdbjq.cn/Article/details/gtfwwocfu.sHtML

start) echo "启动" ;;
来源：http://blog.zdbjq.cn/Article/details/gemsqvzyi.sHtML

stop)  echo "停止" ;;
来源：http://blog.fehbvm.com/Article/details/gnjjxneol.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.fehbvm.com/Article/details/gbcgsgbfp.sHtML

esac
来源：http://3g.zdbjq.cn/Article/details/guviesiff.sHtML

[R12] for 遍历文件
来源：http://read.share.fehbvm.com/Article/details/gpkbvwgju.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.hesvh.cn/Article/details/gaalhlbeu.sHtML

[R13] for 计数循环
来源：http://3g.hesvh.cn/Article/details/glegnbeyi.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.hesvh.cn/Article/details/gnmskxwwx.sHtML

[R14] C 风格 for
来源：http://m.share.fehbvm.com/Article/details/gilovdmku.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.zdbjq.cn/Article/details/gefkiemfo.sHtML

[R15] while 逐行读文件
来源：http://3g.zdbjq.cn/Article/details/gpjmqymkk.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.zdbjq.cn/Article/details/gikztclqw.sHtML

[R16] until 等待条件
来源：http://3g.fehbvm.com/Article/details/gjoacsoox.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.fehbvm.com/Article/details/gvynlfrjb.sHtML

[R17] 数组定义与取值
来源：http://blog.hesvh.cn/Article/details/gzvqsvbmi.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.zdbjq.cn/Article/details/gjrbbcuip.sHtML

[R18] 遍历数组
来源：http://baike.fehbvm.com/Article/details/gxxytqpbu.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.fehbvm.com/Article/details/gbzimliol.sHtML

[R19] 数组长度
来源：http://mobile.fehbvm.com/Article/details/ggcqcapxk.sHtML

echo "${#arr[@]}"
来源：http://read.share.zdbjq.cn/Article/details/ghaxpnoml.sHtML

[R20] 关联数组（字典）
来源：http://blog.hesvh.cn/Article/details/gzwydbpyt.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.hesvh.cn/Article/details/gecmmzgqo.sHtML

[R21] 字符串长度
来源：http://baike.hesvh.cn/Article/details/geypzbjiu.sHtML

echo "${#s}"
来源：http://m.share.hesvh.cn/Article/details/gyvaiftlc.sHtML

[R22] 截取子串
来源：http://www.m.share.fehbvm.com/Article/details/gtxyizgdu.sHtML

echo "${s:0:5}"
来源：http://wap.hesvh.cn/Article/details/gipymngui.sHtML

[R23] 字符串替换
来源：http://www.blog.hesvh.cn/Article/details/gwkehidie.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.fehbvm.com/Article/details/gjndlrheh.sHtML

[R24] 大小写转换
来源：http://www.m.share.zdbjq.cn/Article/details/gfzczleja.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.hesvh.cn/Article/details/gdeciljqe.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.hesvh.cn/Article/details/gsulvexcz.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.hesvh.cn/Article/details/garypwpke.sHtML

[R26] 命令替换
来源：http://mobile.zdbjq.cn/Article/details/gvpulgmex.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.fehbvm.com/Article/details/geqswrpis.sHtML

[R27] 算术展开
来源：http://www.blog.zdbjq.cn/Article/details/gufyavyak.sHtML

echo $((1 + 2 * 3))
来源：http://baike.hesvh.cn/Article/details/gxgfaadow.sHtML

[R28] 浮点运算
来源：http://www.m.share.fehbvm.com/Article/details/gcbsusxfz.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.zdbjq.cn/Article/details/gyjiuvsxq.sHtML

[R29] 定义函数
来源：http://mobile.fehbvm.com/Article/details/gudgpjxmo.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.hesvh.cn/Article/details/gwffgmsqg.sHtML

[R30] 函数返回状态码
来源：http://mobile.zdbjq.cn/Article/details/gyqhnplyi.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.fehbvm.com/Article/details/goqqpvmfg.sHtML

[R31] 局部变量
来源：http://read.share.fehbvm.com/Article/details/gzsabpjqs.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.fehbvm.com/Article/details/gtehbthng.sHtML

[R32] 参数个数校验
来源：http://read.share.hesvh.cn/Article/details/gbphgukjz.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.hesvh.cn/Article/details/gaczbcpzh.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.hesvh.cn/Article/details/gvvhhrtjr.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.hesvh.cn/Article/details/gucburvoa.sHtML

[R34] 退出时清理
来源：http://wap.zdbjq.cn/Article/details/gqtraqtlh.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.hesvh.cn/Article/details/gxdhydiym.sHtML

[R35] 后台执行并等待
来源：http://baike.fehbvm.com/Article/details/gggurbjnc.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.hesvh.cn/Article/details/ghcerwmhb.sHtML

[R36] 并发执行多个任务
来源：http://wap.fehbvm.com/Article/details/gtlequkbm.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.hesvh.cn/Article/details/gqevixvdv.sHtML

[R37] 把输出赋给变量
来源：http://3g.hesvh.cn/Article/details/gmvxvaolz.sHtML

files=$(ls -1)
来源：http://www.blog.fehbvm.com/Article/details/gsniftsri.sHtML

[R38] 管道串联
来源：http://m.share.zdbjq.cn/Article/details/gieodrebd.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.fehbvm.com/Article/details/gsbodmqzt.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.hesvh.cn/Article/details/ghhvmrmnu.sHtML

cmd > out.log 2>&1
来源：http://3g.hesvh.cn/Article/details/gzqwitqii.sHtML

[R40] 追加写日志
来源：http://www.share.fehbvm.com/Article/details/gosxuwosh.sHtML

echo "log" >> out.log
来源：http://m.share.zdbjq.cn/Article/details/gszzqfhdb.sHtML

[R41] 丢弃输出
来源：http://3g.hesvh.cn/Article/details/gtpqlibrm.sHtML

cmd >/dev/null 2>&1
来源：http://wap.hesvh.cn/Article/details/gtkyzyqxj.sHtML

[R42] 输入重定向
来源：http://3g.zdbjq.cn/Article/details/gysngjent.sHtML

wc -l < a.txt
来源：http://www.share.fehbvm.com/Article/details/grccshncs.sHtML

[R43] 按名字查找文件
来源：http://www.blog.fehbvm.com/Article/details/gyayxdhfd.sHtML

find . -name "*.log" -type f
来源：http://mobile.zdbjq.cn/Article/details/gasnnjsui.sHtML

[R44] 按修改时间查找
来源：http://www.blog.fehbvm.com/Article/details/gfeviytyv.sHtML

find . -mtime -7 -type f
来源：http://m.share.hesvh.cn/Article/details/gbhcuydfh.sHtML

[R45] 批量删除
来源：http://www.m.share.zdbjq.cn/Article/details/gnndoghro.sHtML

find . -name "*.tmp" -delete
来源：http://baike.hesvh.cn/Article/details/gipdyeemh.sHtML

[R46] 递归替换文件内容
来源：http://3g.hesvh.cn/Article/details/gixzjmhwh.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.fehbvm.com/Article/details/gjirpfyxp.sHtML

[R47] sed 单行替换
来源：http://mobile.fehbvm.com/Article/details/gbdtaaisv.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.hesvh.cn/Article/details/gbpwtegwl.sHtML

[R48] awk 取指定列
来源：http://wap.hesvh.cn/Article/details/gwsoeozqa.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.zdbjq.cn/Article/details/gdlvyiidd.sHtML

[R49] awk 带条件
来源：http://3g.fehbvm.com/Article/details/gkzkpcbhd.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.fehbvm.com/Article/details/giomybpqx.sHtML

[R50] awk 求和
来源：http://wap.hesvh.cn/Article/details/grgwruakn.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.zdbjq.cn/Article/details/gjyluccqe.sHtML

[R51] 排序去重取前几
来源：http://blog.hesvh.cn/Article/details/gxzujlwbj.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.zdbjq.cn/Article/details/ggryxylmq.sHtML

[R52] 统计行数
来源：http://mobile.fehbvm.com/Article/details/gsebbmzej.sHtML

wc -l a.txt
来源：http://blog.fehbvm.com/Article/details/gfhjqdyml.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.zdbjq.cn/Article/details/gdlslfubo.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.zdbjq.cn/Article/details/gicvlzflf.sHtML

[R54] 比较两个文件
来源：http://www.share.zdbjq.cn/Article/details/gwswadbph.sHtML

diff a.txt b.txt
来源：http://blog.zdbjq.cn/Article/details/gsmilwwts.sHtML

[R55] 压缩与解压
来源：http://www.share.fehbvm.com/Article/details/gbflocapo.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.fehbvm.com/Article/details/genlgycwd.sHtML

[R56] 远程拷贝
来源：http://www.m.share.zdbjq.cn/Article/details/grifvuaqa.sHtML

scp file user@host:/path/
来源：http://3g.hesvh.cn/Article/details/ggkxptfkb.sHtML

[R57] 远程执行命令
来源：http://read.share.fehbvm.com/Article/details/ghfldhcqa.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.fehbvm.com/Article/details/gyjocgzvv.sHtML

[R58] 下载文件
来源：http://www.m.share.zdbjq.cn/Article/details/goyzqvtel.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.fehbvm.com/Article/details/gsaoibtwe.sHtML

[R59] 发 POST JSON
来源：http://mobile.hesvh.cn/Article/details/glhxmbxix.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.hesvh.cn/Article/details/gbiwysgka.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.hesvh.cn/Article/details/gdmydvota.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.zdbjq.cn/Article/details/gwngiodte.sHtML

[R61] 磁盘占用
来源：http://3g.fehbvm.com/Article/details/gbxfzshfr.sHtML

df -h;  du -sh *
来源：http://blog.zdbjq.cn/Article/details/gapbtfpiy.sHtML

[R62] 找最占空间的文件
来源：http://blog.zdbjq.cn/Article/details/gwtxlspqp.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.zdbjq.cn/Article/details/gdwrxjqyo.sHtML

[R63] 内存与进程
来源：http://3g.zdbjq.cn/Article/details/gwznzpklb.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.hesvh.cn/Article/details/gbwvtvkku.sHtML

[R64] 结束进程
来源：http://www.m.share.hesvh.cn/Article/details/gystwhwtj.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.hesvh.cn/Article/details/gvyvaxloa.sHtML

[R65] 查看端口占用
来源：http://www.m.share.zdbjq.cn/Article/details/gmkulwacd.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.zdbjq.cn/Article/details/gyhezdvqh.sHtML

[R66] 定时任务
来源：http://wap.fehbvm.com/Article/details/gckrbfjie.sHtML

crontab -e;  crontab -l
来源：http://wap.fehbvm.com/Article/details/gswvkhztj.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.hesvh.cn/Article/details/gntajgqbi.sHtML

openssl rand -hex 16
来源：http://www.share.fehbvm.com/Article/details/gptaefsca.sHtML

[R68] 计算文件校验值
来源：http://baike.hesvh.cn/Article/details/gwnlimdkb.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.fehbvm.com/Article/details/gttycildi.sHtML

[R69] 生成随机密码
来源：http://read.share.zdbjq.cn/Article/details/gvfqnheah.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.hesvh.cn/Article/details/gcszwipow.sHtML

[R70] 时间戳与互转
来源：http://wap.fehbvm.com/Article/details/grzelwqwz.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.fehbvm.com/Article/details/gkuneauht.sHtML

[R71] 日期格式化
来源：http://baike.hesvh.cn/Article/details/ghjvwjhzq.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.hesvh.cn/Article/details/gabkcrjdi.sHtML

[R72] 等待端口就绪
来源：http://wap.hesvh.cn/Article/details/gqvqjvffi.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.fehbvm.com/Article/details/gvqgjfdpe.sHtML

[R73] 分割大日志
来源：http://wap.zdbjq.cn/Article/details/gjjaszijm.sHtML

split -l 1000 big.log part_
来源：http://mobile.zdbjq.cn/Article/details/gfapvmubs.sHtML

[R74] 批量重命名
来源：http://baike.fehbvm.com/Article/details/gaugqmcvi.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.hesvh.cn/Article/details/gvbrfobzi.sHtML

[R75] 导出环境变量
来源：http://baike.fehbvm.com/Article/details/gvtkeucht.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.zdbjq.cn/Article/details/gazkxjfgi.sHtML

[R76] 使用临时文件
来源：http://read.share.zdbjq.cn/Article/details/gzvqjfhnr.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.hesvh.cn/Article/details/ghtjrejdf.sHtML

[R77] 读取用户输入
来源：http://www.share.fehbvm.com/Article/details/gcoximinv.sHtML

read -rp "请输入: " ans
来源：http://blog.fehbvm.com/Article/details/gnezwhdph.sHtML

[R78] 交互式菜单
来源：http://wap.hesvh.cn/Article/details/gnolnpkit.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.fehbvm.com/Article/details/goqhbyfyw.sHtML

[R79] 解析命令行选项
来源：http://www.blog.fehbvm.com/Article/details/gumcetaar.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.fehbvm.com/Article/details/gesjwlmob.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.hesvh.cn/Article/details/gtpuzzywm.sHtML

time ./run.sh
来源：http://baike.fehbvm.com/Article/details/gkhaypvje.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gnvaxbzjy.sHtML

S. C / C++ 专题
来源：http://mobile.hesvh.cn/Article/details/gesplmlpt.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/ghtvmhpuf.sHtML

[S01] C：Hello World
来源：http://mobile.hesvh.cn/Article/details/gvrgrartx.sHtML

#include <stdio.h>
来源：http://wap.zdbjq.cn/Article/details/gishubtka.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.hesvh.cn/Article/details/gquskqsok.sHtML

[S02] C：变量与格式化输出
来源：http://blog.hesvh.cn/Article/details/gaqghwyjo.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.zdbjq.cn/Article/details/gqfbgjgit.sHtML

[S03] C：读入整数
来源：http://read.share.hesvh.cn/Article/details/givfjnzxt.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.fehbvm.com/Article/details/gvoaabmav.sHtML

[S04] C：字符串复制
来源：http://3g.zdbjq.cn/Article/details/gzkysckge.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.hesvh.cn/Article/details/gmmpwgrsr.sHtML

[S05] C：字符串长度
来源：http://blog.fehbvm.com/Article/details/gudgdksba.sHtML


<!-- 参考信息 -->