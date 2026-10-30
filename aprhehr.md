代发 wailian999

[Q44] IN 子查询
来源：http://3g.fanxiaobao.xyz/Article/details/gnbmymlfy.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpgycuhkg.sHtML

[Q45] EXISTS 判断存在
来源：http://read.share.fanxiaobao.xyz/Article/details/gjfttqpdu.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gumgrcgsk.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzevmfdjk.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.fanxiaobao.xyz/Article/details/gwpcrtuxd.sHtML

[Q47] 与平均值比较
来源：http://blog.fanxiaobao.xyz/Article/details/guxbqpfke.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtndrcafx.sHtML

[Q48] CTE 公用表表达式
来源：http://mobile.fanxiaobao.xyz/Article/details/gvepgdypt.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://baike.fanxiaobao.xyz/Article/details/gzgdsfgzf.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://baike.fanxiaobao.xyz/Article/details/gtpbmwfnf.sHtML

[Q49] 更新单行
来源：http://wap.fanxiaobao.xyz/Article/details/goqhjaued.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://blog.fanxiaobao.xyz/Article/details/gcmvbfuzf.sHtML

[Q50] 批量更新
来源：http://read.share.fanxiaobao.xyz/Article/details/grvyqzanl.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.fanxiaobao.xyz/Article/details/gqcbdxicj.sHtML

[Q51] 用子查询更新
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gigvaqyjf.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gadomzlyq.sHtML

[Q52] 删除指定行
来源：http://www.blog.fanxiaobao.xyz/Article/details/gliqwnzeo.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghtwjysdz.sHtML

[Q53] 按条件删除
来源：http://3g.fanxiaobao.xyz/Article/details/gflrvqvnf.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wap.fanxiaobao.xyz/Article/details/glbadayzv.sHtML

[Q54] 清空表
来源：http://blog.fanxiaobao.xyz/Article/details/gfvljzpex.sHtML

TRUNCATE TABLE logs;
来源：http://www.share.fanxiaobao.xyz/Article/details/grvlwimjn.sHtML

[Q55] 排名（并列占位）
来源：http://m.share.fanxiaobao.xyz/Article/details/glevuvxbh.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggcltnoyz.sHtML

[Q56] 密集排名（并列不占位）
来源：http://3g.fanxiaobao.xyz/Article/details/glsxhlays.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://baike.fanxiaobao.xyz/Article/details/grqskomou.sHtML

[Q57] 行号
来源：http://m.share.fanxiaobao.xyz/Article/details/gcbzqxsgc.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/grdiwjuek.sHtML

[Q58] 累计求和
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grxolbtpw.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.fanxiaobao.xyz/Article/details/gixxxnbyf.sHtML

[Q59] 分组内累计
来源：http://www.share.fanxiaobao.xyz/Article/details/goytbmeuc.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.fanxiaobao.xyz/Article/details/gzydfpeam.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.blog.fanxiaobao.xyz/Article/details/guzqawort.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.fanxiaobao.xyz/Article/details/gittqompg.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.share.fanxiaobao.xyz/Article/details/gxmsjbekr.sHtML

[Q61] 移动平均
来源：http://mobile.fanxiaobao.xyz/Article/details/gskcniiem.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goeoxetqf.sHtML

[Q62] 分组占比
来源：http://m.share.fanxiaobao.xyz/Article/details/gplvmtyuy.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mobile.fanxiaobao.xyz/Article/details/ghaizfqgv.sHtML

[Q63] 开启事务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpcnpccti.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnmtllpey.sHtML

[Q64] 提交事务
来源：http://3g.fanxiaobao.xyz/Article/details/ghnnvfgyp.sHtML

COMMIT;
来源：http://wap.fanxiaobao.xyz/Article/details/gciuehswa.sHtML

[Q65] 回滚事务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmzgadimu.sHtML

ROLLBACK;
来源：http://m.share.fanxiaobao.xyz/Article/details/gixkzammz.sHtML

[Q66] 行锁查询
来源：http://3g.fanxiaobao.xyz/Article/details/gosnbeghq.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaxfyrsbz.sHtML

