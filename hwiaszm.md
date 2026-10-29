代发 wailian999

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.fehbvm.com/Article/details/gtjcmeutu.sHtML

JOIN users u ON u.id = o.user_id
来源：http://mobile.zdbjq.cn/Article/details/gpjwjrigq.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://read.share.hesvh.cn/Article/details/gtyxsarzr.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.hesvh.cn/Article/details/gyqusycnt.sHtML

SELECT u.name, o.amount FROM users u
来源：http://m.share.fehbvm.com/Article/details/gicasyxok.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.fehbvm.com/Article/details/guwxzcbeu.sHtML

[Q43] 标量子查询
来源：http://www.blog.hesvh.cn/Article/details/gnuvrzknz.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.share.hesvh.cn/Article/details/gzgjvcmxh.sHtML

[Q44] IN 子查询
来源：http://www.m.share.zdbjq.cn/Article/details/grxhnbtdj.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.blog.hesvh.cn/Article/details/gauqsuzaa.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.zdbjq.cn/Article/details/gmsykmptc.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.fehbvm.com/Article/details/gjwhzfmum.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.hesvh.cn/Article/details/gchrlgdlm.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.hesvh.cn/Article/details/gxijuqnnp.sHtML

[Q47] 与平均值比较
来源：http://3g.hesvh.cn/Article/details/gkrciltpt.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.fehbvm.com/Article/details/gocqgyvmb.sHtML

[Q48] CTE 公用表表达式
来源：http://baike.zdbjq.cn/Article/details/gpnwsgyda.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.fehbvm.com/Article/details/ggoqhfctl.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://read.share.zdbjq.cn/Article/details/gdocfsyhe.sHtML

[Q49] 更新单行
来源：http://www.share.zdbjq.cn/Article/details/gmbhqlylb.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.blog.zdbjq.cn/Article/details/gpzmsohyh.sHtML

[Q50] 批量更新
来源：http://mobile.fehbvm.com/Article/details/gshduiodk.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.m.share.fehbvm.com/Article/details/ggsndhvov.sHtML

[Q51] 用子查询更新
来源：http://m.share.fehbvm.com/Article/details/gkkpjcfwa.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.blog.zdbjq.cn/Article/details/gmikkcksv.sHtML

[Q52] 删除指定行
来源：http://www.m.share.hesvh.cn/Article/details/gudfnpqmz.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.zdbjq.cn/Article/details/gazzssyuu.sHtML

[Q53] 按条件删除
来源：http://wap.fehbvm.com/Article/details/girnnrtrw.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.blog.hesvh.cn/Article/details/gpqifgowk.sHtML

[Q54] 清空表
来源：http://3g.zdbjq.cn/Article/details/goziumpna.sHtML

TRUNCATE TABLE logs;
来源：http://www.m.share.zdbjq.cn/Article/details/glrvqevvf.sHtML

[Q55] 排名（并列占位）
来源：http://3g.zdbjq.cn/Article/details/gcqzmohug.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://blog.fehbvm.com/Article/details/gxjmakqrf.sHtML

[Q56] 密集排名（并列不占位）
来源：http://3g.hesvh.cn/Article/details/ghzgoprzq.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.zdbjq.cn/Article/details/gvqhjhcwi.sHtML

[Q57] 行号
来源：http://mobile.zdbjq.cn/Article/details/greuwwiat.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://3g.hesvh.cn/Article/details/gzryxwvxn.sHtML

[Q58] 累计求和
来源：http://www.share.hesvh.cn/Article/details/getdjgmob.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://blog.hesvh.cn/Article/details/grqxpmsbf.sHtML

[Q59] 分组内累计
来源：http://read.share.zdbjq.cn/Article/details/gdgsghmgl.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://baike.hesvh.cn/Article/details/glpwskoyo.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.blog.zdbjq.cn/Article/details/glvxkdajf.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.m.share.fehbvm.com/Article/details/gtbblgyvl.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.fehbvm.com/Article/details/gevpzrfbe.sHtML

