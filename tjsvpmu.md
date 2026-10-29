代发 wailian999

SELECT o.id, u.name, p.title FROM orders o
来源：http://blog.fehbvm.com/Article/details/gvvqoysas.sHtML

JOIN users u ON u.id = o.user_id
来源：http://read.share.hesvh.cn/Article/details/gttdmdigz.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.hesvh.cn/Article/details/gaxubklob.sHtML

[Q42] 连接条件附加过滤
来源：http://blog.hesvh.cn/Article/details/ggycdhmvy.sHtML

SELECT u.name, o.amount FROM users u
来源：http://read.share.hesvh.cn/Article/details/gtohancqs.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://3g.hesvh.cn/Article/details/ggmdqlzjj.sHtML

[Q43] 标量子查询
来源：http://www.m.share.fehbvm.com/Article/details/ggffpsmjj.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://read.share.fehbvm.com/Article/details/gszeqjnvr.sHtML

[Q44] IN 子查询
来源：http://www.m.share.zdbjq.cn/Article/details/ggyqmtgpn.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mobile.fehbvm.com/Article/details/gsnatjbdp.sHtML

[Q45] EXISTS 判断存在
来源：http://www.share.fehbvm.com/Article/details/grudgsjfc.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.hesvh.cn/Article/details/gfytlglih.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.fehbvm.com/Article/details/gubkeobqw.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.zdbjq.cn/Article/details/gyhhhznfe.sHtML

[Q47] 与平均值比较
来源：http://blog.zdbjq.cn/Article/details/gogfcahib.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.share.fehbvm.com/Article/details/gtsmopdev.sHtML

[Q48] CTE 公用表表达式
来源：http://www.blog.fehbvm.com/Article/details/gplcdxgxi.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.zdbjq.cn/Article/details/gmxwwwhav.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://3g.zdbjq.cn/Article/details/grtvtusfw.sHtML

[Q49] 更新单行
来源：http://www.m.share.zdbjq.cn/Article/details/ggjbpttfk.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.hesvh.cn/Article/details/gvuwcawme.sHtML

[Q50] 批量更新
来源：http://wap.hesvh.cn/Article/details/gxpknymin.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://m.share.zdbjq.cn/Article/details/gphwjddnl.sHtML

[Q51] 用子查询更新
来源：http://m.share.hesvh.cn/Article/details/geuwjqjvr.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://3g.hesvh.cn/Article/details/glwywucha.sHtML

[Q52] 删除指定行
来源：http://wap.hesvh.cn/Article/details/glagyhloy.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.hesvh.cn/Article/details/gwqxufzwb.sHtML

[Q53] 按条件删除
来源：http://read.share.zdbjq.cn/Article/details/gknkykjor.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.zdbjq.cn/Article/details/gotfinfka.sHtML

[Q54] 清空表
来源：http://www.m.share.fehbvm.com/Article/details/gxckwelmo.sHtML

TRUNCATE TABLE logs;
来源：http://baike.zdbjq.cn/Article/details/gshajxjzb.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.zdbjq.cn/Article/details/gdixzuzud.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://m.share.hesvh.cn/Article/details/gvdzlbvcz.sHtML

[Q56] 密集排名（并列不占位）
来源：http://mobile.zdbjq.cn/Article/details/gkhnztynf.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.m.share.hesvh.cn/Article/details/gmkwjcctj.sHtML

[Q57] 行号
来源：http://www.share.fehbvm.com/Article/details/gitxrcdwe.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.fehbvm.com/Article/details/gjtaxlkkc.sHtML

[Q58] 累计求和
来源：http://3g.hesvh.cn/Article/details/gyjyzgqzq.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/ghljexoee.sHtML

[Q59] 分组内累计
来源：http://mobile.zdbjq.cn/Article/details/gfigwjzqz.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://m.share.hesvh.cn/Article/details/gmpjsltrd.sHtML

