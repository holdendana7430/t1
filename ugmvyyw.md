代发 wailian999

[Q36] 左连接
来源：http://mobile.hesvh.cn/Article/details/gspprjpzf.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.fehbvm.com/Article/details/gfqnbyzqr.sHtML

[Q37] 右连接
来源：http://www.blog.fehbvm.com/Article/details/gyatvwkrn.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://blog.fehbvm.com/Article/details/gfzrarkve.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://blog.fehbvm.com/Article/details/gfcagaayb.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.zdbjq.cn/Article/details/ghoglpoev.sHtML

[Q39] 自连接（查上下级）
来源：http://3g.hesvh.cn/Article/details/grpymwykr.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.fehbvm.com/Article/details/gcxuwhjwt.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.blog.hesvh.cn/Article/details/gwmtdfkmy.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.fehbvm.com/Article/details/ggozzxxsx.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://m.share.zdbjq.cn/Article/details/gltumsjfh.sHtML

[Q41] 多表连接
来源：http://mobile.hesvh.cn/Article/details/gmhajdbfc.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://3g.hesvh.cn/Article/details/gvyqvxxhn.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.zdbjq.cn/Article/details/gjxdwftnc.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.zdbjq.cn/Article/details/gycdzvwbc.sHtML

[Q42] 连接条件附加过滤
来源：http://blog.fehbvm.com/Article/details/gpcnzrnmm.sHtML

SELECT u.name, o.amount FROM users u
来源：http://3g.zdbjq.cn/Article/details/geentjpbn.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.fehbvm.com/Article/details/grtqdoeke.sHtML

[Q43] 标量子查询
来源：http://wap.fehbvm.com/Article/details/gsfiautrf.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.m.share.hesvh.cn/Article/details/guvvonjtk.sHtML

[Q44] IN 子查询
来源：http://www.share.fehbvm.com/Article/details/gxqiyyzyx.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://baike.zdbjq.cn/Article/details/ggjyuqcpm.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.fehbvm.com/Article/details/gxsmqavcw.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.zdbjq.cn/Article/details/gwbiecyaa.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.fehbvm.com/Article/details/gfhtccddl.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.fehbvm.com/Article/details/gtwbjkfaf.sHtML

[Q47] 与平均值比较
来源：http://baike.zdbjq.cn/Article/details/gqvftdkei.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.m.share.zdbjq.cn/Article/details/ggwdzzsfe.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.hesvh.cn/Article/details/glqkcgces.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://3g.hesvh.cn/Article/details/gsmlpyjxd.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://wap.hesvh.cn/Article/details/gfgkphlnn.sHtML

[Q49] 更新单行
来源：http://m.share.hesvh.cn/Article/details/gluhrhzpy.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://blog.zdbjq.cn/Article/details/guuicuqtb.sHtML

[Q50] 批量更新
来源：http://read.share.hesvh.cn/Article/details/gnvplygwn.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.fehbvm.com/Article/details/gyydencwl.sHtML

[Q51] 用子查询更新
来源：http://read.share.hesvh.cn/Article/details/glmczfkxd.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://3g.hesvh.cn/Article/details/goquxnuuw.sHtML

[Q52] 删除指定行
来源：http://www.m.share.fehbvm.com/Article/details/gznmkntsw.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.zdbjq.cn/Article/details/gdcpardmj.sHtML

[Q53] 按条件删除
来源：http://www.blog.hesvh.cn/Article/details/gztbjluwc.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.blog.zdbjq.cn/Article/details/gvblhykri.sHtML

[Q54] 清空表
来源：http://mobile.zdbjq.cn/Article/details/ghytrfxzw.sHtML

TRUNCATE TABLE logs;
来源：http://www.m.share.zdbjq.cn/Article/details/gvkmtliyp.sHtML