[Q67] 设置隔离级别
来源：http://wap.fanxiaobao.xyz/Article/details/ggmvqzpoe.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://3g.fanxiaobao.xyz/Article/details/gvvkxbgwo.sHtML

[Q68] 保存点
来源：http://read.share.fanxiaobao.xyz/Article/details/gbekbouov.sHtML

SAVEPOINT sp1;
来源：http://read.share.fanxiaobao.xyz/Article/details/ggiologsi.sHtML

ROLLBACK TO sp1;
来源：http://wap.fanxiaobao.xyz/Article/details/gvgpvbaqv.sHtML

[Q69] 查看执行计划
来源：http://mobile.fanxiaobao.xyz/Article/details/gdokdzgva.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.fanxiaobao.xyz/Article/details/gcjxuhsnc.sHtML

[Q70] 更新统计信息
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grnhdfazl.sHtML

ANALYZE TABLE users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gnzjhqgal.sHtML

[Q71] 查看建表语句
来源：http://baike.fanxiaobao.xyz/Article/details/gmrnwqygh.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://blog.fanxiaobao.xyz/Article/details/gpvykmmfi.sHtML

[Q72] 查看索引
来源：http://blog.fanxiaobao.xyz/Article/details/gtzuizgbg.sHtML

SHOW INDEX FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcsokhcau.sHtML

[Q73] 查看表状态
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwmbikdae.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.fanxiaobao.xyz/Article/details/gmmziqldg.sHtML

[Q74] 强制使用索引
来源：http://wap.fanxiaobao.xyz/Article/details/ggfizqioi.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.fanxiaobao.xyz/Article/details/grylwiqje.sHtML

[Q75] 日期格式化
来源：http://m.share.fanxiaobao.xyz/Article/details/gnxddnpoy.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://m.share.fanxiaobao.xyz/Article/details/gughjeuiv.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.fanxiaobao.xyz/Article/details/gmsqcagtv.sHtML

[Q76] 按天统计
来源：http://www.share.fanxiaobao.xyz/Article/details/guibcxmst.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.fanxiaobao.xyz/Article/details/grrjnozqq.sHtML

[Q77] 时间加减
来源：http://baike.fanxiaobao.xyz/Article/details/gjshtabip.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.fanxiaobao.xyz/Article/details/gtciefpvt.sHtML

[Q78] 当前时间
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbshwobhn.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.fanxiaobao.xyz/Article/details/ghfqoyhrb.sHtML

[Q79] 字符串拼接
来源：http://wap.fanxiaobao.xyz/Article/details/ghrhfnlvx.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.fanxiaobao.xyz/Article/details/gprjxakem.sHtML

[Q80] 字符串截取
来源：http://m.share.fanxiaobao.xyz/Article/details/gueggcudx.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gdeueatui.sHtML

[Q81] 字符串替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gdmszgzlu.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gzpjcxwpj.sHtML

[Q82] 字符长度与字节长度
来源：http://blog.fanxiaobao.xyz/Article/details/gfzvbfwcp.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gnqgboosv.sHtML

[Q83] 大小写转换
来源：http://mobile.fanxiaobao.xyz/Article/details/gxjeuleoz.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/glmwshboz.sHtML

[Q84] 去除首尾空格
来源：http://blog.fanxiaobao.xyz/Article/details/gmuacggzt.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gctrfrdnw.sHtML

[Q85] 数值取整
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmscituyb.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.fanxiaobao.xyz/Article/details/gddzdceqq.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.fanxiaobao.xyz/Article/details/grmithuyv.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.fanxiaobao.xyz/Article/details/gigbmvvxm.sHtML

[Q87] JSON 字段做条件
来源：http://wap.fanxiaobao.xyz/Article/details/gqajhjscz.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wap.fanxiaobao.xyz/Article/details/gspzgpkha.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.fanxiaobao.xyz/Article/details/gidsdboqf.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.fanxiaobao.xyz/Article/details/ghmasxwok.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gqmxoqakg.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdwnybtut.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.fanxiaobao.xyz/Article/details/gybjvqpln.sHtML

[Q90] 生成序号列
来源：http://blog.fanxiaobao.xyz/Article/details/gpeuttmvw.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxxkhgxsl.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gtedbprcz.sHtML