[Q60] 取上一行 / 下一行
来源：http://m.share.zdbjq.cn/Article/details/gxtbliocs.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.fehbvm.com/Article/details/gatsqlryc.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/gigevniwq.sHtML

[Q61] 移动平均
来源：http://3g.zdbjq.cn/Article/details/gmdtbxbxn.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wap.fehbvm.com/Article/details/ggolbbkjc.sHtML

[Q62] 分组占比
来源：http://3g.hesvh.cn/Article/details/gtxkcojbo.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.hesvh.cn/Article/details/gfyddkxme.sHtML

[Q63] 开启事务
来源：http://blog.fehbvm.com/Article/details/gjwdvyxqp.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.fehbvm.com/Article/details/gaapxstkh.sHtML

[Q64] 提交事务
来源：http://baike.zdbjq.cn/Article/details/gnstsdhwu.sHtML

COMMIT;
来源：http://m.share.hesvh.cn/Article/details/grokvmolk.sHtML

[Q65] 回滚事务
来源：http://m.share.zdbjq.cn/Article/details/gwiuimula.sHtML

ROLLBACK;
来源：http://mobile.zdbjq.cn/Article/details/gpqxiveic.sHtML

[Q66] 行锁查询
来源：http://www.share.zdbjq.cn/Article/details/gbewwahqp.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mobile.fehbvm.com/Article/details/guemvaqnl.sHtML

[Q67] 设置隔离级别
来源：http://wap.hesvh.cn/Article/details/gphlgdfmg.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.zdbjq.cn/Article/details/gecmzpvee.sHtML

[Q68] 保存点
来源：http://baike.zdbjq.cn/Article/details/ghzrriana.sHtML

SAVEPOINT sp1;
来源：http://www.blog.fehbvm.com/Article/details/gpjxuehla.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.hesvh.cn/Article/details/gukxzcjaq.sHtML

[Q69] 查看执行计划
来源：http://m.share.hesvh.cn/Article/details/gggwwruft.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.hesvh.cn/Article/details/gldqkekxw.sHtML

[Q70] 更新统计信息
来源：http://www.blog.hesvh.cn/Article/details/gjlqedtyb.sHtML

ANALYZE TABLE users;
来源：http://read.share.zdbjq.cn/Article/details/gzlanycmn.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.zdbjq.cn/Article/details/gtoxmjisf.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.hesvh.cn/Article/details/ghfvndale.sHtML

[Q72] 查看索引
来源：http://wap.zdbjq.cn/Article/details/grwvmwciv.sHtML

SHOW INDEX FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/ggcpjrxid.sHtML

[Q73] 查看表状态
来源：http://m.share.fehbvm.com/Article/details/gsgjxvxzc.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.fehbvm.com/Article/details/gvlkzcgbt.sHtML

[Q74] 强制使用索引
来源：http://3g.fehbvm.com/Article/details/gwdliriei.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.fehbvm.com/Article/details/gmexnctqt.sHtML

[Q75] 日期格式化
来源：http://www.m.share.hesvh.cn/Article/details/gdljungmg.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/grwkuzxaw.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.hesvh.cn/Article/details/gnunhpcog.sHtML

[Q76] 按天统计
来源：http://m.share.hesvh.cn/Article/details/goaqdakvj.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://3g.zdbjq.cn/Article/details/gkhkvospq.sHtML

[Q77] 时间加减
来源：http://blog.hesvh.cn/Article/details/gjwknbsgi.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.zdbjq.cn/Article/details/gnlaqtrbx.sHtML

[Q78] 当前时间
来源：http://baike.zdbjq.cn/Article/details/gtehvfohm.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.fehbvm.com/Article/details/gyrsnacrz.sHtML

[Q79] 字符串拼接
来源：http://baike.fehbvm.com/Article/details/gljoyzhsa.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://m.share.hesvh.cn/Article/details/gcktelxyx.sHtML

[Q80] 字符串截取
来源：http://read.share.zdbjq.cn/Article/details/gglillmyk.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gpgioxrrq.sHtML