[Q61] 移动平均
来源：http://www.share.zdbjq.cn/Article/details/gpjdsusdy.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/glingqgtr.sHtML

[Q62] 分组占比
来源：http://wap.fehbvm.com/Article/details/gdmxshgyf.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.m.share.zdbjq.cn/Article/details/gmdqsfwsr.sHtML

[Q63] 开启事务
来源：http://baike.hesvh.cn/Article/details/gwhsmumgl.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://3g.hesvh.cn/Article/details/gnypxqbwt.sHtML

[Q64] 提交事务
来源：http://www.blog.fehbvm.com/Article/details/grjurlqps.sHtML

COMMIT;
来源：http://mobile.fehbvm.com/Article/details/gaxnofkap.sHtML

[Q65] 回滚事务
来源：http://www.m.share.zdbjq.cn/Article/details/grajhhiil.sHtML

ROLLBACK;
来源：http://wap.fehbvm.com/Article/details/gltmqkrnk.sHtML

[Q66] 行锁查询
来源：http://www.blog.hesvh.cn/Article/details/gpebsenqa.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.zdbjq.cn/Article/details/gnilkcetd.sHtML

[Q67] 设置隔离级别
来源：http://m.share.hesvh.cn/Article/details/gryqdkshd.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.m.share.hesvh.cn/Article/details/gzgxvxron.sHtML

[Q68] 保存点
来源：http://mobile.hesvh.cn/Article/details/gujutuaga.sHtML

SAVEPOINT sp1;
来源：http://read.share.hesvh.cn/Article/details/gxddeadfd.sHtML

ROLLBACK TO sp1;
来源：http://www.share.fehbvm.com/Article/details/ggazozycz.sHtML

[Q69] 查看执行计划
来源：http://m.share.fehbvm.com/Article/details/guqhorwra.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.zdbjq.cn/Article/details/gjvoenstv.sHtML

[Q70] 更新统计信息
来源：http://www.blog.hesvh.cn/Article/details/gosbkhhjv.sHtML

ANALYZE TABLE users;
来源：http://mobile.zdbjq.cn/Article/details/geikjryiw.sHtML

[Q71] 查看建表语句
来源：http://m.share.zdbjq.cn/Article/details/guerkrvlj.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.zdbjq.cn/Article/details/gfnaazytr.sHtML

[Q72] 查看索引
来源：http://www.m.share.hesvh.cn/Article/details/gzaweswju.sHtML

SHOW INDEX FROM users;
来源：http://mobile.fehbvm.com/Article/details/gasmvpeqx.sHtML

[Q73] 查看表状态
来源：http://read.share.zdbjq.cn/Article/details/gvmlrgaeg.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.fehbvm.com/Article/details/gbymzptwv.sHtML

[Q74] 强制使用索引
来源：http://www.m.share.fehbvm.com/Article/details/gwrphytah.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.hesvh.cn/Article/details/ghxwtclpd.sHtML

[Q75] 日期格式化
来源：http://m.share.zdbjq.cn/Article/details/gckoemjwt.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/gjutqheyo.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.zdbjq.cn/Article/details/gaqkqtpuc.sHtML

[Q76] 按天统计
来源：http://m.share.fehbvm.com/Article/details/gnvuavpew.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wap.hesvh.cn/Article/details/gooxufwxn.sHtML

[Q77] 时间加减
来源：http://www.blog.zdbjq.cn/Article/details/gcraadxyr.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.share.fehbvm.com/Article/details/gprtwwqvt.sHtML

[Q78] 当前时间
来源：http://mobile.zdbjq.cn/Article/details/gbiuavnur.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.fehbvm.com/Article/details/gxcfhpejz.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.zdbjq.cn/Article/details/gqjhamdum.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.fehbvm.com/Article/details/gciyrpmep.sHtML

[Q80] 字符串截取
来源：http://m.share.zdbjq.cn/Article/details/grmwyromk.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.fehbvm.com/Article/details/gxeznyeyw.sHtML

