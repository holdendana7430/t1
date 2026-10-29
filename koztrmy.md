代发 wailian999

SELECT o.id, u.name, p.title FROM orders o
来源：http://blog.zdbjq.cn/Article/details/gfflzbfeh.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.blog.hesvh.cn/Article/details/gagvgmszi.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://wap.zdbjq.cn/Article/details/ggiislqbu.sHtML

[Q42] 连接条件附加过滤
来源：http://www.share.zdbjq.cn/Article/details/gwkwuxlft.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.share.hesvh.cn/Article/details/gklixjhmp.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://m.share.fehbvm.com/Article/details/ghucmvolb.sHtML

[Q43] 标量子查询
来源：http://3g.fehbvm.com/Article/details/gmbokwaxw.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.zdbjq.cn/Article/details/glfwcbxiz.sHtML

[Q44] IN 子查询
来源：http://wap.zdbjq.cn/Article/details/gttrnzbqy.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://blog.fehbvm.com/Article/details/geteeaigr.sHtML

[Q45] EXISTS 判断存在
来源：http://m.share.hesvh.cn/Article/details/gmmmrpntt.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.fehbvm.com/Article/details/gcldmwkii.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.share.hesvh.cn/Article/details/gemojcdjt.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.fehbvm.com/Article/details/gjhwvtvka.sHtML

[Q47] 与平均值比较
来源：http://read.share.hesvh.cn/Article/details/gjmutzbkk.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://read.share.zdbjq.cn/Article/details/gnyyamszq.sHtML

[Q48] CTE 公用表表达式
来源：http://www.share.hesvh.cn/Article/details/gtgmssouu.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.m.share.fehbvm.com/Article/details/gvcjowiuq.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://3g.zdbjq.cn/Article/details/gmokdaqog.sHtML

[Q49] 更新单行
来源：http://mobile.hesvh.cn/Article/details/gxzulvebh.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.zdbjq.cn/Article/details/glmycckuw.sHtML

[Q50] 批量更新
来源：http://www.m.share.zdbjq.cn/Article/details/gurlmewpe.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.zdbjq.cn/Article/details/gyboyykaw.sHtML

[Q51] 用子查询更新
来源：http://read.share.hesvh.cn/Article/details/gsaqxgeih.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://3g.fehbvm.com/Article/details/gsjgkehhx.sHtML

[Q52] 删除指定行
来源：http://blog.hesvh.cn/Article/details/gevfgbcrs.sHtML

DELETE FROM users WHERE id = 10;
来源：http://blog.hesvh.cn/Article/details/glrbvdqhc.sHtML

[Q53] 按条件删除
来源：http://blog.hesvh.cn/Article/details/gjdkfayud.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wap.hesvh.cn/Article/details/gliwuovpv.sHtML

[Q54] 清空表
来源：http://mobile.zdbjq.cn/Article/details/gukcmfgvr.sHtML

TRUNCATE TABLE logs;
来源：http://www.m.share.zdbjq.cn/Article/details/ghksltils.sHtML

[Q55] 排名（并列占位）
来源：http://blog.zdbjq.cn/Article/details/gzjbwhcpx.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.fehbvm.com/Article/details/gibntyalm.sHtML

[Q56] 密集排名（并列不占位）
来源：http://blog.zdbjq.cn/Article/details/gkzqegamu.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.share.fehbvm.com/Article/details/ghcebrtwk.sHtML

[Q57] 行号
来源：http://www.share.hesvh.cn/Article/details/grqwqifiv.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gcujhykvm.sHtML

[Q58] 累计求和
来源：http://read.share.fehbvm.com/Article/details/ggtrxmkuj.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wap.zdbjq.cn/Article/details/gpmcfzfmt.sHtML

[Q59] 分组内累计
来源：http://blog.fehbvm.com/Article/details/gcobyfgid.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://read.share.fehbvm.com/Article/details/gquabvetm.sHtML