[Q55] 排名（并列占位）
来源：http://wap.hesvh.cn/Article/details/gaqrsfolj.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.blog.zdbjq.cn/Article/details/ghjylbqex.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.fehbvm.com/Article/details/gnedgkqkl.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.fehbvm.com/Article/details/gwdukfxcv.sHtML

[Q57] 行号
来源：http://mobile.zdbjq.cn/Article/details/gimybzxdm.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://3g.hesvh.cn/Article/details/gqoxunvtb.sHtML

[Q58] 累计求和
来源：http://wap.zdbjq.cn/Article/details/gkqnlhggg.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/gvkgwoijd.sHtML

[Q59] 分组内累计
来源：http://www.blog.hesvh.cn/Article/details/gvedjwlpw.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/ggwbepgqc.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.share.zdbjq.cn/Article/details/gzqnddnji.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.hesvh.cn/Article/details/gfxswgktu.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://blog.hesvh.cn/Article/details/gshuafxpk.sHtML

[Q61] 移动平均
来源：http://www.share.zdbjq.cn/Article/details/gbkpefisq.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/gpneuhoxi.sHtML

[Q62] 分组占比
来源：http://baike.zdbjq.cn/Article/details/gjysxnzpy.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://baike.hesvh.cn/Article/details/gioqxwbgd.sHtML

[Q63] 开启事务
来源：http://blog.zdbjq.cn/Article/details/gcxveaubz.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.zdbjq.cn/Article/details/gdfflptsn.sHtML

[Q64] 提交事务
来源：http://3g.zdbjq.cn/Article/details/gtrxotehp.sHtML

COMMIT;
来源：http://m.share.zdbjq.cn/Article/details/gsuoohkqt.sHtML

[Q65] 回滚事务
来源：http://3g.fehbvm.com/Article/details/ghgnahxki.sHtML

ROLLBACK;
来源：http://wap.zdbjq.cn/Article/details/gjflprpcq.sHtML

[Q66] 行锁查询
来源：http://www.blog.hesvh.cn/Article/details/godzqcies.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.hesvh.cn/Article/details/gwzpwbbde.sHtML

[Q67] 设置隔离级别
来源：http://3g.fehbvm.com/Article/details/gghngvcpn.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://3g.zdbjq.cn/Article/details/ggnsduquu.sHtML

[Q68] 保存点
来源：http://baike.fehbvm.com/Article/details/ghjuhvlpn.sHtML

SAVEPOINT sp1;
来源：http://blog.fehbvm.com/Article/details/gfkerznci.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.fehbvm.com/Article/details/grcqunepy.sHtML

[Q69] 查看执行计划
来源：http://baike.hesvh.cn/Article/details/gendcaqiw.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.hesvh.cn/Article/details/gqvjsnxkw.sHtML

[Q70] 更新统计信息
来源：http://www.share.fehbvm.com/Article/details/gfkvefsmv.sHtML

ANALYZE TABLE users;
来源：http://m.share.zdbjq.cn/Article/details/gojuxmipb.sHtML

[Q71] 查看建表语句
来源：http://wap.hesvh.cn/Article/details/gpfpqupwn.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.hesvh.cn/Article/details/gpsckgpab.sHtML

[Q72] 查看索引
来源：http://read.share.hesvh.cn/Article/details/gephkblzr.sHtML

SHOW INDEX FROM users;
来源：http://www.share.fehbvm.com/Article/details/grcoxxocx.sHtML

[Q73] 查看表状态
来源：http://mobile.hesvh.cn/Article/details/gbvsfnzpe.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.fehbvm.com/Article/details/gktrppgvl.sHtML

[Q74] 强制使用索引
来源：http://m.share.fehbvm.com/Article/details/gwdizbxlu.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.fehbvm.com/Article/details/grfaewolr.sHtML

[Q75] 日期格式化
来源：http://www.blog.hesvh.cn/Article/details/gwvnjjteg.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.share.hesvh.cn/Article/details/godpklhmn.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.fehbvm.com/Article/details/gwgzbfzyg.sHtML