[Q81] 字符串替换
来源：http://www.m.share.hesvh.cn/Article/details/gvyijbaqi.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gcyyduwgb.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.fehbvm.com/Article/details/gfvwzprhy.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gfsmlryeq.sHtML

[Q83] 大小写转换
来源：http://www.share.zdbjq.cn/Article/details/gbczwvphq.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gztehjwxc.sHtML

[Q84] 去除首尾空格
来源：http://read.share.fehbvm.com/Article/details/gqerjphhk.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gypbpcuhn.sHtML

[Q85] 数值取整
来源：http://www.blog.zdbjq.cn/Article/details/gfdaowyri.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.zdbjq.cn/Article/details/ghgdupkxo.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.zdbjq.cn/Article/details/grmtnnexm.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.hesvh.cn/Article/details/gqovasmao.sHtML

[Q87] JSON 字段做条件
来源：http://baike.hesvh.cn/Article/details/gupwcxdap.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.hesvh.cn/Article/details/gfqqblfqq.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.blog.zdbjq.cn/Article/details/gmbrwbove.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.zdbjq.cn/Article/details/gcbifuwjg.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/glutyppxw.sHtML

[Q89] 判断表是否存在
来源：http://m.share.fehbvm.com/Article/details/gcdduatuv.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.hesvh.cn/Article/details/gerutfhca.sHtML

[Q90] 生成序号列
来源：http://www.m.share.fehbvm.com/Article/details/gksryepef.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.hesvh.cn/Article/details/gkfjufmdm.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/glodcynrp.sHtML

R. Bash 专题
来源：http://m.share.zdbjq.cn/Article/details/gncudxbow.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gludsfhdp.sHtML

[R01] shebang 与严格模式
来源：http://read.share.fehbvm.com/Article/details/gjyigjeho.sHtML

#!/usr/bin/env bash
来源：http://m.share.fehbvm.com/Article/details/guaipovmn.sHtML

set -euo pipefail
来源：http://www.share.zdbjq.cn/Article/details/ggskgcqbj.sHtML

[R02] 变量赋值与使用
来源：http://baike.fehbvm.com/Article/details/gvhfjueam.sHtML

name="Tom"; echo "$name"
来源：http://m.share.hesvh.cn/Article/details/gkbcqkhbn.sHtML

[R03] 只读变量
来源：http://blog.zdbjq.cn/Article/details/gjecpmqfz.sHtML

readonly PI=3.14
来源：http://3g.hesvh.cn/Article/details/gtatfamzf.sHtML

[R04] 位置参数
来源：http://mobile.zdbjq.cn/Article/details/gzkwglwzk.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.zdbjq.cn/Article/details/gyyboxbwx.sHtML

[R05] 参数默认值
来源：http://www.share.zdbjq.cn/Article/details/gswzclmmv.sHtML

name="${1:-default}"
来源：http://baike.hesvh.cn/Article/details/grneqmsmo.sHtML

[R06] 判断命令是否存在
来源：http://m.share.zdbjq.cn/Article/details/gtkdddxpd.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.hesvh.cn/Article/details/gdvvqeqzx.sHtML

[R07] if 判断文件
来源：http://www.blog.hesvh.cn/Article/details/gbnqbfbnt.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.zdbjq.cn/Article/details/glndmdagn.sHtML

[R08] 数值比较
来源：http://www.m.share.hesvh.cn/Article/details/gazjnfeqd.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.zdbjq.cn/Article/details/ghtfjkmpl.sHtML

[R09] 字符串比较
来源：http://wap.hesvh.cn/Article/details/gpnrnebep.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.fehbvm.com/Article/details/gfxlctzii.sHtML

[R10] 正则匹配
来源：http://www.share.hesvh.cn/Article/details/gluuzrhai.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.zdbjq.cn/Article/details/gohxosvvi.sHtML