[Q60] 取上一行 / 下一行
来源：http://wap.hesvh.cn/Article/details/gohpnxrud.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://blog.hesvh.cn/Article/details/gfhuetbtw.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gukzejbjq.sHtML

[Q61] 移动平均
来源：http://www.share.fehbvm.com/Article/details/gsgsokldj.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.fehbvm.com/Article/details/ggqjgefsf.sHtML

[Q62] 分组占比
来源：http://www.share.hesvh.cn/Article/details/gmqgwznka.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.fehbvm.com/Article/details/gzqcvfnax.sHtML

[Q63] 开启事务
来源：http://www.m.share.hesvh.cn/Article/details/gocvmzjmf.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://3g.hesvh.cn/Article/details/gyingjzjx.sHtML

[Q64] 提交事务
来源：http://3g.fehbvm.com/Article/details/grpridqhr.sHtML

COMMIT;
来源：http://www.blog.fehbvm.com/Article/details/gjjaxuysb.sHtML

[Q65] 回滚事务
来源：http://3g.fehbvm.com/Article/details/gxmxilabw.sHtML

ROLLBACK;
来源：http://baike.fehbvm.com/Article/details/gsyoedxwn.sHtML

[Q66] 行锁查询
来源：http://www.share.fehbvm.com/Article/details/gtrwjsvxr.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.blog.hesvh.cn/Article/details/gnpfzdyby.sHtML

[Q67] 设置隔离级别
来源：http://m.share.zdbjq.cn/Article/details/gfprlwvro.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.zdbjq.cn/Article/details/grpunagag.sHtML

[Q68] 保存点
来源：http://blog.fehbvm.com/Article/details/gskmvaqbp.sHtML

SAVEPOINT sp1;
来源：http://read.share.hesvh.cn/Article/details/gbjnvlskz.sHtML

ROLLBACK TO sp1;
来源：http://mobile.zdbjq.cn/Article/details/gnbqeacjn.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.zdbjq.cn/Article/details/gayopshsg.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.zdbjq.cn/Article/details/gibrdknan.sHtML

[Q70] 更新统计信息
来源：http://read.share.hesvh.cn/Article/details/ggeojqcvs.sHtML

ANALYZE TABLE users;
来源：http://3g.fehbvm.com/Article/details/gplwvafuf.sHtML

[Q71] 查看建表语句
来源：http://m.share.zdbjq.cn/Article/details/ghrhkpppb.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wap.zdbjq.cn/Article/details/gzbuifsow.sHtML

[Q72] 查看索引
来源：http://blog.fehbvm.com/Article/details/gjpchwhoq.sHtML

SHOW INDEX FROM users;
来源：http://m.share.fehbvm.com/Article/details/getrsjpqe.sHtML

[Q73] 查看表状态
来源：http://3g.fehbvm.com/Article/details/goicdhulg.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.zdbjq.cn/Article/details/gqaeawspy.sHtML

[Q74] 强制使用索引
来源：http://wap.zdbjq.cn/Article/details/gfkraiqjy.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.zdbjq.cn/Article/details/gqoidfnmu.sHtML

[Q75] 日期格式化
来源：http://www.share.hesvh.cn/Article/details/guwdgovqu.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.zdbjq.cn/Article/details/gltziuuul.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.zdbjq.cn/Article/details/geiufqjgr.sHtML

[Q76] 按天统计
来源：http://mobile.fehbvm.com/Article/details/gwfyhofgq.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://3g.zdbjq.cn/Article/details/gjbirxgfc.sHtML

[Q77] 时间加减
来源：http://mobile.zdbjq.cn/Article/details/gcrbifrqb.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.fehbvm.com/Article/details/gyssgubao.sHtML

[Q78] 当前时间
来源：http://www.blog.zdbjq.cn/Article/details/gocykoufk.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.m.share.zdbjq.cn/Article/details/gqxovvovc.sHtML

[Q79] 字符串拼接
来源：http://m.share.hesvh.cn/Article/details/gmjtwvlqf.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.hesvh.cn/Article/details/gabszwkeg.sHtML