[Q76] 按天统计
来源：http://www.blog.fehbvm.com/Article/details/gozielasl.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://3g.hesvh.cn/Article/details/gcbrihjcf.sHtML

[Q77] 时间加减
来源：http://3g.fehbvm.com/Article/details/gnutguasa.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.fehbvm.com/Article/details/gymritgof.sHtML

[Q78] 当前时间
来源：http://baike.zdbjq.cn/Article/details/gcxajpdam.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.hesvh.cn/Article/details/gxscdnepf.sHtML

[Q79] 字符串拼接
来源：http://m.share.hesvh.cn/Article/details/gcdeprwbe.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://m.share.zdbjq.cn/Article/details/ghhworjlz.sHtML

[Q80] 字符串截取
来源：http://3g.hesvh.cn/Article/details/gbpxquswq.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/geajhmdzz.sHtML

[Q81] 字符串替换
来源：http://www.m.share.zdbjq.cn/Article/details/gzjqscpfs.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gidxokcwr.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.fehbvm.com/Article/details/gffafsyjz.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gotxweizm.sHtML

[Q83] 大小写转换
来源：http://mobile.zdbjq.cn/Article/details/gkdzgqqmq.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.zdbjq.cn/Article/details/glhigdfng.sHtML

[Q84] 去除首尾空格
来源：http://blog.zdbjq.cn/Article/details/giffltpbr.sHtML

SELECT TRIM(name) FROM users;
来源：http://mobile.fehbvm.com/Article/details/gsdnseypt.sHtML

[Q85] 数值取整
来源：http://read.share.hesvh.cn/Article/details/gkjywfupv.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.fehbvm.com/Article/details/gltaiwoow.sHtML

[Q86] 读取 JSON 字段
来源：http://blog.hesvh.cn/Article/details/gjopmaztb.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.zdbjq.cn/Article/details/glnngribg.sHtML

[Q87] JSON 字段做条件
来源：http://wap.fehbvm.com/Article/details/gfzoihpfx.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.zdbjq.cn/Article/details/gkdtfqaqn.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.hesvh.cn/Article/details/gjomdkepn.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.zdbjq.cn/Article/details/grgpjegph.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.hesvh.cn/Article/details/gnolkjxzt.sHtML

[Q89] 判断表是否存在
来源：http://wap.hesvh.cn/Article/details/gkiobflmr.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.hesvh.cn/Article/details/gljyrrgup.sHtML

[Q90] 生成序号列
来源：http://baike.zdbjq.cn/Article/details/gmuifizey.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.hesvh.cn/Article/details/gutwvwyht.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gslznxmla.sHtML

R. Bash 专题
来源：http://www.share.zdbjq.cn/Article/details/geowrlzzv.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gzjpefoks.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.hesvh.cn/Article/details/gcuksifcd.sHtML

#!/usr/bin/env bash
来源：http://read.share.zdbjq.cn/Article/details/gapnyiwlr.sHtML

set -euo pipefail
来源：http://blog.zdbjq.cn/Article/details/gbkcclumi.sHtML

[R02] 变量赋值与使用
来源：http://wap.zdbjq.cn/Article/details/geicubatn.sHtML

name="Tom"; echo "$name"
来源：http://m.share.fehbvm.com/Article/details/gijsxhwxp.sHtML

[R03] 只读变量
来源：http://mobile.fehbvm.com/Article/details/ghwmcklyg.sHtML

readonly PI=3.14
来源：http://m.share.fehbvm.com/Article/details/gckkyudoa.sHtML

[R04] 位置参数
来源：http://mobile.fehbvm.com/Article/details/gvtaveuzs.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.fehbvm.com/Article/details/gptrmxtar.sHtML

[R05] 参数默认值
来源：http://blog.zdbjq.cn/Article/details/gdykxrpla.sHtML