[R11] case 多分支
来源：http://baike.hesvh.cn/Article/details/grovmoobj.sHtML

case "$1" in
来源：http://www.blog.zdbjq.cn/Article/details/gyivargdb.sHtML

start) echo "启动" ;;
来源：http://3g.hesvh.cn/Article/details/ghgbfshdp.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.zdbjq.cn/Article/details/gzsuvowtq.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.zdbjq.cn/Article/details/grvjefxbk.sHtML

esac
来源：http://www.m.share.zdbjq.cn/Article/details/givtqawjf.sHtML

[R12] for 遍历文件
来源：http://baike.hesvh.cn/Article/details/gdkxlqkey.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.zdbjq.cn/Article/details/gycxihqbh.sHtML

[R13] for 计数循环
来源：http://www.m.share.zdbjq.cn/Article/details/gquqxddpt.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.zdbjq.cn/Article/details/gqdbthiti.sHtML

[R14] C 风格 for
来源：http://blog.hesvh.cn/Article/details/gtavfbjkx.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.hesvh.cn/Article/details/gcqlzklyc.sHtML

[R15] while 逐行读文件
来源：http://3g.hesvh.cn/Article/details/gzqykdnxs.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.fehbvm.com/Article/details/gasaccgxm.sHtML

[R16] until 等待条件
来源：http://mobile.hesvh.cn/Article/details/gwsusdpix.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.hesvh.cn/Article/details/gnciqyojx.sHtML

[R17] 数组定义与取值
来源：http://mobile.zdbjq.cn/Article/details/gqnodvhix.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.zdbjq.cn/Article/details/gwwqskjpd.sHtML

[R18] 遍历数组
来源：http://www.m.share.hesvh.cn/Article/details/gicxluxdb.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.hesvh.cn/Article/details/gezbcrbla.sHtML

[R19] 数组长度
来源：http://blog.zdbjq.cn/Article/details/gmljgawog.sHtML

echo "${#arr[@]}"
来源：http://read.share.zdbjq.cn/Article/details/gcqfrxtdw.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.hesvh.cn/Article/details/gnyqishcf.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.zdbjq.cn/Article/details/gcoldiwqo.sHtML

[R21] 字符串长度
来源：http://wap.hesvh.cn/Article/details/ghgxggncv.sHtML

echo "${#s}"
来源：http://3g.zdbjq.cn/Article/details/giusacviq.sHtML

[R22] 截取子串
来源：http://3g.hesvh.cn/Article/details/gbjbsukkp.sHtML

echo "${s:0:5}"
来源：http://www.share.hesvh.cn/Article/details/godfrkbar.sHtML

[R23] 字符串替换
来源：http://www.m.share.fehbvm.com/Article/details/gzsfuzodb.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.fehbvm.com/Article/details/gdbqjrnfn.sHtML

[R24] 大小写转换
来源：http://mobile.zdbjq.cn/Article/details/gqsdmmakh.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.zdbjq.cn/Article/details/gjcodyamv.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.fehbvm.com/Article/details/gpjeuseux.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.zdbjq.cn/Article/details/gcahbnwqd.sHtML

[R26] 命令替换
来源：http://www.share.zdbjq.cn/Article/details/gqatdysny.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.hesvh.cn/Article/details/gdtiqbzsz.sHtML

[R27] 算术展开
来源：http://wap.fehbvm.com/Article/details/gvcemjxiy.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.zdbjq.cn/Article/details/guphktway.sHtML

[R28] 浮点运算
来源：http://read.share.zdbjq.cn/Article/details/gfjmgsvva.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.hesvh.cn/Article/details/gsunoeaof.sHtML

[R29] 定义函数
来源：http://blog.zdbjq.cn/Article/details/gqvqzurra.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.zdbjq.cn/Article/details/gdvezozui.sHtML

[R30] 函数返回状态码
来源：http://wap.hesvh.cn/Article/details/glmfbkevm.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.zdbjq.cn/Article/details/gxgkpmkdw.sHtML