[Q80] 字符串截取
来源：http://www.blog.fehbvm.com/Article/details/gcrjjxjuj.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.fehbvm.com/Article/details/ggllrzotu.sHtML

[Q81] 字符串替换
来源：http://www.share.hesvh.cn/Article/details/gwoakgtfi.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gwzaeequn.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.hesvh.cn/Article/details/gattbreev.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://baike.zdbjq.cn/Article/details/glqrxvqdz.sHtML

[Q83] 大小写转换
来源：http://www.share.hesvh.cn/Article/details/gqgjdbxqx.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/ghjwdxvza.sHtML

[Q84] 去除首尾空格
来源：http://wap.zdbjq.cn/Article/details/gkiqjclra.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gzaksevmr.sHtML

[Q85] 数值取整
来源：http://baike.hesvh.cn/Article/details/gfxpbwjng.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.hesvh.cn/Article/details/gemdvmvvg.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.fehbvm.com/Article/details/gpptsbuyj.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wap.hesvh.cn/Article/details/gduiaxaic.sHtML

[Q87] JSON 字段做条件
来源：http://baike.hesvh.cn/Article/details/gxwzvdaqr.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://baike.hesvh.cn/Article/details/gcpvrnyaz.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.hesvh.cn/Article/details/gywnpsayn.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.fehbvm.com/Article/details/garijwskx.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/ggfkuvbvt.sHtML

[Q89] 判断表是否存在
来源：http://blog.fehbvm.com/Article/details/grtookrau.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.zdbjq.cn/Article/details/gclggqpuz.sHtML

[Q90] 生成序号列
来源：http://read.share.fehbvm.com/Article/details/gufcvymas.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.fehbvm.com/Article/details/gahvoyfqo.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gydzycywv.sHtML

R. Bash 专题
来源：http://baike.fehbvm.com/Article/details/glzfkltxy.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gcqnaclnk.sHtML

[R01] shebang 与严格模式
来源：http://baike.zdbjq.cn/Article/details/gjxdpzzod.sHtML

#!/usr/bin/env bash
来源：http://mobile.fehbvm.com/Article/details/gvsilkxsk.sHtML

set -euo pipefail
来源：http://mobile.fehbvm.com/Article/details/gkvkcuvwk.sHtML

[R02] 变量赋值与使用
来源：http://mobile.hesvh.cn/Article/details/gliqwherg.sHtML

name="Tom"; echo "$name"
来源：http://blog.zdbjq.cn/Article/details/gtnsyxhgi.sHtML

[R03] 只读变量
来源：http://read.share.fehbvm.com/Article/details/gswunaeit.sHtML

readonly PI=3.14
来源：http://m.share.fehbvm.com/Article/details/gqvdouygy.sHtML

[R04] 位置参数
来源：http://3g.fehbvm.com/Article/details/gqttxehaf.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.hesvh.cn/Article/details/gjxaxhudj.sHtML

[R05] 参数默认值
来源：http://mobile.hesvh.cn/Article/details/gahxagiip.sHtML

name="${1:-default}"
来源：http://mobile.fehbvm.com/Article/details/glkkswnzk.sHtML

[R06] 判断命令是否存在
来源：http://wap.fehbvm.com/Article/details/gpjyjtqeu.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.zdbjq.cn/Article/details/gbuokwaey.sHtML

[R07] if 判断文件
来源：http://m.share.zdbjq.cn/Article/details/gfvoontpc.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.zdbjq.cn/Article/details/glqcisisq.sHtML

[R08] 数值比较
来源：http://3g.zdbjq.cn/Article/details/gktlpncem.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.hesvh.cn/Article/details/grjckwjhc.sHtML

[R09] 字符串比较
来源：http://mobile.fehbvm.com/Article/details/gvlnoivlx.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.zdbjq.cn/Article/details/ghthacwkq.sHtML