name="${1:-default}"
来源：http://blog.hesvh.cn/Article/details/gwbpilwpj.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.hesvh.cn/Article/details/gzmybywwy.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.hesvh.cn/Article/details/gneavqymi.sHtML

[R07] if 判断文件
来源：http://3g.fehbvm.com/Article/details/gosbhbzmo.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.zdbjq.cn/Article/details/gvgpbcwqm.sHtML

[R08] 数值比较
来源：http://m.share.zdbjq.cn/Article/details/gdzpqvhqb.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.fehbvm.com/Article/details/gareqnggh.sHtML

[R09] 字符串比较
来源：http://www.share.hesvh.cn/Article/details/ggqungayg.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.zdbjq.cn/Article/details/gslrnaunz.sHtML

[R10] 正则匹配
来源：http://read.share.fehbvm.com/Article/details/gyrxxouhk.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.zdbjq.cn/Article/details/gwrbfqjdo.sHtML

[R11] case 多分支
来源：http://wap.zdbjq.cn/Article/details/gvdrgfkhg.sHtML

case "$1" in
来源：http://wap.hesvh.cn/Article/details/gqmffmqou.sHtML

start) echo "启动" ;;
来源：http://blog.hesvh.cn/Article/details/gmsvahyny.sHtML

stop)  echo "停止" ;;
来源：http://read.share.zdbjq.cn/Article/details/gfiyuanji.sHtML

*)     echo "未知命令" ;;
来源：http://wap.zdbjq.cn/Article/details/gabqjkxrb.sHtML

esac
来源：http://mobile.fehbvm.com/Article/details/glkmwrjei.sHtML

[R12] for 遍历文件
来源：http://mobile.fehbvm.com/Article/details/ggvqyunfn.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.hesvh.cn/Article/details/gumttxffe.sHtML

[R13] for 计数循环
来源：http://mobile.zdbjq.cn/Article/details/gsksnduho.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.fehbvm.com/Article/details/ggweepona.sHtML

[R14] C 风格 for
来源：http://3g.fehbvm.com/Article/details/gubkwoplp.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.zdbjq.cn/Article/details/gkuozpshs.sHtML

[R15] while 逐行读文件
来源：http://m.share.fehbvm.com/Article/details/gjjhaabzg.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.zdbjq.cn/Article/details/gcapupooj.sHtML

[R16] until 等待条件
来源：http://baike.hesvh.cn/Article/details/gnpmnqale.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.zdbjq.cn/Article/details/gihsbberb.sHtML

[R17] 数组定义与取值
来源：http://baike.fehbvm.com/Article/details/gcqscfjwn.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.fehbvm.com/Article/details/gbctyyfpv.sHtML

[R18] 遍历数组
来源：http://read.share.zdbjq.cn/Article/details/gneqmuckk.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.zdbjq.cn/Article/details/gbycufeis.sHtML

[R19] 数组长度
来源：http://www.share.fehbvm.com/Article/details/gsbzqeimt.sHtML

echo "${#arr[@]}"
来源：http://m.share.zdbjq.cn/Article/details/gvhrrjngp.sHtML

[R20] 关联数组（字典）
来源：http://read.share.zdbjq.cn/Article/details/gxdsiwnng.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.zdbjq.cn/Article/details/gimoelwtx.sHtML

[R21] 字符串长度
来源：http://www.blog.fehbvm.com/Article/details/glhymcepc.sHtML

echo "${#s}"
来源：http://www.share.zdbjq.cn/Article/details/guyjbynlr.sHtML

[R22] 截取子串
来源：http://www.blog.fehbvm.com/Article/details/gsaiqhoff.sHtML

echo "${s:0:5}"
来源：http://mobile.hesvh.cn/Article/details/gqrqzgfhf.sHtML

[R23] 字符串替换
来源：http://www.blog.fehbvm.com/Article/details/gpyziovjd.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.zdbjq.cn/Article/details/ghelselpy.sHtML