R. Bash 专题
来源：http://read.share.fanxiaobao.xyz/Article/details/gqzkpyngn.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gqmvvjoes.sHtML

[R01] shebang 与严格模式
来源：http://3g.fanxiaobao.xyz/Article/details/grvexshnw.sHtML

#!/usr/bin/env bash
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghfkfeznl.sHtML

set -euo pipefail
来源：http://blog.fanxiaobao.xyz/Article/details/geiyglxyp.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmdzsdsse.sHtML

name="Tom"; echo "$name"
来源：http://baike.fanxiaobao.xyz/Article/details/grnokaoty.sHtML

[R03] 只读变量
来源：http://3g.fanxiaobao.xyz/Article/details/gcaonzcko.sHtML

readonly PI=3.14
来源：http://mobile.fanxiaobao.xyz/Article/details/gfiggrbca.sHtML

[R04] 位置参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvhujpzfw.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghikfiark.sHtML

[R05] 参数默认值
来源：http://baike.fanxiaobao.xyz/Article/details/gvotmouet.sHtML

name="${1:-default}"
来源：http://mobile.fanxiaobao.xyz/Article/details/glyloryzs.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.fanxiaobao.xyz/Article/details/grulzixdz.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.fanxiaobao.xyz/Article/details/ggttuxnvo.sHtML

[R07] if 判断文件
来源：http://m.share.fanxiaobao.xyz/Article/details/geubnyepg.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.fanxiaobao.xyz/Article/details/gopzvkjfh.sHtML

[R08] 数值比较
来源：http://blog.fanxiaobao.xyz/Article/details/gjuwwgujc.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.fanxiaobao.xyz/Article/details/gaoicyecj.sHtML

[R09] 字符串比较
来源：http://3g.fanxiaobao.xyz/Article/details/geaaaasua.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzcacinrm.sHtML

[R10] 正则匹配
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gozlkdapn.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.fanxiaobao.xyz/Article/details/gcnqblvwy.sHtML

[R11] case 多分支
来源：http://3g.fanxiaobao.xyz/Article/details/gmbrxwylx.sHtML

case "$1" in
来源：http://wap.fanxiaobao.xyz/Article/details/gvjxkbsly.sHtML

start) echo "启动" ;;
来源：http://3g.fanxiaobao.xyz/Article/details/gkkzaephl.sHtML

stop)  echo "停止" ;;
来源：http://baike.fanxiaobao.xyz/Article/details/gqnnbvbpy.sHtML

*)     echo "未知命令" ;;
来源：http://baike.fanxiaobao.xyz/Article/details/gbdluuqso.sHtML

esac
来源：http://baike.fanxiaobao.xyz/Article/details/gqdujboxe.sHtML

[R12] for 遍历文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gxrxgvsgs.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gygudbumt.sHtML

[R13] for 计数循环
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glhqjxgbv.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gspvxvnol.sHtML

[R14] C 风格 for
来源：http://3g.fanxiaobao.xyz/Article/details/glhyehtzc.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/giuonxwdf.sHtML

[R15] while 逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gzmnycmco.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/ggmpluvvt.sHtML

[R16] until 等待条件
来源：http://read.share.fanxiaobao.xyz/Article/details/gwhsitpmr.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.fanxiaobao.xyz/Article/details/ggcpakttb.sHtML

[R17] 数组定义与取值
来源：http://wap.fanxiaobao.xyz/Article/details/gcmcirfwt.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.fanxiaobao.xyz/Article/details/glvavjxlf.sHtML

[R18] 遍历数组
来源：http://m.share.fanxiaobao.xyz/Article/details/glxvrmbvt.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gluvjkcvx.sHtML

[R19] 数组长度
来源：http://blog.fanxiaobao.xyz/Article/details/gigewjktd.sHtML

echo "${#arr[@]}"
来源：http://baike.fanxiaobao.xyz/Article/details/gvhtreocd.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjumbebso.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcdfyjccp.sHtML

[R21] 字符串长度
来源：http://mobile.fanxiaobao.xyz/Article/details/gcbmogwxs.sHtML

echo "${#s}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gfluiuvgx.sHtML