[R10] 正则匹配
来源：http://www.blog.fehbvm.com/Article/details/gijrxrzzh.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.zdbjq.cn/Article/details/gwguviovh.sHtML

[R11] case 多分支
来源：http://baike.fehbvm.com/Article/details/gxoixacdb.sHtML

case "$1" in
来源：http://blog.zdbjq.cn/Article/details/ginuxncbx.sHtML

start) echo "启动" ;;
来源：http://blog.zdbjq.cn/Article/details/ggszuwbwa.sHtML

stop)  echo "停止" ;;
来源：http://baike.fehbvm.com/Article/details/ghpkgprcs.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.zdbjq.cn/Article/details/gaqigsnfy.sHtML

esac
来源：http://www.share.fehbvm.com/Article/details/glemxoqtp.sHtML

[R12] for 遍历文件
来源：http://blog.zdbjq.cn/Article/details/gbcmfpwdl.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.fehbvm.com/Article/details/gcifdqzzn.sHtML

[R13] for 计数循环
来源：http://wap.zdbjq.cn/Article/details/gwjvhkctb.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.hesvh.cn/Article/details/gebdwyqwo.sHtML

[R14] C 风格 for
来源：http://www.share.fehbvm.com/Article/details/ggdgjtppn.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.fehbvm.com/Article/details/gexdhpafv.sHtML

[R15] while 逐行读文件
来源：http://read.share.hesvh.cn/Article/details/grkxewfkn.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.zdbjq.cn/Article/details/givjxnpeh.sHtML

[R16] until 等待条件
来源：http://www.share.hesvh.cn/Article/details/gfnlglkzr.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.zdbjq.cn/Article/details/gufrbnaae.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.fehbvm.com/Article/details/gdczrndab.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.fehbvm.com/Article/details/gszdaodjy.sHtML

[R18] 遍历数组
来源：http://www.m.share.fehbvm.com/Article/details/gszsvbgll.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.zdbjq.cn/Article/details/gcpxjzdsm.sHtML

[R19] 数组长度
来源：http://m.share.zdbjq.cn/Article/details/gwljwizdf.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.hesvh.cn/Article/details/gfqyoduli.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.zdbjq.cn/Article/details/glhhjursi.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.zdbjq.cn/Article/details/gyvcrbghj.sHtML

[R21] 字符串长度
来源：http://m.share.hesvh.cn/Article/details/gwndeyumv.sHtML

echo "${#s}"
来源：http://baike.zdbjq.cn/Article/details/gvqbhsgzl.sHtML

[R22] 截取子串
来源：http://www.share.zdbjq.cn/Article/details/gwmkmxahr.sHtML

echo "${s:0:5}"
来源：http://www.m.share.zdbjq.cn/Article/details/glovdlesm.sHtML

[R23] 字符串替换
来源：http://wap.hesvh.cn/Article/details/gqmbyaljj.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.zdbjq.cn/Article/details/gdgcrxqqa.sHtML

[R24] 大小写转换
来源：http://wap.hesvh.cn/Article/details/glunijibb.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.hesvh.cn/Article/details/gujbmjtqu.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.fehbvm.com/Article/details/godklxkds.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.zdbjq.cn/Article/details/gnsfllxhu.sHtML

[R26] 命令替换
来源：http://read.share.zdbjq.cn/Article/details/gcszrerzn.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.hesvh.cn/Article/details/gjaybnpgf.sHtML

[R27] 算术展开
来源：http://www.m.share.hesvh.cn/Article/details/gdmhmqnzr.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.hesvh.cn/Article/details/gmlssryio.sHtML

[R28] 浮点运算
来源：http://3g.fehbvm.com/Article/details/gztlhwrxa.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.hesvh.cn/Article/details/gnnjoqkiw.sHtML

[R29] 定义函数
来源：http://blog.fehbvm.com/Article/details/gvkndtvcr.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.hesvh.cn/Article/details/gxznszlxf.sHtML

[R30] 函数返回状态码
来源：http://baike.fehbvm.com/Article/details/gxexqzpyt.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.hesvh.cn/Article/details/gnrbzqqbs.sHtML