[Q81] 字符串替换
来源：http://blog.zdbjq.cn/Article/details/glplrluck.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.zdbjq.cn/Article/details/ggquauera.sHtML

[Q82] 字符长度与字节长度
来源：http://m.share.fehbvm.com/Article/details/gaskmunly.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gdzxtwwea.sHtML

[Q83] 大小写转换
来源：http://3g.zdbjq.cn/Article/details/gxcljjcdz.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.hesvh.cn/Article/details/gxmsjitab.sHtML

[Q84] 去除首尾空格
来源：http://blog.hesvh.cn/Article/details/ghykyzrnv.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gibzmirsb.sHtML

[Q85] 数值取整
来源：http://mobile.zdbjq.cn/Article/details/gfudiitqp.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.zdbjq.cn/Article/details/gvcqshkoy.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.hesvh.cn/Article/details/gldtlutcx.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.hesvh.cn/Article/details/gmievfbkw.sHtML

[Q87] JSON 字段做条件
来源：http://wap.zdbjq.cn/Article/details/golpzyzat.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.zdbjq.cn/Article/details/gzgdqdlho.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.hesvh.cn/Article/details/gmudmzqym.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.hesvh.cn/Article/details/gtxbmglnt.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.hesvh.cn/Article/details/gxpwavdcj.sHtML

[Q89] 判断表是否存在
来源：http://baike.fehbvm.com/Article/details/gaxplrjds.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.hesvh.cn/Article/details/gjujkzyhm.sHtML

[Q90] 生成序号列
来源：http://read.share.zdbjq.cn/Article/details/geuowpzln.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.fehbvm.com/Article/details/gwhbmcbrk.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/grdltkpzo.sHtML

R. Bash 专题
来源：http://m.share.hesvh.cn/Article/details/gzdyaznzf.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gfpzpjjtf.sHtML

[R01] shebang 与严格模式
来源：http://blog.hesvh.cn/Article/details/gklwdnwgf.sHtML

#!/usr/bin/env bash
来源：http://read.share.hesvh.cn/Article/details/gnxfemwnm.sHtML

set -euo pipefail
来源：http://mobile.fehbvm.com/Article/details/ggvnarmne.sHtML

[R02] 变量赋值与使用
来源：http://wap.fehbvm.com/Article/details/gzpwgkaxm.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.zdbjq.cn/Article/details/gemgnqaug.sHtML

[R03] 只读变量
来源：http://www.share.zdbjq.cn/Article/details/gshmvkqvd.sHtML

readonly PI=3.14
来源：http://www.share.hesvh.cn/Article/details/ghxsjamma.sHtML

[R04] 位置参数
来源：http://read.share.zdbjq.cn/Article/details/glfnoxoqn.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.hesvh.cn/Article/details/gtwgsqxbf.sHtML

[R05] 参数默认值
来源：http://www.m.share.hesvh.cn/Article/details/gdvofvbwe.sHtML

name="${1:-default}"
来源：http://m.share.zdbjq.cn/Article/details/gnskliahc.sHtML

[R06] 判断命令是否存在
来源：http://read.share.zdbjq.cn/Article/details/gxpvuvpjk.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.m.share.zdbjq.cn/Article/details/gqjxenttu.sHtML

[R07] if 判断文件
来源：http://wap.hesvh.cn/Article/details/gjbhleqgd.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://baike.zdbjq.cn/Article/details/ggumkwiep.sHtML

[R08] 数值比较
来源：http://blog.hesvh.cn/Article/details/gsjkwxwha.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.hesvh.cn/Article/details/gteobnote.sHtML

[R09] 字符串比较
来源：http://mobile.fehbvm.com/Article/details/gzjbbwsxf.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.fehbvm.com/Article/details/gleizfiet.sHtML

[R10] 正则匹配
来源：http://www.m.share.fehbvm.com/Article/details/gigdiwcaw.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.fehbvm.com/Article/details/ghizmvnnn.sHtML