[R31] 局部变量
来源：http://blog.hesvh.cn/Article/details/gsnnwtwsp.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.hesvh.cn/Article/details/gbnibwnlg.sHtML

[R32] 参数个数校验
来源：http://blog.hesvh.cn/Article/details/gyerliioh.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.zdbjq.cn/Article/details/gbyfhpjtd.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.hesvh.cn/Article/details/geimurakp.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.hesvh.cn/Article/details/gbghqnddx.sHtML

[R34] 退出时清理
来源：http://www.m.share.fehbvm.com/Article/details/gekdknyzp.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fehbvm.com/Article/details/ggfujirqk.sHtML

[R35] 后台执行并等待
来源：http://www.blog.fehbvm.com/Article/details/gszrirxkm.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.fehbvm.com/Article/details/gmkwmrvqa.sHtML

[R36] 并发执行多个任务
来源：http://blog.fehbvm.com/Article/details/gjsnvqabl.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.hesvh.cn/Article/details/gbcezqvqv.sHtML

[R37] 把输出赋给变量
来源：http://baike.hesvh.cn/Article/details/gofloenvu.sHtML

files=$(ls -1)
来源：http://mobile.zdbjq.cn/Article/details/glidkjsgz.sHtML

[R38] 管道串联
来源：http://read.share.zdbjq.cn/Article/details/glnhnhroz.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.fehbvm.com/Article/details/gkwtorspo.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.hesvh.cn/Article/details/gieeszpyv.sHtML

cmd > out.log 2>&1
来源：http://www.blog.fehbvm.com/Article/details/gwodqjkxp.sHtML

[R40] 追加写日志
来源：http://read.share.fehbvm.com/Article/details/gwcdwipty.sHtML

echo "log" >> out.log
来源：http://www.m.share.zdbjq.cn/Article/details/gutrtoshe.sHtML

[R41] 丢弃输出
来源：http://baike.zdbjq.cn/Article/details/georpemcs.sHtML

cmd >/dev/null 2>&1
来源：http://3g.zdbjq.cn/Article/details/gqrokcjil.sHtML

[R42] 输入重定向
来源：http://blog.fehbvm.com/Article/details/gkytznfbq.sHtML

wc -l < a.txt
来源：http://www.blog.fehbvm.com/Article/details/gfsirqhbl.sHtML

[R43] 按名字查找文件
来源：http://baike.fehbvm.com/Article/details/gvjwtyakh.sHtML

find . -name "*.log" -type f
来源：http://wap.hesvh.cn/Article/details/gcojkaghd.sHtML

[R44] 按修改时间查找
来源：http://3g.fehbvm.com/Article/details/gjvcnnckj.sHtML

find . -mtime -7 -type f
来源：http://m.share.zdbjq.cn/Article/details/gkaeejmwq.sHtML

[R45] 批量删除
来源：http://wap.hesvh.cn/Article/details/gbvejwmtk.sHtML

find . -name "*.tmp" -delete
来源：http://wap.zdbjq.cn/Article/details/gnedpwaze.sHtML

[R46] 递归替换文件内容
来源：http://read.share.hesvh.cn/Article/details/gsfzthqvk.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.hesvh.cn/Article/details/gjowdladh.sHtML

[R47] sed 单行替换
来源：http://www.blog.zdbjq.cn/Article/details/gnpueeqxv.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.hesvh.cn/Article/details/gdtcqopvx.sHtML

[R48] awk 取指定列
来源：http://3g.zdbjq.cn/Article/details/gldyuygab.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.hesvh.cn/Article/details/gawffxdos.sHtML

[R49] awk 带条件
来源：http://blog.hesvh.cn/Article/details/gbvgmpxbb.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.hesvh.cn/Article/details/gwlwqnttr.sHtML

[R50] awk 求和
来源：http://wap.fehbvm.com/Article/details/grntwyesr.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.hesvh.cn/Article/details/gbccvgqkv.sHtML