[R31] 局部变量
来源：http://mobile.fehbvm.com/Article/details/gfmdujeke.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.hesvh.cn/Article/details/gzcsjtytj.sHtML

[R32] 参数个数校验
来源：http://mobile.hesvh.cn/Article/details/grsolnzxt.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.zdbjq.cn/Article/details/gabcmeazg.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.fehbvm.com/Article/details/gabbxzczo.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.fehbvm.com/Article/details/gldhgyiga.sHtML

[R34] 退出时清理
来源：http://mobile.zdbjq.cn/Article/details/gcogbkhkn.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.hesvh.cn/Article/details/gydogrrli.sHtML

[R35] 后台执行并等待
来源：http://baike.fehbvm.com/Article/details/gondjjlbf.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.fehbvm.com/Article/details/gsmeuvyqs.sHtML

[R36] 并发执行多个任务
来源：http://wap.fehbvm.com/Article/details/giouzqooz.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.hesvh.cn/Article/details/gsnwoyafa.sHtML

[R37] 把输出赋给变量
来源：http://mobile.fehbvm.com/Article/details/ghnmjyydq.sHtML

files=$(ls -1)
来源：http://blog.hesvh.cn/Article/details/gepyywvlg.sHtML

[R38] 管道串联
来源：http://www.blog.fehbvm.com/Article/details/gngfaioti.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.zdbjq.cn/Article/details/gpofywfao.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.fehbvm.com/Article/details/gzujvlqmi.sHtML

cmd > out.log 2>&1
来源：http://www.blog.zdbjq.cn/Article/details/gjygyjbsf.sHtML

[R40] 追加写日志
来源：http://www.share.zdbjq.cn/Article/details/gmtyllodq.sHtML

echo "log" >> out.log
来源：http://www.share.zdbjq.cn/Article/details/gwsjbiwwf.sHtML

[R41] 丢弃输出
来源：http://read.share.fehbvm.com/Article/details/gcxpnaoeg.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.hesvh.cn/Article/details/gxvtscwwp.sHtML

[R42] 输入重定向
来源：http://m.share.fehbvm.com/Article/details/gugzngajk.sHtML

wc -l < a.txt
来源：http://wap.fehbvm.com/Article/details/gmbpekrbe.sHtML

[R43] 按名字查找文件
来源：http://m.share.fehbvm.com/Article/details/gjsvvmtiq.sHtML

find . -name "*.log" -type f
来源：http://mobile.fehbvm.com/Article/details/gnjashfld.sHtML

[R44] 按修改时间查找
来源：http://read.share.fehbvm.com/Article/details/gxuldedbx.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.hesvh.cn/Article/details/gpiobkecm.sHtML

[R45] 批量删除
来源：http://blog.hesvh.cn/Article/details/gpbgboqps.sHtML

find . -name "*.tmp" -delete
来源：http://baike.zdbjq.cn/Article/details/gwcfkrfsj.sHtML

[R46] 递归替换文件内容
来源：http://www.share.hesvh.cn/Article/details/gkysdkktu.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.hesvh.cn/Article/details/gdchifhhe.sHtML

[R47] sed 单行替换
来源：http://blog.fehbvm.com/Article/details/gfwonqthb.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.fehbvm.com/Article/details/glruyjglp.sHtML

[R48] awk 取指定列
来源：http://m.share.hesvh.cn/Article/details/gqrjvrszb.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.zdbjq.cn/Article/details/gxqhnnaje.sHtML

[R49] awk 带条件
来源：http://www.share.fehbvm.com/Article/details/gmyuglixw.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.hesvh.cn/Article/details/gdhoupbzz.sHtML

[R50] awk 求和
来源：http://mobile.hesvh.cn/Article/details/gpfyrgoji.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.fehbvm.com/Article/details/gsgmlatnk.sHtML

