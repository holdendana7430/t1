代发 wailian999

[Q44] IN 子查询
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grxxdzvkg.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://baike.fanxiaobao.xyz/Article/details/gowepvaxt.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghuarmpqg.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.fanxiaobao.xyz/Article/details/gapjkgkwp.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.fanxiaobao.xyz/Article/details/gmzhqnmld.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.fanxiaobao.xyz/Article/details/ghoicfnip.sHtML

[Q47] 与平均值比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gulrqvrim.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://baike.fanxiaobao.xyz/Article/details/gsguwqaau.sHtML

[Q48] CTE 公用表表达式
来源：http://wap.fanxiaobao.xyz/Article/details/gsgdmnorn.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gefulxxig.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://baike.fanxiaobao.xyz/Article/details/gpaonuefg.sHtML

[Q49] 更新单行
来源：http://m.share.fanxiaobao.xyz/Article/details/gqaymajje.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mobile.fanxiaobao.xyz/Article/details/gmhorzmbd.sHtML

[Q50] 批量更新
来源：http://baike.fanxiaobao.xyz/Article/details/gtdmopyyv.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.fanxiaobao.xyz/Article/details/gcjgdmcwt.sHtML

[Q51] 用子查询更新
来源：http://baike.fanxiaobao.xyz/Article/details/ghufphngb.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/gwsgpsnmz.sHtML

[Q52] 删除指定行
来源：http://read.share.fanxiaobao.xyz/Article/details/grxgdepmt.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbcqkxxaq.sHtML

[Q53] 按条件删除
来源：http://mobile.fanxiaobao.xyz/Article/details/gvlkfzrsy.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.fanxiaobao.xyz/Article/details/gdhhiageg.sHtML

[Q54] 清空表
来源：http://www.share.fanxiaobao.xyz/Article/details/gjhufcinx.sHtML

TRUNCATE TABLE logs;
来源：http://mobile.fanxiaobao.xyz/Article/details/gvsyyoxgr.sHtML

[Q55] 排名（并列占位）
来源：http://m.share.fanxiaobao.xyz/Article/details/gnuwdwomi.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mobile.fanxiaobao.xyz/Article/details/ggsvrhqyz.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.fanxiaobao.xyz/Article/details/ggiuctcpt.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwoxetjef.sHtML

[Q57] 行号
来源：http://www.share.fanxiaobao.xyz/Article/details/ggqqnhyyp.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/guctlnwxl.sHtML

[Q58] 累计求和
来源：http://read.share.fanxiaobao.xyz/Article/details/gncpasmym.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/gtfnayqyz.sHtML

[Q59] 分组内累计
来源：http://baike.fanxiaobao.xyz/Article/details/gqemzzsnx.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/gfraskhzc.sHtML

[Q60] 取上一行 / 下一行
来源：http://read.share.fanxiaobao.xyz/Article/details/gemxsvhuz.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.fanxiaobao.xyz/Article/details/gfllhictm.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqnlidypw.sHtML

[Q61] 移动平均
来源：http://m.share.fanxiaobao.xyz/Article/details/gqagzyivw.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://3g.fanxiaobao.xyz/Article/details/ggaaadcll.sHtML

[Q62] 分组占比
来源：http://baike.fanxiaobao.xyz/Article/details/gsxgbzmkl.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmmjwjfsh.sHtML

[Q63] 开启事务
来源：http://www.share.fanxiaobao.xyz/Article/details/gkffkyygp.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.share.fanxiaobao.xyz/Article/details/ginmornaj.sHtML

[Q64] 提交事务
来源：http://mobile.fanxiaobao.xyz/Article/details/goutizpml.sHtML

COMMIT;
来源：http://www.share.fanxiaobao.xyz/Article/details/gscvqbjba.sHtML

[Q65] 回滚事务
来源：http://www.share.fanxiaobao.xyz/Article/details/gyqjbbgrk.sHtML

ROLLBACK;
来源：http://read.share.fanxiaobao.xyz/Article/details/gmwcjmxqw.sHtML

[Q66] 行锁查询
来源：http://m.share.fanxiaobao.xyz/Article/details/gpiwmvhed.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.fanxiaobao.xyz/Article/details/gwkubpmke.sHtML