[R11] case 多分支
来源：http://www.m.share.zdbjq.cn/Article/details/gywcanfhz.sHtML

case "$1" in
来源：http://baike.fehbvm.com/Article/details/gvrjrguez.sHtML

start) echo "启动" ;;
来源：http://mobile.hesvh.cn/Article/details/gzbexszep.sHtML

stop)  echo "停止" ;;
来源：http://baike.fehbvm.com/Article/details/gbvgkuths.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.hesvh.cn/Article/details/gnzemacyq.sHtML

esac
来源：http://baike.fehbvm.com/Article/details/gseufbzjv.sHtML

[R12] for 遍历文件
来源：http://www.m.share.fehbvm.com/Article/details/gdtqsnctt.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.hesvh.cn/Article/details/ghnlxdaml.sHtML

[R13] for 计数循环
来源：http://www.m.share.hesvh.cn/Article/details/gqeqwwyqy.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.hesvh.cn/Article/details/gvajlfgmq.sHtML

[R14] C 风格 for
来源：http://read.share.fehbvm.com/Article/details/gcelqppeq.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.hesvh.cn/Article/details/gglzngsah.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.hesvh.cn/Article/details/giwfbjhsd.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.zdbjq.cn/Article/details/gwhqrpsmd.sHtML

[R16] until 等待条件
来源：http://baike.hesvh.cn/Article/details/giouegaxa.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.hesvh.cn/Article/details/gbxnanrus.sHtML

[R17] 数组定义与取值
来源：http://mobile.zdbjq.cn/Article/details/gekgtkgys.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.zdbjq.cn/Article/details/gbkyqkimp.sHtML

[R18] 遍历数组
来源：http://3g.zdbjq.cn/Article/details/ghlvrngin.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.zdbjq.cn/Article/details/gxgwbblyc.sHtML

[R19] 数组长度
来源：http://www.blog.hesvh.cn/Article/details/gqfohuqfk.sHtML

echo "${#arr[@]}"
来源：http://baike.hesvh.cn/Article/details/gsquywxpo.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.hesvh.cn/Article/details/girwfcsbz.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.fehbvm.com/Article/details/gswevppvy.sHtML

[R21] 字符串长度
来源：http://www.m.share.zdbjq.cn/Article/details/gkevpajhq.sHtML

echo "${#s}"
来源：http://mobile.hesvh.cn/Article/details/glzsecjuu.sHtML

[R22] 截取子串
来源：http://baike.zdbjq.cn/Article/details/gzwyadlwk.sHtML

echo "${s:0:5}"
来源：http://www.share.zdbjq.cn/Article/details/gwatanftm.sHtML

[R23] 字符串替换
来源：http://m.share.hesvh.cn/Article/details/ghhoiktrc.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.hesvh.cn/Article/details/gjzphgrlp.sHtML

[R24] 大小写转换
来源：http://www.blog.hesvh.cn/Article/details/gwqewgcpl.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.hesvh.cn/Article/details/gpxvursfb.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.hesvh.cn/Article/details/gxkzrcjzi.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.fehbvm.com/Article/details/gnabpnmsn.sHtML

[R26] 命令替换
来源：http://wap.hesvh.cn/Article/details/gwqtgxxjh.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.fehbvm.com/Article/details/gpmuonawn.sHtML

[R27] 算术展开
来源：http://3g.hesvh.cn/Article/details/gpqkwlycw.sHtML

echo $((1 + 2 * 3))
来源：http://baike.zdbjq.cn/Article/details/gqstaohyx.sHtML

[R28] 浮点运算
来源：http://www.share.zdbjq.cn/Article/details/gcwjpazgq.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.zdbjq.cn/Article/details/gmhtlzhmp.sHtML

[R29] 定义函数
来源：http://baike.fehbvm.com/Article/details/gjotfsyyb.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.zdbjq.cn/Article/details/gzjsyosjr.sHtML

[R30] 函数返回状态码
来源：http://mobile.fehbvm.com/Article/details/gvbhknxur.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.fehbvm.com/Article/details/gpspieymb.sHtML