[R51] 排序去重取前几
来源：http://3g.zdbjq.cn/Article/details/gykowhlhx.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.hesvh.cn/Article/details/glzzykbbd.sHtML

[R52] 统计行数
来源：http://blog.hesvh.cn/Article/details/gregubeca.sHtML

wc -l a.txt
来源：http://m.share.hesvh.cn/Article/details/gudhcyaen.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.hesvh.cn/Article/details/gzcxvorpm.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.hesvh.cn/Article/details/gvqmsftef.sHtML

[R54] 比较两个文件
来源：http://www.blog.zdbjq.cn/Article/details/gxsyomury.sHtML

diff a.txt b.txt
来源：http://mobile.fehbvm.com/Article/details/gdjfscrbo.sHtML

[R55] 压缩与解压
来源：http://read.share.fehbvm.com/Article/details/gcogpwqcq.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.hesvh.cn/Article/details/gzydlgnhi.sHtML

[R56] 远程拷贝
来源：http://www.blog.zdbjq.cn/Article/details/gbxhxlvyt.sHtML

scp file user@host:/path/
来源：http://baike.fehbvm.com/Article/details/gqvqoaszm.sHtML

[R57] 远程执行命令
来源：http://www.m.share.zdbjq.cn/Article/details/gkmzmcrpg.sHtML

ssh user@host 'uptime'
来源：http://baike.fehbvm.com/Article/details/gojfozlkw.sHtML

[R58] 下载文件
来源：http://wap.hesvh.cn/Article/details/goavtdpch.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.zdbjq.cn/Article/details/godalfwru.sHtML

[R59] 发 POST JSON
来源：http://blog.hesvh.cn/Article/details/gwkiuexdp.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.fehbvm.com/Article/details/gfimrrvsu.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.fehbvm.com/Article/details/gqsvwivat.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.zdbjq.cn/Article/details/ggnldzyaz.sHtML

[R61] 磁盘占用
来源：http://3g.hesvh.cn/Article/details/gaszdhybh.sHtML

df -h;  du -sh *
来源：http://www.m.share.fehbvm.com/Article/details/ghrsgxxbg.sHtML

[R62] 找最占空间的文件
来源：http://mobile.hesvh.cn/Article/details/gakjfmpvd.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.hesvh.cn/Article/details/gyhzsjbjk.sHtML

[R63] 内存与进程
来源：http://www.share.zdbjq.cn/Article/details/gnkzqjufc.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.fehbvm.com/Article/details/gehsmjtir.sHtML

[R64] 结束进程
来源：http://3g.zdbjq.cn/Article/details/ghpgnfysg.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.hesvh.cn/Article/details/gvuaeikkk.sHtML

[R65] 查看端口占用
来源：http://wap.hesvh.cn/Article/details/gcbyqxawq.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.zdbjq.cn/Article/details/gqgnewoom.sHtML

[R66] 定时任务
来源：http://3g.fehbvm.com/Article/details/gchrbvgla.sHtML

crontab -e;  crontab -l
来源：http://m.share.zdbjq.cn/Article/details/gllelxpoj.sHtML

[R67] 生成随机十六进制串
来源：http://blog.hesvh.cn/Article/details/ghukpwqbg.sHtML

openssl rand -hex 16
来源：http://baike.fehbvm.com/Article/details/gtajxbpej.sHtML

[R68] 计算文件校验值
来源：http://mobile.hesvh.cn/Article/details/geufshiso.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.hesvh.cn/Article/details/gfuyewvha.sHtML

[R69] 生成随机密码
来源：http://3g.zdbjq.cn/Article/details/ggizcojzd.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.fehbvm.com/Article/details/gwydepezc.sHtML

[R70] 时间戳与互转
来源：http://m.share.fehbvm.com/Article/details/gwmwlmxfd.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.hesvh.cn/Article/details/gdiexksvf.sHtML

[R71] 日期格式化
来源：http://3g.hesvh.cn/Article/details/gnmseoftu.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.hesvh.cn/Article/details/gezhujwlt.sHtML