[R22] 截取子串
来源：http://blog.fanxiaobao.xyz/Article/details/gjigymahi.sHtML

echo "${s:0:5}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gzcjeyixh.sHtML

[R23] 字符串替换
来源：http://blog.fanxiaobao.xyz/Article/details/gixboztmj.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.fanxiaobao.xyz/Article/details/ghfgcepqm.sHtML

[R24] 大小写转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gauspzvdt.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gsazutdgr.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.fanxiaobao.xyz/Article/details/gpigwqprd.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.fanxiaobao.xyz/Article/details/gzvcbgclx.sHtML

[R26] 命令替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkytzxiap.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.fanxiaobao.xyz/Article/details/gbkrhxuou.sHtML

[R27] 算术展开
来源：http://blog.fanxiaobao.xyz/Article/details/gimjdfstj.sHtML

echo $((1 + 2 * 3))
来源：http://3g.fanxiaobao.xyz/Article/details/geoutxyzf.sHtML

[R28] 浮点运算
来源：http://www.share.fanxiaobao.xyz/Article/details/gpzsxfhzx.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.fanxiaobao.xyz/Article/details/gozqvlxrk.sHtML

[R29] 定义函数
来源：http://blog.fanxiaobao.xyz/Article/details/gttgkcwtb.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.fanxiaobao.xyz/Article/details/gktadllbp.sHtML

[R30] 函数返回状态码
来源：http://read.share.fanxiaobao.xyz/Article/details/gbjbrkzti.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.fanxiaobao.xyz/Article/details/gpubhaijk.sHtML

[R31] 局部变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gnzwhedoc.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gltwzjzuf.sHtML

[R32] 参数个数校验
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpzicjnhx.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.fanxiaobao.xyz/Article/details/ggprypudu.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.fanxiaobao.xyz/Article/details/gxrgmionr.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.fanxiaobao.xyz/Article/details/gsrqzvyoj.sHtML

[R34] 退出时清理
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcnurgqti.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fanxiaobao.xyz/Article/details/gucfmzhml.sHtML

[R35] 后台执行并等待
来源：http://m.share.fanxiaobao.xyz/Article/details/gtjvldltu.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.fanxiaobao.xyz/Article/details/gfvzpqssz.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gofndtyae.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.fanxiaobao.xyz/Article/details/gbktmsxre.sHtML

[R37] 把输出赋给变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gxcgscjvi.sHtML

files=$(ls -1)
来源：http://3g.fanxiaobao.xyz/Article/details/giruttuex.sHtML

[R38] 管道串联
来源：http://blog.fanxiaobao.xyz/Article/details/glnlimuwt.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjzwyiutd.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gugfakydg.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqjnceiay.sHtML

[R40] 追加写日志
来源：http://read.share.fanxiaobao.xyz/Article/details/gbhydxtpm.sHtML

echo "log" >> out.log
来源：http://mobile.fanxiaobao.xyz/Article/details/gnxtjufmp.sHtML

[R41] 丢弃输出
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzvlupghq.sHtML

cmd >/dev/null 2>&1
来源：http://blog.fanxiaobao.xyz/Article/details/gxwtavnxy.sHtML

[R42] 输入重定向
来源：http://3g.fanxiaobao.xyz/Article/details/gonsebpcf.sHtML

wc -l < a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gckisllrc.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grvuoegga.sHtML

find . -name "*.log" -type f
来源：http://wap.fanxiaobao.xyz/Article/details/gdpvguajv.sHtML

[R44] 按修改时间查找
来源：http://m.share.fanxiaobao.xyz/Article/details/gjwyocrur.sHtML

find . -mtime -7 -type f
来源：http://m.share.fanxiaobao.xyz/Article/details/gxubqxgfe.sHtML

[R45] 批量删除
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzccrfeqf.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.fanxiaobao.xyz/Article/details/gmuawjwje.sHtML

[R46] 递归替换文件内容
来源：http://www.share.fanxiaobao.xyz/Article/details/glumutsfv.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.fanxiaobao.xyz/Article/details/gnnwimlkx.sHtML

[R47] sed 单行替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gltktwctz.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/giaadfiah.sHtML