[R24] 大小写转换
来源：http://baike.hesvh.cn/Article/details/gyhvlxzlk.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.zdbjq.cn/Article/details/gkwkspkch.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.hesvh.cn/Article/details/gvziopxdf.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.zdbjq.cn/Article/details/gsiidbzbk.sHtML

[R26] 命令替换
来源：http://blog.fehbvm.com/Article/details/gejneirub.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.hesvh.cn/Article/details/gqtfybuef.sHtML

[R27] 算术展开
来源：http://wap.hesvh.cn/Article/details/gigrifmcg.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.fehbvm.com/Article/details/gqwhgdrdd.sHtML

[R28] 浮点运算
来源：http://www.share.fehbvm.com/Article/details/guriiwrsp.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.zdbjq.cn/Article/details/gmfwfabil.sHtML

[R29] 定义函数
来源：http://www.m.share.zdbjq.cn/Article/details/glvbwfdzm.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.zdbjq.cn/Article/details/gjzvokvzf.sHtML

[R30] 函数返回状态码
来源：http://www.share.fehbvm.com/Article/details/gtwfvjiau.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.hesvh.cn/Article/details/ggjmsznzz.sHtML

[R31] 局部变量
来源：http://www.blog.zdbjq.cn/Article/details/gylszvald.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.zdbjq.cn/Article/details/ghvsrzrsg.sHtML

[R32] 参数个数校验
来源：http://m.share.zdbjq.cn/Article/details/gsizogjas.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.fehbvm.com/Article/details/gecgandec.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.zdbjq.cn/Article/details/gnucessnr.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.fehbvm.com/Article/details/golvbqpmi.sHtML

[R34] 退出时清理
来源：http://blog.fehbvm.com/Article/details/geiiclnqd.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fehbvm.com/Article/details/gsaulqdyw.sHtML

[R35] 后台执行并等待
来源：http://mobile.fehbvm.com/Article/details/gthbnnumw.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.zdbjq.cn/Article/details/gklxncfhn.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.fehbvm.com/Article/details/gobekowjd.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.fehbvm.com/Article/details/gsgejbnfk.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.fehbvm.com/Article/details/gtusflhnn.sHtML

files=$(ls -1)
来源：http://wap.hesvh.cn/Article/details/gdtnqdsvu.sHtML

[R38] 管道串联
来源：http://wap.hesvh.cn/Article/details/gjlkokoqv.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.fehbvm.com/Article/details/gogxrbocd.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.zdbjq.cn/Article/details/ghsvtxyuv.sHtML

cmd > out.log 2>&1
来源：http://m.share.hesvh.cn/Article/details/goilrazli.sHtML

[R40] 追加写日志
来源：http://www.m.share.hesvh.cn/Article/details/gaxbxqqil.sHtML

echo "log" >> out.log
来源：http://blog.hesvh.cn/Article/details/gkutkymda.sHtML

[R41] 丢弃输出
来源：http://mobile.hesvh.cn/Article/details/gfdruhvie.sHtML

cmd >/dev/null 2>&1
来源：http://3g.zdbjq.cn/Article/details/grxrefvpl.sHtML

[R42] 输入重定向
来源：http://wap.zdbjq.cn/Article/details/gzycirlva.sHtML

wc -l < a.txt
来源：http://baike.hesvh.cn/Article/details/gchthierx.sHtML

[R43] 按名字查找文件
来源：http://www.blog.hesvh.cn/Article/details/ggxydpxdx.sHtML

find . -name "*.log" -type f
来源：http://mobile.hesvh.cn/Article/details/gcewjeviq.sHtML

[R44] 按修改时间查找
来源：http://read.share.zdbjq.cn/Article/details/grgsclict.sHtML

find . -mtime -7 -type f
来源：http://read.share.zdbjq.cn/Article/details/gdtrdlpwe.sHtML