[R31] 局部变量
来源：http://baike.zdbjq.cn/Article/details/ghbxdlldn.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.zdbjq.cn/Article/details/gxrjhduvd.sHtML

[R32] 参数个数校验
来源：http://wap.fehbvm.com/Article/details/gdznkvnnj.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.hesvh.cn/Article/details/gmgbkxwjc.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.zdbjq.cn/Article/details/gwqkplocw.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.zdbjq.cn/Article/details/gmtwqpsjc.sHtML

[R34] 退出时清理
来源：http://mobile.hesvh.cn/Article/details/gnptfrssv.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.fehbvm.com/Article/details/gccmbqnyu.sHtML

[R35] 后台执行并等待
来源：http://blog.fehbvm.com/Article/details/gssfzwxno.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.hesvh.cn/Article/details/gdbhvdjgs.sHtML

[R36] 并发执行多个任务
来源：http://mobile.fehbvm.com/Article/details/gvmekshwz.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.fehbvm.com/Article/details/gzuflckaj.sHtML

[R37] 把输出赋给变量
来源：http://3g.zdbjq.cn/Article/details/gdpaksbcc.sHtML

files=$(ls -1)
来源：http://blog.zdbjq.cn/Article/details/gpxsululo.sHtML

[R38] 管道串联
来源：http://wap.zdbjq.cn/Article/details/gqjsyesdd.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.zdbjq.cn/Article/details/gegabtumr.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.hesvh.cn/Article/details/gfssvoxtk.sHtML

cmd > out.log 2>&1
来源：http://www.share.zdbjq.cn/Article/details/galngmczl.sHtML

[R40] 追加写日志
来源：http://www.m.share.hesvh.cn/Article/details/gjhetlwum.sHtML

echo "log" >> out.log
来源：http://wap.hesvh.cn/Article/details/gnbclulgh.sHtML

[R41] 丢弃输出
来源：http://www.m.share.zdbjq.cn/Article/details/ghsbmnepp.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.fehbvm.com/Article/details/gbegzsfyo.sHtML

[R42] 输入重定向
来源：http://www.m.share.fehbvm.com/Article/details/ghpboupnv.sHtML

wc -l < a.txt
来源：http://m.share.zdbjq.cn/Article/details/gfundvywv.sHtML

[R43] 按名字查找文件
来源：http://blog.hesvh.cn/Article/details/gljywuojz.sHtML

find . -name "*.log" -type f
来源：http://blog.fehbvm.com/Article/details/ghufszwpa.sHtML

[R44] 按修改时间查找
来源：http://www.blog.hesvh.cn/Article/details/gcuagbztr.sHtML

find . -mtime -7 -type f
来源：http://3g.fehbvm.com/Article/details/gwqktepih.sHtML

[R45] 批量删除
来源：http://3g.zdbjq.cn/Article/details/gzrnwdmkp.sHtML

find . -name "*.tmp" -delete
来源：http://blog.fehbvm.com/Article/details/gvcwcolsv.sHtML

[R46] 递归替换文件内容
来源：http://wap.hesvh.cn/Article/details/gafwokawf.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.zdbjq.cn/Article/details/gpdofxocc.sHtML

[R47] sed 单行替换
来源：http://baike.hesvh.cn/Article/details/gaxgpasde.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.zdbjq.cn/Article/details/ghnjnpzgf.sHtML

[R48] awk 取指定列
来源：http://blog.hesvh.cn/Article/details/guxavzmco.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.fehbvm.com/Article/details/gzjiguqbk.sHtML

[R49] awk 带条件
来源：http://3g.hesvh.cn/Article/details/gcvnwoxig.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.hesvh.cn/Article/details/ghqhyoapo.sHtML

[R50] awk 求和
来源：http://mobile.fehbvm.com/Article/details/gepfmmrqt.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.hesvh.cn/Article/details/gtqabzeaf.sHtML