[R48] awk 取指定列
来源：http://read.share.fanxiaobao.xyz/Article/details/gqyvshcqi.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gablvkbla.sHtML

[R49] awk 带条件
来源：http://3g.fanxiaobao.xyz/Article/details/gjxfagvvh.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gngfekqbr.sHtML

[R50] awk 求和
来源：http://baike.fanxiaobao.xyz/Article/details/glnffjijt.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/geiwujqoz.sHtML

[R51] 排序去重取前几
来源：http://read.share.fanxiaobao.xyz/Article/details/gloixyysy.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.fanxiaobao.xyz/Article/details/gbiqlssst.sHtML

[R52] 统计行数
来源：http://mobile.fanxiaobao.xyz/Article/details/gvwahsoqq.sHtML

wc -l a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/glunvvkhs.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvrhkhbdb.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.fanxiaobao.xyz/Article/details/grmwgmurf.sHtML

[R54] 比较两个文件
来源：http://www.share.fanxiaobao.xyz/Article/details/grzruuefu.sHtML

diff a.txt b.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/ghjgjmnbc.sHtML

[R55] 压缩与解压
来源：http://www.share.fanxiaobao.xyz/Article/details/gemrfrmiz.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.fanxiaobao.xyz/Article/details/gzquzuvja.sHtML

[R56] 远程拷贝
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjefckmru.sHtML

scp file user@host:/path/
来源：http://mobile.fanxiaobao.xyz/Article/details/giskcjrfl.sHtML

[R57] 远程执行命令
来源：http://wap.fanxiaobao.xyz/Article/details/gpsipwacm.sHtML

ssh user@host 'uptime'
来源：http://www.share.fanxiaobao.xyz/Article/details/gfzxnswtd.sHtML

[R58] 下载文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gefqsdahu.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.fanxiaobao.xyz/Article/details/gndjwjkxa.sHtML

[R59] 发 POST JSON
来源：http://mobile.fanxiaobao.xyz/Article/details/gpiynyrze.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.fanxiaobao.xyz/Article/details/gnojotjsi.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.fanxiaobao.xyz/Article/details/gwmzdimwi.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.fanxiaobao.xyz/Article/details/galdidslp.sHtML

[R61] 磁盘占用
来源：http://www.share.fanxiaobao.xyz/Article/details/gkyxykxko.sHtML

df -h;  du -sh *
来源：http://mobile.fanxiaobao.xyz/Article/details/genxbretq.sHtML

[R62] 找最占空间的文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gudxcyfqq.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.fanxiaobao.xyz/Article/details/goakzvklc.sHtML

[R63] 内存与进程
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdvaivchu.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.fanxiaobao.xyz/Article/details/gxauwjvxm.sHtML

[R64] 结束进程
来源：http://read.share.fanxiaobao.xyz/Article/details/ggohuqukk.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.fanxiaobao.xyz/Article/details/gvrnreyrt.sHtML

[R65] 查看端口占用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsfmpeoij.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.fanxiaobao.xyz/Article/details/gmzizrkmk.sHtML

[R66] 定时任务
来源：http://m.share.fanxiaobao.xyz/Article/details/gcubinhcm.sHtML

crontab -e;  crontab -l
来源：http://www.blog.fanxiaobao.xyz/Article/details/grnvgiegk.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.fanxiaobao.xyz/Article/details/gmaoyyiur.sHtML

openssl rand -hex 16
来源：http://baike.fanxiaobao.xyz/Article/details/ghtblnioi.sHtML

[R68] 计算文件校验值
来源：http://baike.fanxiaobao.xyz/Article/details/ggvzxzwxb.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gtptpdwgi.sHtML

[R69] 生成随机密码
来源：http://mobile.fanxiaobao.xyz/Article/details/guypmziez.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.fanxiaobao.xyz/Article/details/gonkfjatb.sHtML

[R70] 时间戳与互转
来源：http://m.share.fanxiaobao.xyz/Article/details/gthvagiou.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.fanxiaobao.xyz/Article/details/gpvjszxps.sHtML

[R71] 日期格式化
来源：http://www.share.fanxiaobao.xyz/Article/details/glznazond.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.fanxiaobao.xyz/Article/details/gsfscowpq.sHtML