[R45] 批量删除
来源：http://read.share.fehbvm.com/Article/details/gjdiinqav.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.zdbjq.cn/Article/details/gcwlzlrda.sHtML

[R46] 递归替换文件内容
来源：http://www.share.fehbvm.com/Article/details/gjexhzkwn.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.zdbjq.cn/Article/details/guxsvgnpm.sHtML

[R47] sed 单行替换
来源：http://www.share.zdbjq.cn/Article/details/gstoqbqzc.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.fehbvm.com/Article/details/glnhkehbz.sHtML

[R48] awk 取指定列
来源：http://baike.fehbvm.com/Article/details/gecqrrxfm.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.zdbjq.cn/Article/details/gjjoqwwfy.sHtML

[R49] awk 带条件
来源：http://baike.hesvh.cn/Article/details/gborgxlhj.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.zdbjq.cn/Article/details/genygpinn.sHtML

[R50] awk 求和
来源：http://m.share.zdbjq.cn/Article/details/gyxonqyzj.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.zdbjq.cn/Article/details/givvnngwh.sHtML

[R51] 排序去重取前几
来源：http://www.share.zdbjq.cn/Article/details/gwsjmovcp.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.zdbjq.cn/Article/details/gcypdmdah.sHtML

[R52] 统计行数
来源：http://www.m.share.zdbjq.cn/Article/details/gtcvpntnb.sHtML

wc -l a.txt
来源：http://mobile.hesvh.cn/Article/details/gjwaljbux.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.fehbvm.com/Article/details/gvgnrzypl.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.fehbvm.com/Article/details/gjtdjzaxn.sHtML

[R54] 比较两个文件
来源：http://baike.hesvh.cn/Article/details/gcpocanet.sHtML

diff a.txt b.txt
来源：http://www.blog.hesvh.cn/Article/details/gndzhgtjw.sHtML

[R55] 压缩与解压
来源：http://mobile.zdbjq.cn/Article/details/gaxjfxlau.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.hesvh.cn/Article/details/gtngbvokh.sHtML

[R56] 远程拷贝
来源：http://www.share.zdbjq.cn/Article/details/gmoydeqhv.sHtML

scp file user@host:/path/
来源：http://www.blog.fehbvm.com/Article/details/gsdbymltn.sHtML

[R57] 远程执行命令
来源：http://3g.hesvh.cn/Article/details/gxcoldflt.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.fehbvm.com/Article/details/gkhatghts.sHtML

[R58] 下载文件
来源：http://read.share.fehbvm.com/Article/details/ghxcogymx.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.hesvh.cn/Article/details/gbogdqtbp.sHtML

[R59] 发 POST JSON
来源：http://baike.hesvh.cn/Article/details/gmhwninvv.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.hesvh.cn/Article/details/gnpcsqpgg.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.hesvh.cn/Article/details/glpuqvkhe.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.fehbvm.com/Article/details/gyeurnnkr.sHtML

[R61] 磁盘占用
来源：http://www.m.share.fehbvm.com/Article/details/ggvzcansr.sHtML

df -h;  du -sh *
来源：http://www.share.zdbjq.cn/Article/details/gkcnvccvb.sHtML

[R62] 找最占空间的文件
来源：http://wap.hesvh.cn/Article/details/gisqqhurc.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.fehbvm.com/Article/details/gweuotinh.sHtML

[R63] 内存与进程
来源：http://read.share.fehbvm.com/Article/details/gkxdjrwcn.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.zdbjq.cn/Article/details/gxobxzjge.sHtML

[R64] 结束进程
来源：http://read.share.hesvh.cn/Article/details/gdjewipxc.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.zdbjq.cn/Article/details/givgvnckk.sHtML

[R65] 查看端口占用
来源：http://m.share.fehbvm.com/Article/details/gqcxntqpr.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.hesvh.cn/Article/details/gxigfzjyi.sHtML

[R66] 定时任务
来源：http://wap.zdbjq.cn/Article/details/grozotfsl.sHtML