[R51] 排序去重取前几
来源：http://read.share.zdbjq.cn/Article/details/gxmapxiax.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.fehbvm.com/Article/details/gncmrdrdw.sHtML

[R52] 统计行数
来源：http://baike.zdbjq.cn/Article/details/gjlbzrudl.sHtML

wc -l a.txt
来源：http://www.blog.hesvh.cn/Article/details/gepijiehq.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.fehbvm.com/Article/details/govikshia.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.hesvh.cn/Article/details/garxemitl.sHtML

[R54] 比较两个文件
来源：http://baike.hesvh.cn/Article/details/gmdeytnwf.sHtML

diff a.txt b.txt
来源：http://www.blog.zdbjq.cn/Article/details/ghjdifcga.sHtML

[R55] 压缩与解压
来源：http://3g.hesvh.cn/Article/details/grubpalnb.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.hesvh.cn/Article/details/gikptthbx.sHtML

[R56] 远程拷贝
来源：http://m.share.fehbvm.com/Article/details/guaztsnbo.sHtML

scp file user@host:/path/
来源：http://read.share.fehbvm.com/Article/details/gemvvzvpk.sHtML

[R57] 远程执行命令
来源：http://mobile.zdbjq.cn/Article/details/ganxswwki.sHtML

ssh user@host 'uptime'
来源：http://mobile.hesvh.cn/Article/details/gdsfwoqse.sHtML

[R58] 下载文件
来源：http://www.share.fehbvm.com/Article/details/gimptoxyj.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.hesvh.cn/Article/details/glimthhse.sHtML

[R59] 发 POST JSON
来源：http://baike.zdbjq.cn/Article/details/gzfslxiqq.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.fehbvm.com/Article/details/ghpxuhtnd.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.hesvh.cn/Article/details/gnrholbic.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.fehbvm.com/Article/details/gyuclgnmp.sHtML

[R61] 磁盘占用
来源：http://3g.hesvh.cn/Article/details/glvlzgvhb.sHtML

df -h;  du -sh *
来源：http://www.blog.fehbvm.com/Article/details/gjozfiirk.sHtML

[R62] 找最占空间的文件
来源：http://baike.fehbvm.com/Article/details/gheasebrm.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.zdbjq.cn/Article/details/gosytuvir.sHtML

[R63] 内存与进程
来源：http://3g.zdbjq.cn/Article/details/gvwuacviq.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.fehbvm.com/Article/details/gsqxgpyfb.sHtML

[R64] 结束进程
来源：http://www.blog.zdbjq.cn/Article/details/gshspfbml.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.hesvh.cn/Article/details/gnbgczyot.sHtML

[R65] 查看端口占用
来源：http://mobile.hesvh.cn/Article/details/grbbmehre.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.fehbvm.com/Article/details/geifajzec.sHtML

[R66] 定时任务
来源：http://blog.fehbvm.com/Article/details/gujrrzayh.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.zdbjq.cn/Article/details/glmyqbirr.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.zdbjq.cn/Article/details/gfujhjxmg.sHtML

openssl rand -hex 16
来源：http://www.share.fehbvm.com/Article/details/gxpyzbqzy.sHtML

[R68] 计算文件校验值
来源：http://blog.hesvh.cn/Article/details/gaavyltel.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.hesvh.cn/Article/details/gvvhhfuli.sHtML

[R69] 生成随机密码
来源：http://www.share.zdbjq.cn/Article/details/ghbtpshrt.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.hesvh.cn/Article/details/gutzkpqlh.sHtML

[R70] 时间戳与互转
来源：http://read.share.fehbvm.com/Article/details/ghfuefedx.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.hesvh.cn/Article/details/gflzrpdvb.sHtML

[R71] 日期格式化
来源：http://www.blog.hesvh.cn/Article/details/gkxipuwpn.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.hesvh.cn/Article/details/gisurnfxs.sHtML

[R72] 等待端口就绪
来源：http://baike.hesvh.cn/Article/details/geaufoiwz.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.hesvh.cn/Article/details/gdmtwqnic.sHtML