[Q67] 设置隔离级别
来源：http://www.share.fanxiaobao.xyz/Article/details/ggsrgqkvo.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.fanxiaobao.xyz/Article/details/ggmbpizwk.sHtML

[Q68] 保存点
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gziudvhsf.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxekirchg.sHtML

ROLLBACK TO sp1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gnrcjpdap.sHtML

[Q69] 查看执行计划
来源：http://m.share.fanxiaobao.xyz/Article/details/grahxpvvq.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.share.fanxiaobao.xyz/Article/details/gruckuifb.sHtML

[Q70] 更新统计信息
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpmxsdzhk.sHtML

ANALYZE TABLE users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gtydnpzym.sHtML

[Q71] 查看建表语句
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghhxllzeb.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://blog.fanxiaobao.xyz/Article/details/gwwcguxlf.sHtML

[Q72] 查看索引
来源：http://www.share.fanxiaobao.xyz/Article/details/gdrlrmobe.sHtML

SHOW INDEX FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gkvrphghi.sHtML

[Q73] 查看表状态
来源：http://3g.fanxiaobao.xyz/Article/details/gklhzokhr.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.fanxiaobao.xyz/Article/details/gpewutmov.sHtML

[Q74] 强制使用索引
来源：http://m.share.fanxiaobao.xyz/Article/details/gemvzxfzv.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwxnuijry.sHtML

[Q75] 日期格式化
来源：http://blog.fanxiaobao.xyz/Article/details/glqukcoxz.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gykaknqns.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.fanxiaobao.xyz/Article/details/gkexfcwnh.sHtML

[Q76] 按天统计
来源：http://mobile.fanxiaobao.xyz/Article/details/gqigbluxx.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.fanxiaobao.xyz/Article/details/grmflyceg.sHtML

[Q77] 时间加减
来源：http://baike.fanxiaobao.xyz/Article/details/gayxoxkjf.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guvzusyvn.sHtML

[Q78] 当前时间
来源：http://blog.fanxiaobao.xyz/Article/details/gyxegnnnz.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzuqluiiz.sHtML

[Q79] 字符串拼接
来源：http://wap.fanxiaobao.xyz/Article/details/giapmqcvm.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.fanxiaobao.xyz/Article/details/giuyzecde.sHtML

[Q80] 字符串截取
来源：http://m.share.fanxiaobao.xyz/Article/details/gsisvzhwq.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gtkvubhar.sHtML

[Q81] 字符串替换
来源：http://blog.fanxiaobao.xyz/Article/details/gyqqoqwjl.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gypfdbztk.sHtML

[Q82] 字符长度与字节长度
来源：http://mobile.fanxiaobao.xyz/Article/details/gtkqjmavk.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gwlitfgpv.sHtML

[Q83] 大小写转换
来源：http://blog.fanxiaobao.xyz/Article/details/gunhatjyn.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gzhrzgohi.sHtML

[Q84] 去除首尾空格
来源：http://m.share.fanxiaobao.xyz/Article/details/geauxvygn.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/guxjjmwut.sHtML

[Q85] 数值取整
来源：http://m.share.fanxiaobao.xyz/Article/details/gxvzbrabe.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.fanxiaobao.xyz/Article/details/geqdlkigz.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.fanxiaobao.xyz/Article/details/golbvfsif.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.fanxiaobao.xyz/Article/details/gmovddbky.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnwkikgaa.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://baike.fanxiaobao.xyz/Article/details/gdjxrusmn.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.fanxiaobao.xyz/Article/details/grykyspep.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.fanxiaobao.xyz/Article/details/gzwjsukmr.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqgetsgrb.sHtML

[Q89] 判断表是否存在
来源：http://wap.fanxiaobao.xyz/Article/details/grqgkhgdt.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.fanxiaobao.xyz/Article/details/gbafmcafy.sHtML

[Q90] 生成序号列
来源：http://3g.fanxiaobao.xyz/Article/details/gymcxmkcf.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.fanxiaobao.xyz/Article/details/gvyicveny.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gbzypqmdy.sHtML

R. Bash 专题
来源：http://read.share.fanxiaobao.xyz/Article/details/gdnbsurlk.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gavehqopz.sHtML

[R01] shebang 与严格模式
来源：http://baike.fanxiaobao.xyz/Article/details/gcjqimrij.sHtML