[R72] 等待端口就绪
来源：http://wap.fanxiaobao.xyz/Article/details/godbzrjec.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxckqermh.sHtML

[R73] 分割大日志
来源：http://blog.fanxiaobao.xyz/Article/details/gcnagedbg.sHtML

split -l 1000 big.log part_
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnwqltsqm.sHtML

[R74] 批量重命名
来源：http://baike.fanxiaobao.xyz/Article/details/gdjrlsiae.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gfbsrqokk.sHtML

[R75] 导出环境变量
来源：http://wap.fanxiaobao.xyz/Article/details/ggznjilfr.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.fanxiaobao.xyz/Article/details/gzxwikzic.sHtML

[R76] 使用临时文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gaxhxunev.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.fanxiaobao.xyz/Article/details/ginbklxfv.sHtML

[R77] 读取用户输入
来源：http://wap.fanxiaobao.xyz/Article/details/gozqslpwy.sHtML

read -rp "请输入: " ans
来源：http://baike.fanxiaobao.xyz/Article/details/gktakdqry.sHtML

[R78] 交互式菜单
来源：http://m.share.fanxiaobao.xyz/Article/details/gzngbtlak.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gadebhohm.sHtML

[R79] 解析命令行选项
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqqtuokjb.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.fanxiaobao.xyz/Article/details/gigrtevgc.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.fanxiaobao.xyz/Article/details/guskneuob.sHtML

time ./run.sh
来源：http://blog.fanxiaobao.xyz/Article/details/gxfnytpqe.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gmqbsxdiq.sHtML

S. C / C++ 专题
来源：http://m.share.fanxiaobao.xyz/Article/details/gwafholsm.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/glydmsclf.sHtML

[S01] C：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gafbwiqkk.sHtML

#include <stdio.h>
来源：http://wap.fanxiaobao.xyz/Article/details/gbpurcqsg.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.fanxiaobao.xyz/Article/details/gxjgrfngw.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.fanxiaobao.xyz/Article/details/gwxozgsoz.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.fanxiaobao.xyz/Article/details/gchqoxdqu.sHtML

[S03] C：读入整数
来源：http://wap.fanxiaobao.xyz/Article/details/gmminosch.sHtML

int x; scanf("%d", &x);
来源：http://blog.fanxiaobao.xyz/Article/details/gjstiayyg.sHtML

[S04] C：字符串复制
来源：http://blog.fanxiaobao.xyz/Article/details/gvijzqyeu.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.fanxiaobao.xyz/Article/details/gjvsjfsjh.sHtML

[S05] C：字符串长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gdnxedinz.sHtML

strlen(s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpxflabvh.sHtML

[S06] C：字符串比较
来源：http://read.share.fanxiaobao.xyz/Article/details/gxuaaineg.sHtML

strcmp(a, b) == 0
来源：http://read.share.fanxiaobao.xyz/Article/details/gwtqgpqyh.sHtML

[S07] C：数组遍历求和
来源：http://m.share.fanxiaobao.xyz/Article/details/gdfmrhpho.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.fanxiaobao.xyz/Article/details/ganfxgxyn.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtfylujka.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtbbqghmw.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.fanxiaobao.xyz/Article/details/ggqtpgkxy.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.fanxiaobao.xyz/Article/details/gahhrccpe.sHtML

[S10] C：指针与解引用
来源：http://mobile.fanxiaobao.xyz/Article/details/gpihudora.sHtML

int *p = &a;  *p = 5;
来源：http://baike.fanxiaobao.xyz/Article/details/gxjleftvy.sHtML

[S11] C：逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gfjveabqe.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.fanxiaobao.xyz/Article/details/gydzwarkd.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmepvksmm.sHtML

fclose(f);
来源：http://read.share.fanxiaobao.xyz/Article/details/gsaiymdsl.sHtML

[S12] C：写文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gxcattsgo.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.fanxiaobao.xyz/Article/details/gbnndtmvp.sHtML

[S13] C：宏定义
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyejpqzll.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.fanxiaobao.xyz/Article/details/gbmtpzvwd.sHtML

[S14] C：枚举
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guxvqnwni.sHtML


<!-- 参考信息 -->