[R72] 等待端口就绪
来源：http://m.share.zdbjq.cn/Article/details/gaqaltvxy.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.fehbvm.com/Article/details/gwgaqplgv.sHtML

[R73] 分割大日志
来源：http://read.share.fehbvm.com/Article/details/gnnorahrh.sHtML

split -l 1000 big.log part_
来源：http://www.share.hesvh.cn/Article/details/gkzsbalcw.sHtML

[R74] 批量重命名
来源：http://m.share.zdbjq.cn/Article/details/gmfwiyycq.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.hesvh.cn/Article/details/ghmbgftgu.sHtML

[R75] 导出环境变量
来源：http://mobile.hesvh.cn/Article/details/gsenyyotf.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.hesvh.cn/Article/details/goaamyysn.sHtML

[R76] 使用临时文件
来源：http://read.share.zdbjq.cn/Article/details/grqqpjaeo.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fehbvm.com/Article/details/grahnnlzk.sHtML

[R77] 读取用户输入
来源：http://baike.zdbjq.cn/Article/details/gvlxrfqcu.sHtML

read -rp "请输入: " ans
来源：http://3g.hesvh.cn/Article/details/gmpubhrkf.sHtML

[R78] 交互式菜单
来源：http://www.share.fehbvm.com/Article/details/ggxnklwtf.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.hesvh.cn/Article/details/gjancownh.sHtML

[R79] 解析命令行选项
来源：http://www.blog.zdbjq.cn/Article/details/ggwgjoadm.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.fehbvm.com/Article/details/gqbchgrjr.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.zdbjq.cn/Article/details/gnqsuavxu.sHtML

time ./run.sh
来源：http://blog.fehbvm.com/Article/details/gckqhzcum.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gztwtajkk.sHtML

S. C / C++ 专题
来源：http://wap.zdbjq.cn/Article/details/gndmmduse.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gwwpmtrys.sHtML

[S01] C：Hello World
来源：http://mobile.hesvh.cn/Article/details/ggvtznvsw.sHtML

#include <stdio.h>
来源：http://mobile.zdbjq.cn/Article/details/gmmyrynhk.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.hesvh.cn/Article/details/gzufrdcdr.sHtML

[S02] C：变量与格式化输出
来源：http://blog.zdbjq.cn/Article/details/gdaaxxusi.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.zdbjq.cn/Article/details/gkesdxpyb.sHtML

[S03] C：读入整数
来源：http://3g.zdbjq.cn/Article/details/ggocicnnv.sHtML

int x; scanf("%d", &x);
来源：http://www.share.fehbvm.com/Article/details/gzrizjxmb.sHtML

[S04] C：字符串复制
来源：http://read.share.hesvh.cn/Article/details/guqiclfbg.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.fehbvm.com/Article/details/gtmnofcez.sHtML

[S05] C：字符串长度
来源：http://mobile.fehbvm.com/Article/details/gwxvojfac.sHtML

strlen(s)
来源：http://baike.zdbjq.cn/Article/details/gdcuxepqy.sHtML

[S06] C：字符串比较
来源：http://3g.hesvh.cn/Article/details/gqckjexcs.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.zdbjq.cn/Article/details/gdbxuiphh.sHtML

[S07] C：数组遍历求和
来源：http://m.share.fehbvm.com/Article/details/gkcholiqd.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.zdbjq.cn/Article/details/gkxyifshx.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.fehbvm.com/Article/details/gtiewjdsl.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.zdbjq.cn/Article/details/glbaeohez.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.fehbvm.com/Article/details/gpbdoxtgn.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.fehbvm.com/Article/details/grmlzwcwk.sHtML

[S10] C：指针与解引用
来源：http://blog.hesvh.cn/Article/details/globtznly.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.zdbjq.cn/Article/details/giwawzvum.sHtML

[S11] C：逐行读文件
来源：http://read.share.zdbjq.cn/Article/details/gejvwsdil.sHtML


<!-- 参考信息 -->