#!/usr/bin/env bash
来源：http://blog.fanxiaobao.xyz/Article/details/gzczpufnk.sHtML

set -euo pipefail
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxadktmls.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpqllykff.sHtML

name="Tom"; echo "$name"
来源：http://wap.fanxiaobao.xyz/Article/details/gxculqqne.sHtML

[R03] 只读变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gtemxdkvt.sHtML

readonly PI=3.14
来源：http://baike.fanxiaobao.xyz/Article/details/gkvuppbls.sHtML

[R04] 位置参数
来源：http://baike.fanxiaobao.xyz/Article/details/geizoiivb.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.fanxiaobao.xyz/Article/details/gcbmapasr.sHtML

[R05] 参数默认值
来源：http://mobile.fanxiaobao.xyz/Article/details/gnsifykhm.sHtML

name="${1:-default}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/grntescza.sHtML

[R06] 判断命令是否存在
来源：http://mobile.fanxiaobao.xyz/Article/details/gonerobjh.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.fanxiaobao.xyz/Article/details/gutxnxvyb.sHtML

[R07] if 判断文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/galqxzqdp.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnyvuynim.sHtML

[R08] 数值比较
来源：http://baike.fanxiaobao.xyz/Article/details/ggnkenlqj.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.fanxiaobao.xyz/Article/details/gxynnkdyi.sHtML

[R09] 字符串比较
来源：http://blog.fanxiaobao.xyz/Article/details/ghbesuohq.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.fanxiaobao.xyz/Article/details/gpzinqdce.sHtML

[R10] 正则匹配
来源：http://blog.fanxiaobao.xyz/Article/details/gsmhirltf.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/gjzdblclp.sHtML

[R11] case 多分支
来源：http://www.share.fanxiaobao.xyz/Article/details/gwoxmwuxm.sHtML

case "$1" in
来源：http://www.blog.fanxiaobao.xyz/Article/details/geiiauqsy.sHtML

start) echo "启动" ;;
来源：http://mobile.fanxiaobao.xyz/Article/details/gbsrztilw.sHtML

stop)  echo "停止" ;;
来源：http://blog.fanxiaobao.xyz/Article/details/gumatfpjj.sHtML

*)     echo "未知命令" ;;
来源：http://wap.fanxiaobao.xyz/Article/details/govzkdlgm.sHtML

esac
来源：http://www.share.fanxiaobao.xyz/Article/details/gwgjhllaq.sHtML

[R12] for 遍历文件
来源：http://baike.fanxiaobao.xyz/Article/details/gkobbcioa.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gfeyfjzna.sHtML

[R13] for 计数循环
来源：http://blog.fanxiaobao.xyz/Article/details/gncojmudx.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gxwojvdnx.sHtML

[R14] C 风格 for
来源：http://baike.fanxiaobao.xyz/Article/details/ggteylwkh.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gxoybeaea.sHtML

[R15] while 逐行读文件
来源：http://wap.fanxiaobao.xyz/Article/details/gyjbjvubw.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gukoxyyyr.sHtML

[R16] until 等待条件
来源：http://mobile.fanxiaobao.xyz/Article/details/gwrcvyvtl.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gmpljdcwe.sHtML

[R17] 数组定义与取值
来源：http://read.share.fanxiaobao.xyz/Article/details/gpgtnzuom.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.fanxiaobao.xyz/Article/details/ggmnpixvk.sHtML

[R18] 遍历数组
来源：http://mobile.fanxiaobao.xyz/Article/details/gspxrcequ.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gfnmnywzc.sHtML

[R19] 数组长度
来源：http://3g.fanxiaobao.xyz/Article/details/gdccrnddq.sHtML

echo "${#arr[@]}"
来源：http://3g.fanxiaobao.xyz/Article/details/gjmcflzgo.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guoswujob.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gcymcdjdh.sHtML

[R21] 字符串长度
来源：http://mobile.fanxiaobao.xyz/Article/details/gssjmcbyx.sHtML

echo "${#s}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gksdagice.sHtML

[R22] 截取子串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmdagmzau.sHtML

echo "${s:0:5}"
来源：http://3g.fanxiaobao.xyz/Article/details/gmgkopmsh.sHtML

[R23] 字符串替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gxekryebo.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.fanxiaobao.xyz/Article/details/gxtmzumbr.sHtML