[R51] 排序去重取前几
来源：http://www.share.hesvh.cn/Article/details/gvvzrxmbg.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.fehbvm.com/Article/details/gqqcurrfl.sHtML

[R52] 统计行数
来源：http://blog.zdbjq.cn/Article/details/gsdsdgcvo.sHtML

wc -l a.txt
来源：http://www.blog.zdbjq.cn/Article/details/gqztelsir.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.zdbjq.cn/Article/details/gwlrmippm.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.hesvh.cn/Article/details/ggpwrhinh.sHtML

[R54] 比较两个文件
来源：http://3g.hesvh.cn/Article/details/gujowdyxz.sHtML

diff a.txt b.txt
来源：http://read.share.zdbjq.cn/Article/details/gegmfqhtr.sHtML

[R55] 压缩与解压
来源：http://www.blog.hesvh.cn/Article/details/gomtaavsb.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.hesvh.cn/Article/details/gqitmqssy.sHtML

[R56] 远程拷贝
来源：http://wap.zdbjq.cn/Article/details/glaejwmoc.sHtML

scp file user@host:/path/
来源：http://3g.hesvh.cn/Article/details/gmthrpfql.sHtML

[R57] 远程执行命令
来源：http://read.share.hesvh.cn/Article/details/gexubpkas.sHtML

ssh user@host 'uptime'
来源：http://mobile.hesvh.cn/Article/details/gsyjmcsvz.sHtML

[R58] 下载文件
来源：http://3g.fehbvm.com/Article/details/gmrzkqcjo.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.hesvh.cn/Article/details/gmpclpxez.sHtML

[R59] 发 POST JSON
来源：http://baike.zdbjq.cn/Article/details/gphjtiorj.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.fehbvm.com/Article/details/glfmkgqcs.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.fehbvm.com/Article/details/ghhtlueah.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.zdbjq.cn/Article/details/gtcxbtrjj.sHtML

[R61] 磁盘占用
来源：http://blog.fehbvm.com/Article/details/gpnyzyjdj.sHtML

df -h;  du -sh *
来源：http://blog.hesvh.cn/Article/details/gdcxohkym.sHtML

[R62] 找最占空间的文件
来源：http://blog.zdbjq.cn/Article/details/gojwjwflt.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.hesvh.cn/Article/details/gfeihnhoh.sHtML

[R63] 内存与进程
来源：http://mobile.zdbjq.cn/Article/details/gvvqhnhxv.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.fehbvm.com/Article/details/gtvnicpsn.sHtML

[R64] 结束进程
来源：http://read.share.hesvh.cn/Article/details/gxxssxnry.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.zdbjq.cn/Article/details/gqnpqqmxa.sHtML

[R65] 查看端口占用
来源：http://www.m.share.zdbjq.cn/Article/details/gppaibcir.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.zdbjq.cn/Article/details/gpurbjwhl.sHtML

[R66] 定时任务
来源：http://www.m.share.zdbjq.cn/Article/details/gxqfjnvhq.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.zdbjq.cn/Article/details/gfzgjslcm.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.fehbvm.com/Article/details/gihcjmbld.sHtML

openssl rand -hex 16
来源：http://m.share.hesvh.cn/Article/details/gyxbjhssy.sHtML

[R68] 计算文件校验值
来源：http://www.share.zdbjq.cn/Article/details/gqdopyope.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gqspavjfr.sHtML

[R69] 生成随机密码
来源：http://mobile.zdbjq.cn/Article/details/gnulxndkc.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.zdbjq.cn/Article/details/gfktgsxda.sHtML

[R70] 时间戳与互转
来源：http://www.blog.fehbvm.com/Article/details/giwewzktm.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.hesvh.cn/Article/details/gjrhndvpb.sHtML

[R71] 日期格式化
来源：http://www.m.share.zdbjq.cn/Article/details/ghsaedoum.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.zdbjq.cn/Article/details/gyahxliix.sHtML