crontab -e;  crontab -l
来源：http://baike.fehbvm.com/Article/details/gytdhvgjx.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.hesvh.cn/Article/details/gppwzghmz.sHtML

openssl rand -hex 16
来源：http://www.m.share.hesvh.cn/Article/details/gctgdkxxu.sHtML

[R68] 计算文件校验值
来源：http://baike.fehbvm.com/Article/details/gjuxfkczg.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.zdbjq.cn/Article/details/ghmghqvsv.sHtML

[R69] 生成随机密码
来源：http://3g.fehbvm.com/Article/details/gmyghxhan.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.zdbjq.cn/Article/details/ghwutbstt.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.zdbjq.cn/Article/details/gsrbuvzpm.sHtML

date +%s;  date -d @1700000000
来源：http://3g.zdbjq.cn/Article/details/gtkeqkvzx.sHtML

[R71] 日期格式化
来源：http://blog.fehbvm.com/Article/details/gdsiitiea.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.zdbjq.cn/Article/details/grjfzgulr.sHtML

[R72] 等待端口就绪
来源：http://baike.fehbvm.com/Article/details/goiqeltlu.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.fehbvm.com/Article/details/ggqiteeqb.sHtML

[R73] 分割大日志
来源：http://www.share.hesvh.cn/Article/details/ggpabvgly.sHtML

split -l 1000 big.log part_
来源：http://read.share.zdbjq.cn/Article/details/gkxlvblnv.sHtML

[R74] 批量重命名
来源：http://mobile.zdbjq.cn/Article/details/gcxyoiyso.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.zdbjq.cn/Article/details/gnffvbddq.sHtML

[R75] 导出环境变量
来源：http://www.m.share.zdbjq.cn/Article/details/gnvyskpgs.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.zdbjq.cn/Article/details/gafnujtvb.sHtML

[R76] 使用临时文件
来源：http://www.share.zdbjq.cn/Article/details/gynlqdwmx.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.hesvh.cn/Article/details/gbgzpsgyi.sHtML

[R77] 读取用户输入
来源：http://m.share.hesvh.cn/Article/details/ghgqtuwbn.sHtML

read -rp "请输入: " ans
来源：http://baike.fehbvm.com/Article/details/ghkcokixt.sHtML

[R78] 交互式菜单
来源：http://3g.fehbvm.com/Article/details/gxosbjrro.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.hesvh.cn/Article/details/grjglkvfi.sHtML

[R79] 解析命令行选项
来源：http://m.share.hesvh.cn/Article/details/gnoxdzyjt.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.hesvh.cn/Article/details/gqxppkaaj.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.hesvh.cn/Article/details/gczytcmux.sHtML

time ./run.sh
来源：http://wap.hesvh.cn/Article/details/gtlxgfqtd.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/guggwxlag.sHtML

S. C / C++ 专题
来源：http://www.m.share.hesvh.cn/Article/details/gzfmakfke.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/grjshpzxu.sHtML

[S01] C：Hello World
来源：http://wap.fehbvm.com/Article/details/grgdjorbw.sHtML

#include <stdio.h>
来源：http://www.m.share.zdbjq.cn/Article/details/gswopzgkl.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.zdbjq.cn/Article/details/gezbbvsao.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.fehbvm.com/Article/details/grvlxgluj.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.hesvh.cn/Article/details/gniknikvn.sHtML

[S03] C：读入整数
来源：http://blog.hesvh.cn/Article/details/gtlaarsdh.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.fehbvm.com/Article/details/gadupfgqr.sHtML

[S04] C：字符串复制
来源：http://read.share.zdbjq.cn/Article/details/glxlqlmsi.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.fehbvm.com/Article/details/gkiwhnrih.sHtML

[S05] C：字符串长度
来源：http://m.share.hesvh.cn/Article/details/gmiznedxy.sHtML


<!-- 参考信息 -->