[R24] 大小写转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guxblwjxo.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gzzdreayv.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.fanxiaobao.xyz/Article/details/gprnukpkz.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gufqacxkt.sHtML

[R26] 命令替换
来源：http://m.share.fanxiaobao.xyz/Article/details/glkzhhxpw.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.fanxiaobao.xyz/Article/details/gpemsfwzi.sHtML

[R27] 算术展开
来源：http://3g.fanxiaobao.xyz/Article/details/gvkhxihct.sHtML

echo $((1 + 2 * 3))
来源：http://blog.fanxiaobao.xyz/Article/details/gobdfytqo.sHtML

[R28] 浮点运算
来源：http://3g.fanxiaobao.xyz/Article/details/gjwhppqat.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.fanxiaobao.xyz/Article/details/ghnjdsvow.sHtML

[R29] 定义函数
来源：http://blog.fanxiaobao.xyz/Article/details/grnlhjobj.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gsphvhkim.sHtML

[R30] 函数返回状态码
来源：http://read.share.fanxiaobao.xyz/Article/details/gxjefxnrl.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.fanxiaobao.xyz/Article/details/gzosarudn.sHtML

[R31] 局部变量
来源：http://mobile.fanxiaobao.xyz/Article/details/goohbcuto.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbugcohhh.sHtML

[R32] 参数个数校验
来源：http://read.share.fanxiaobao.xyz/Article/details/gdarvnjhl.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.fanxiaobao.xyz/Article/details/goyrlrgzg.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.fanxiaobao.xyz/Article/details/gotrnxlyu.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.fanxiaobao.xyz/Article/details/gssjcmpka.sHtML

[R34] 退出时清理
来源：http://baike.fanxiaobao.xyz/Article/details/grgjjojdo.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.fanxiaobao.xyz/Article/details/guplrtenh.sHtML

[R35] 后台执行并等待
来源：http://m.share.fanxiaobao.xyz/Article/details/gatdgjbdx.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.fanxiaobao.xyz/Article/details/gyleedvap.sHtML

[R36] 并发执行多个任务
来源：http://blog.fanxiaobao.xyz/Article/details/gopoydzhx.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.fanxiaobao.xyz/Article/details/ghpbngetc.sHtML

[R37] 把输出赋给变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gmtutadaz.sHtML