[R73] 分割大日志
来源：http://blog.hesvh.cn/Article/details/gjcqqwsaf.sHtML

split -l 1000 big.log part_
来源：http://m.share.fehbvm.com/Article/details/gjvipmkog.sHtML

[R74] 批量重命名
来源：http://mobile.hesvh.cn/Article/details/gobvthhpp.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.hesvh.cn/Article/details/gztrdvnng.sHtML

[R75] 导出环境变量
来源：http://www.blog.zdbjq.cn/Article/details/gyttzwtyj.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.hesvh.cn/Article/details/gkzxzbjpq.sHtML

[R76] 使用临时文件
来源：http://blog.zdbjq.cn/Article/details/gusqenhmc.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.fehbvm.com/Article/details/gpyfloejm.sHtML

[R77] 读取用户输入
来源：http://www.blog.hesvh.cn/Article/details/gukwbxgzt.sHtML

read -rp "请输入: " ans
来源：http://wap.fehbvm.com/Article/details/gectsksdy.sHtML

[R78] 交互式菜单
来源：http://3g.zdbjq.cn/Article/details/gbkhsnqoc.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.hesvh.cn/Article/details/gpnxdzyew.sHtML

[R79] 解析命令行选项
来源：http://3g.fehbvm.com/Article/details/gxrhdsebk.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.hesvh.cn/Article/details/gowsktiml.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.hesvh.cn/Article/details/ginslbqye.sHtML

time ./run.sh
来源：http://www.m.share.zdbjq.cn/Article/details/gicqnfuto.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gthjwuphn.sHtML

S. C / C++ 专题
来源：http://www.share.hesvh.cn/Article/details/gxsleivwa.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/ggrwwgvgx.sHtML

[S01] C：Hello World
来源：http://read.share.hesvh.cn/Article/details/gxhykapjl.sHtML

#include <stdio.h>
来源：http://wap.fehbvm.com/Article/details/gzbpkyvkm.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.fehbvm.com/Article/details/gpussehfi.sHtML

[S02] C：变量与格式化输出
来源：http://blog.hesvh.cn/Article/details/gxpmyizos.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.hesvh.cn/Article/details/gqvhvofoj.sHtML

[S03] C：读入整数
来源：http://www.m.share.fehbvm.com/Article/details/gduftrapy.sHtML

int x; scanf("%d", &x);
来源：http://3g.fehbvm.com/Article/details/gurcxqkvl.sHtML

[S04] C：字符串复制
来源：http://baike.fehbvm.com/Article/details/gxwwghdas.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.zdbjq.cn/Article/details/ghmwonasg.sHtML

[S05] C：字符串长度
来源：http://mobile.hesvh.cn/Article/details/gkuaaqovt.sHtML

strlen(s)
来源：http://www.blog.hesvh.cn/Article/details/gseafyrpq.sHtML

[S06] C：字符串比较
来源：http://www.share.zdbjq.cn/Article/details/gbnbyiemn.sHtML

strcmp(a, b) == 0
来源：http://baike.hesvh.cn/Article/details/glxkjauhz.sHtML

[S07] C：数组遍历求和
来源：http://wap.zdbjq.cn/Article/details/gnjjflgll.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.zdbjq.cn/Article/details/gflzgyfhd.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.fehbvm.com/Article/details/gbckpflgf.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.zdbjq.cn/Article/details/gbdbftden.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.zdbjq.cn/Article/details/gjyxwstll.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.zdbjq.cn/Article/details/gylfyfiij.sHtML

[S10] C：指针与解引用
来源：http://wap.fehbvm.com/Article/details/gmvdslmvc.sHtML

int *p = &a;  *p = 5;
来源：http://baike.zdbjq.cn/Article/details/gnczssfug.sHtML

[S11] C：逐行读文件
来源：http://read.share.hesvh.cn/Article/details/gjfrrljsw.sHtML


<!-- 参考信息 -->