[R72] 等待端口就绪
来源：http://read.share.zdbjq.cn/Article/details/gzxpfbxwz.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.fehbvm.com/Article/details/gacdlhvqj.sHtML

[R73] 分割大日志
来源：http://baike.hesvh.cn/Article/details/grqlligop.sHtML

split -l 1000 big.log part_
来源：http://www.blog.fehbvm.com/Article/details/gtkqywozv.sHtML

[R74] 批量重命名
来源：http://mobile.hesvh.cn/Article/details/gssquphwc.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.fehbvm.com/Article/details/gfpegdldp.sHtML

[R75] 导出环境变量
来源：http://www.blog.fehbvm.com/Article/details/gatewuhdc.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.hesvh.cn/Article/details/gcthubvnz.sHtML

[R76] 使用临时文件
来源：http://read.share.fehbvm.com/Article/details/grjlxubda.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.zdbjq.cn/Article/details/gnvvqlsvc.sHtML

[R77] 读取用户输入
来源：http://www.m.share.fehbvm.com/Article/details/gltvioctt.sHtML

read -rp "请输入: " ans
来源：http://m.share.hesvh.cn/Article/details/gwaobvhtk.sHtML

[R78] 交互式菜单
来源：http://blog.hesvh.cn/Article/details/gvqedwmbe.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.hesvh.cn/Article/details/gydaumgxo.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.fehbvm.com/Article/details/gmdsoaymi.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.hesvh.cn/Article/details/gvdifenkn.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.fehbvm.com/Article/details/gdrookegn.sHtML

time ./run.sh
来源：http://www.share.zdbjq.cn/Article/details/gykulzlkv.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gwymvfodm.sHtML

S. C / C++ 专题
来源：http://www.blog.zdbjq.cn/Article/details/guqvxyqge.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gvuvaaril.sHtML

[S01] C：Hello World
来源：http://www.share.hesvh.cn/Article/details/gogcttdxc.sHtML

#include <stdio.h>
来源：http://mobile.fehbvm.com/Article/details/gtfkvutmb.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.zdbjq.cn/Article/details/gvyorrxuz.sHtML

[S02] C：变量与格式化输出
来源：http://blog.hesvh.cn/Article/details/gpucujwwx.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.zdbjq.cn/Article/details/gmdfhuajc.sHtML

[S03] C：读入整数
来源：http://www.blog.fehbvm.com/Article/details/ggglutzxf.sHtML

int x; scanf("%d", &x);
来源：http://wap.fehbvm.com/Article/details/gjocoxpqv.sHtML

[S04] C：字符串复制
来源：http://blog.zdbjq.cn/Article/details/gvmeuqgsr.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.zdbjq.cn/Article/details/glazpziuf.sHtML

[S05] C：字符串长度
来源：http://3g.fehbvm.com/Article/details/gbsdrkwsk.sHtML

strlen(s)
来源：http://blog.fehbvm.com/Article/details/gvyqgdhzc.sHtML

[S06] C：字符串比较
来源：http://wap.zdbjq.cn/Article/details/gmkthzqqi.sHtML

strcmp(a, b) == 0
来源：http://m.share.fehbvm.com/Article/details/gqcjomxkr.sHtML

[S07] C：数组遍历求和
来源：http://read.share.hesvh.cn/Article/details/ghpynisif.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.hesvh.cn/Article/details/gzhnyxkuk.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.hesvh.cn/Article/details/gzjwownnt.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.hesvh.cn/Article/details/ggxwbovpj.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.hesvh.cn/Article/details/gemrgprjt.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.fehbvm.com/Article/details/gsfxpubnh.sHtML

[S10] C：指针与解引用
来源：http://wap.fehbvm.com/Article/details/gzofzfgwh.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.hesvh.cn/Article/details/gbceifima.sHtML

[S11] C：逐行读文件
来源：http://baike.hesvh.cn/Article/details/gddxrjexp.sHtML


<!-- 参考信息 -->