files=$(ls -1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gsimrdeqd.sHtML

[R38] 管道串联
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqchgmtlv.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvybwbiso.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.fanxiaobao.xyz/Article/details/gtititlhs.sHtML

cmd > out.log 2>&1
来源：http://mobile.fanxiaobao.xyz/Article/details/ghmgsjhgd.sHtML

[R40] 追加写日志
来源：http://wap.fanxiaobao.xyz/Article/details/gpqehrrcq.sHtML

echo "log" >> out.log
来源：http://baike.fanxiaobao.xyz/Article/details/gqbetfxwz.sHtML

[R41] 丢弃输出
来源：http://www.share.fanxiaobao.xyz/Article/details/galkoarcc.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpofevkma.sHtML

[R42] 输入重定向
来源：http://www.share.fanxiaobao.xyz/Article/details/gmepwtxfh.sHtML

wc -l < a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gqnrhehpt.sHtML

[R43] 按名字查找文件
来源：http://m.share.fanxiaobao.xyz/Article/details/giffcatbf.sHtML

find . -name "*.log" -type f
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmfzksljk.sHtML

[R44] 按修改时间查找
来源：http://m.share.fanxiaobao.xyz/Article/details/gyzitjtaw.sHtML

find . -mtime -7 -type f
来源：http://read.share.fanxiaobao.xyz/Article/details/gpwysilkq.sHtML

[R45] 批量删除
来源：http://wap.fanxiaobao.xyz/Article/details/gewhczmbc.sHtML

find . -name "*.tmp" -delete
来源：http://blog.fanxiaobao.xyz/Article/details/gscmsjjjw.sHtML

[R46] 递归替换文件内容
来源：http://3g.fanxiaobao.xyz/Article/details/gmxhjvbfn.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.fanxiaobao.xyz/Article/details/glcvnfdsz.sHtML

[R47] sed 单行替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gfmjqvdbv.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gprnzfbel.sHtML

[R48] awk 取指定列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcyxksyjx.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gjznhnslu.sHtML

[R49] awk 带条件
来源：http://3g.fanxiaobao.xyz/Article/details/gyzbhibjm.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.fanxiaobao.xyz/Article/details/gweycfdam.sHtML

[R50] awk 求和
来源：http://baike.fanxiaobao.xyz/Article/details/ghwgsoqtl.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpeaxfrum.sHtML

[R51] 排序去重取前几
来源：http://mobile.fanxiaobao.xyz/Article/details/gsuhuogrv.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.fanxiaobao.xyz/Article/details/gwnllrkgm.sHtML

[R52] 统计行数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggslrhcik.sHtML

wc -l a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gecnkmohj.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.fanxiaobao.xyz/Article/details/gdqagqmvr.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.fanxiaobao.xyz/Article/details/gddqqigsx.sHtML

[R54] 比较两个文件
来源：http://baike.fanxiaobao.xyz/Article/details/gmtltxtwq.sHtML

diff a.txt b.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gorwouegk.sHtML

[R55] 压缩与解压
来源：http://www.share.fanxiaobao.xyz/Article/details/gmlczzxha.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.fanxiaobao.xyz/Article/details/gyoxrobvu.sHtML

[R56] 远程拷贝
来源：http://wap.fanxiaobao.xyz/Article/details/gtdezbmxn.sHtML

scp file user@host:/path/
来源：http://3g.fanxiaobao.xyz/Article/details/gdrhymdcm.sHtML

[R57] 远程执行命令
来源：http://baike.fanxiaobao.xyz/Article/details/gpakqyimr.sHtML

ssh user@host 'uptime'
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwatboifo.sHtML

[R58] 下载文件
来源：http://blog.fanxiaobao.xyz/Article/details/gdstwlklk.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.fanxiaobao.xyz/Article/details/gfskyrfas.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfbwzksek.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxvdyaapz.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.fanxiaobao.xyz/Article/details/gzhsdqkon.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.fanxiaobao.xyz/Article/details/gfrznohxm.sHtML

[R61] 磁盘占用
来源：http://www.share.fanxiaobao.xyz/Article/details/gwqgepgef.sHtML

df -h;  du -sh *
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdoirzoki.sHtML

[R62] 找最占空间的文件
来源：http://wap.fanxiaobao.xyz/Article/details/ggknrtwcx.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghqamyqnr.sHtML

[R63] 内存与进程
来源：http://wap.fanxiaobao.xyz/Article/details/gwrbswrly.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.fanxiaobao.xyz/Article/details/grvzzkwka.sHtML

[R64] 结束进程
来源：http://m.share.fanxiaobao.xyz/Article/details/ghhypkdyp.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.fanxiaobao.xyz/Article/details/gxrjqmvqs.sHtML

[R65] 查看端口占用
来源：http://wap.fanxiaobao.xyz/Article/details/gslhyeqbj.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwnromrbi.sHtML

[R66] 定时任务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxnekueuc.sHtML

crontab -e;  crontab -l
来源：http://www.share.fanxiaobao.xyz/Article/details/gtrdhchrc.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.fanxiaobao.xyz/Article/details/gvlbxbcut.sHtML

openssl rand -hex 16
来源：http://baike.fanxiaobao.xyz/Article/details/girxnyemx.sHtML

[R68] 计算文件校验值
来源：http://mobile.fanxiaobao.xyz/Article/details/gehiloccp.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gtaxlhhwj.sHtML

[R69] 生成随机密码
来源：http://3g.fanxiaobao.xyz/Article/details/gpnpuzljt.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.fanxiaobao.xyz/Article/details/gpwsoflrg.sHtML

[R70] 时间戳与互转
来源：http://blog.fanxiaobao.xyz/Article/details/gdvraalzd.sHtML

date +%s;  date -d @1700000000
来源：http://blog.fanxiaobao.xyz/Article/details/gvppkamgs.sHtML

[R71] 日期格式化
来源：http://read.share.fanxiaobao.xyz/Article/details/glashazxv.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvwgtmhkl.sHtML

[R72] 等待端口就绪
来源：http://www.share.fanxiaobao.xyz/Article/details/gunyyhgza.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.fanxiaobao.xyz/Article/details/gmwerhizv.sHtML

[R73] 分割大日志
来源：http://www.share.fanxiaobao.xyz/Article/details/gvpdnphbg.sHtML

split -l 1000 big.log part_
来源：http://baike.fanxiaobao.xyz/Article/details/grbrjfvvm.sHtML

[R74] 批量重命名
来源：http://wap.fanxiaobao.xyz/Article/details/grlmayxtm.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/glrzzsuii.sHtML

[R75] 导出环境变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwaugyqql.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.fanxiaobao.xyz/Article/details/gdswevucx.sHtML

[R76] 使用临时文件
来源：http://blog.fanxiaobao.xyz/Article/details/gwoqluxcw.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyuvhxfcv.sHtML

[R77] 读取用户输入
来源：http://read.share.fanxiaobao.xyz/Article/details/gcbnrwzfr.sHtML

read -rp "请输入: " ans
来源：http://mobile.fanxiaobao.xyz/Article/details/gicyjzqiw.sHtML

[R78] 交互式菜单
来源：http://www.share.fanxiaobao.xyz/Article/details/gfiuxwcrj.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.fanxiaobao.xyz/Article/details/gbsuljwqf.sHtML

[R79] 解析命令行选项
来源：http://blog.fanxiaobao.xyz/Article/details/gzpklxhzd.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gebkazdcw.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.fanxiaobao.xyz/Article/details/ggfpyqmdp.sHtML

time ./run.sh
来源：http://3g.fanxiaobao.xyz/Article/details/gutszlamo.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gkfowmnfg.sHtML

S. C / C++ 专题
来源：http://wap.fanxiaobao.xyz/Article/details/glfehaetc.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gxkwcpnia.sHtML

[S01] C：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/guevqkqpq.sHtML

#include <stdio.h>
来源：http://m.share.fanxiaobao.xyz/Article/details/gxjnhtcnk.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.fanxiaobao.xyz/Article/details/grtkdrixo.sHtML

[S02] C：变量与格式化输出
来源：http://wap.fanxiaobao.xyz/Article/details/gbrefiget.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.fanxiaobao.xyz/Article/details/gsiexxqse.sHtML

[S03] C：读入整数
来源：http://baike.fanxiaobao.xyz/Article/details/glfjhxpzk.sHtML

int x; scanf("%d", &x);
来源：http://3g.fanxiaobao.xyz/Article/details/gebbygofj.sHtML

[S04] C：字符串复制
来源：http://3g.fanxiaobao.xyz/Article/details/gbvfcduwv.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.fanxiaobao.xyz/Article/details/gmndxdhon.sHtML

[S05] C：字符串长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gjnbyyogg.sHtML

strlen(s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gksjfqqip.sHtML

[S06] C：字符串比较
来源：http://3g.fanxiaobao.xyz/Article/details/gdwwhjfnf.sHtML

strcmp(a, b) == 0
来源：http://baike.fanxiaobao.xyz/Article/details/gwfsuebka.sHtML

[S07] C：数组遍历求和
来源：http://mobile.fanxiaobao.xyz/Article/details/gxjejuskh.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.fanxiaobao.xyz/Article/details/gssqsjmym.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.fanxiaobao.xyz/Article/details/gjdherkbp.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzqacvukm.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.fanxiaobao.xyz/Article/details/gfxnbcdaz.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjxgwwcni.sHtML

[S10] C：指针与解引用
来源：http://3g.fanxiaobao.xyz/Article/details/ggbzwmamp.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.fanxiaobao.xyz/Article/details/gszsfosjb.sHtML

[S11] C：逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gkqmsikwz.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.fanxiaobao.xyz/Article/details/gggbrzlgc.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggxzijfgf.sHtML

fclose(f);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grzovjtyv.sHtML

[S12] C：写文件
来源：http://m.share.fanxiaobao.xyz/Article/details/grgtbstrr.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.fanxiaobao.xyz/Article/details/gtzuweots.sHtML

[S13] C：宏定义
来源：http://blog.fanxiaobao.xyz/Article/details/ghrebhrte.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.fanxiaobao.xyz/Article/details/gkjkpyohw.sHtML

[S14] C：枚举
来源：http://baike.fanxiaobao.xyz/Article/details/gdwyahioa.sHtML


<!-- 参考信息 -->