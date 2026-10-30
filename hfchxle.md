代发 wailian999

[Q44] IN 子查询
来源：http://mobile.hesvh.cn/Article/details/gzxpgxfey.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://m.share.zdbjq.cn/Article/details/gbwjenkzh.sHtML

[Q45] EXISTS 判断存在
来源：http://www.blog.fehbvm.com/Article/details/gqzlopxef.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.zdbjq.cn/Article/details/gueytuegy.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://wap.fehbvm.com/Article/details/gkukeruhw.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.hesvh.cn/Article/details/gauincekc.sHtML

[Q47] 与平均值比较
来源：http://www.m.share.hesvh.cn/Article/details/gsmftufzo.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://read.share.hesvh.cn/Article/details/grflpjnkq.sHtML

[Q48] CTE 公用表表达式
来源：http://baike.fehbvm.com/Article/details/gqygvifrw.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://m.share.zdbjq.cn/Article/details/gifnyqgkd.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://3g.fehbvm.com/Article/details/gwzbmmmqp.sHtML

[Q49] 更新单行
来源：http://wap.hesvh.cn/Article/details/gppfxkfvp.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://blog.fehbvm.com/Article/details/gdediblep.sHtML

[Q50] 批量更新
来源：http://www.blog.fehbvm.com/Article/details/ghsqjglmr.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://baike.zdbjq.cn/Article/details/gfgryfbmo.sHtML

[Q51] 用子查询更新
来源：http://www.blog.hesvh.cn/Article/details/gphgussfn.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.share.hesvh.cn/Article/details/gpjkkmgam.sHtML

[Q52] 删除指定行
来源：http://blog.zdbjq.cn/Article/details/gkmslfsch.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.hesvh.cn/Article/details/gbibdnwcw.sHtML

[Q53] 按条件删除
来源：http://www.blog.zdbjq.cn/Article/details/ggfhmgeyh.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://3g.fehbvm.com/Article/details/gidokatld.sHtML

[Q54] 清空表
来源：http://www.blog.fehbvm.com/Article/details/gbkwpifzf.sHtML

TRUNCATE TABLE logs;
来源：http://baike.zdbjq.cn/Article/details/gftvzcqaa.sHtML

[Q55] 排名（并列占位）
来源：http://blog.fehbvm.com/Article/details/gyjkaesfg.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://m.share.hesvh.cn/Article/details/grzdghssl.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.hesvh.cn/Article/details/gwosaucsz.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://blog.fehbvm.com/Article/details/gujetqzbi.sHtML

[Q57] 行号
来源：http://blog.hesvh.cn/Article/details/ghdjwwyel.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.hesvh.cn/Article/details/gihwbxrpj.sHtML

[Q58] 累计求和
来源：http://baike.fehbvm.com/Article/details/gdxpxdpke.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://3g.hesvh.cn/Article/details/gtdbltuje.sHtML

[Q59] 分组内累计
来源：http://www.share.hesvh.cn/Article/details/gykxxyfdo.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/gmsfmslfn.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.share.hesvh.cn/Article/details/gwlgsvqva.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.m.share.zdbjq.cn/Article/details/gxwpakyox.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.share.hesvh.cn/Article/details/gxpjnxoty.sHtML

[Q61] 移动平均
来源：http://read.share.zdbjq.cn/Article/details/greznxcpn.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.hesvh.cn/Article/details/gmgbgfimt.sHtML

[Q62] 分组占比
来源：http://www.share.fehbvm.com/Article/details/gdxcaeuea.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://m.share.fehbvm.com/Article/details/grpjyukyc.sHtML

[Q63] 开启事务
来源：http://www.share.hesvh.cn/Article/details/gyvcptfjx.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.zdbjq.cn/Article/details/gijlpvegd.sHtML

[Q64] 提交事务
来源：http://www.share.zdbjq.cn/Article/details/gzilyebat.sHtML

COMMIT;
来源：http://3g.zdbjq.cn/Article/details/gyatxjyhf.sHtML

[Q65] 回滚事务
来源：http://m.share.zdbjq.cn/Article/details/gtbkblnel.sHtML

ROLLBACK;
来源：http://m.share.fehbvm.com/Article/details/gtsanvnyf.sHtML

[Q66] 行锁查询
来源：http://www.m.share.zdbjq.cn/Article/details/gohhwfpqh.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.fehbvm.com/Article/details/gcwbhxvta.sHtML

[Q67] 设置隔离级别
来源：http://wap.fehbvm.com/Article/details/gpxfwvejq.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.hesvh.cn/Article/details/gfnznounc.sHtML

[Q68] 保存点
来源：http://3g.hesvh.cn/Article/details/gdmcrkzps.sHtML

SAVEPOINT sp1;
来源：http://m.share.zdbjq.cn/Article/details/gwttkolni.sHtML

ROLLBACK TO sp1;
来源：http://m.share.fehbvm.com/Article/details/gdybmpyoq.sHtML

[Q69] 查看执行计划
来源：http://www.blog.zdbjq.cn/Article/details/gtbsulnzx.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.m.share.zdbjq.cn/Article/details/grjloiinz.sHtML

[Q70] 更新统计信息
来源：http://3g.zdbjq.cn/Article/details/gwjrozcrn.sHtML

ANALYZE TABLE users;
来源：http://baike.hesvh.cn/Article/details/gfwxkgoro.sHtML

[Q71] 查看建表语句
来源：http://blog.hesvh.cn/Article/details/grwmwoqxd.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.fehbvm.com/Article/details/gfupwfege.sHtML

[Q72] 查看索引
来源：http://www.blog.fehbvm.com/Article/details/giqkxnxda.sHtML

SHOW INDEX FROM users;
来源：http://baike.zdbjq.cn/Article/details/gfknwafhp.sHtML

[Q73] 查看表状态
来源：http://www.m.share.fehbvm.com/Article/details/ghqplpcfp.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.zdbjq.cn/Article/details/gsjkribly.sHtML

[Q74] 强制使用索引
来源：http://blog.zdbjq.cn/Article/details/gbrgpmgey.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.fehbvm.com/Article/details/ggqrzvbnu.sHtML

[Q75] 日期格式化
来源：http://m.share.fehbvm.com/Article/details/gybxfiepp.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.hesvh.cn/Article/details/gontrwonw.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.zdbjq.cn/Article/details/gaqiiiqrx.sHtML

[Q76] 按天统计
来源：http://www.blog.fehbvm.com/Article/details/gcrbfgxfh.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.fehbvm.com/Article/details/gwwuprmvc.sHtML

[Q77] 时间加减
来源：http://mobile.fehbvm.com/Article/details/gkzqtixeq.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.share.fehbvm.com/Article/details/gwozrkrmp.sHtML

[Q78] 当前时间
来源：http://3g.fehbvm.com/Article/details/gptrxrsjh.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.fehbvm.com/Article/details/gwaayphha.sHtML

[Q79] 字符串拼接
来源：http://read.share.fehbvm.com/Article/details/gsqbuughm.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.hesvh.cn/Article/details/gggnerkgr.sHtML

[Q80] 字符串截取
来源：http://blog.fehbvm.com/Article/details/gxyufrhwe.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blog.zdbjq.cn/Article/details/gorxmpyxp.sHtML

[Q81] 字符串替换
来源：http://3g.zdbjq.cn/Article/details/gqthlbwxq.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.fehbvm.com/Article/details/gafszsnho.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.fehbvm.com/Article/details/gnuycgulv.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gbcxqnucr.sHtML

[Q83] 大小写转换
来源：http://mobile.fehbvm.com/Article/details/ggbiojami.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.hesvh.cn/Article/details/gsrqpfzuc.sHtML

[Q84] 去除首尾空格
来源：http://mobile.hesvh.cn/Article/details/ghpoyixjw.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gfafweoxy.sHtML

[Q85] 数值取整
来源：http://wap.zdbjq.cn/Article/details/gqivqlykl.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.zdbjq.cn/Article/details/gtxwlsegb.sHtML

[Q86] 读取 JSON 字段
来源：http://www.m.share.fehbvm.com/Article/details/gkvqwocsn.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.hesvh.cn/Article/details/ggmduslul.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.zdbjq.cn/Article/details/gekvvijan.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.zdbjq.cn/Article/details/glplgyobb.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.hesvh.cn/Article/details/gshqwvcai.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.hesvh.cn/Article/details/glbholxst.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.zdbjq.cn/Article/details/gvicedrgh.sHtML

[Q89] 判断表是否存在
来源：http://3g.zdbjq.cn/Article/details/gmmjqjvbx.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.zdbjq.cn/Article/details/gmklthvjw.sHtML

[Q90] 生成序号列
来源：http://www.blog.hesvh.cn/Article/details/gacafibwd.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://3g.zdbjq.cn/Article/details/gjveahmic.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/grebnepyz.sHtML

R. Bash 专题
来源：http://www.share.hesvh.cn/Article/details/gwqexmasf.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gnsifyrqq.sHtML

[R01] shebang 与严格模式
来源：http://www.share.zdbjq.cn/Article/details/gjsyoocgg.sHtML

#!/usr/bin/env bash
来源：http://baike.zdbjq.cn/Article/details/gotetymiu.sHtML

set -euo pipefail
来源：http://wap.fehbvm.com/Article/details/gpwrwlerq.sHtML

[R02] 变量赋值与使用
来源：http://blog.zdbjq.cn/Article/details/gsoxmkwqj.sHtML

name="Tom"; echo "$name"
来源：http://baike.fehbvm.com/Article/details/gcqjoxywv.sHtML

[R03] 只读变量
来源：http://read.share.zdbjq.cn/Article/details/gtzwsusrr.sHtML

readonly PI=3.14
来源：http://baike.hesvh.cn/Article/details/gmjixvzla.sHtML

[R04] 位置参数
来源：http://wap.hesvh.cn/Article/details/gaozfaoxb.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.hesvh.cn/Article/details/ggxkpfxls.sHtML

[R05] 参数默认值
来源：http://baike.fehbvm.com/Article/details/gwjqyswhw.sHtML

name="${1:-default}"
来源：http://wap.hesvh.cn/Article/details/gbbpbvskl.sHtML

[R06] 判断命令是否存在
来源：http://wap.zdbjq.cn/Article/details/gupexnoaf.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.m.share.fehbvm.com/Article/details/gtsvwdpfw.sHtML

[R07] if 判断文件
来源：http://3g.zdbjq.cn/Article/details/gqvzvwmwe.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.fehbvm.com/Article/details/glwojkewc.sHtML

[R08] 数值比较
来源：http://mobile.hesvh.cn/Article/details/gzyquqjwz.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.fehbvm.com/Article/details/gpuzsbjay.sHtML

[R09] 字符串比较
来源：http://wap.zdbjq.cn/Article/details/gtxoipita.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.zdbjq.cn/Article/details/gabupiojl.sHtML

[R10] 正则匹配
来源：http://read.share.fehbvm.com/Article/details/gordzzbts.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.hesvh.cn/Article/details/gatsjignk.sHtML

[R11] case 多分支
来源：http://baike.fehbvm.com/Article/details/gpgkyctom.sHtML

case "$1" in
来源：http://m.share.hesvh.cn/Article/details/gyamtmcyo.sHtML

start) echo "启动" ;;
来源：http://3g.fehbvm.com/Article/details/gllyzquet.sHtML

stop)  echo "停止" ;;
来源：http://m.share.hesvh.cn/Article/details/gqniyrgbf.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.fehbvm.com/Article/details/gjsuixvby.sHtML

esac
来源：http://mobile.zdbjq.cn/Article/details/ggypuveiv.sHtML

[R12] for 遍历文件
来源：http://read.share.fehbvm.com/Article/details/gaofqdevg.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.hesvh.cn/Article/details/gnmehvspe.sHtML

[R13] for 计数循环
来源：http://wap.fehbvm.com/Article/details/gelbzmxxj.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.fehbvm.com/Article/details/gbnphqsdt.sHtML

[R14] C 风格 for
来源：http://wap.fehbvm.com/Article/details/gfuuilzsx.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.zdbjq.cn/Article/details/gmjaocmgi.sHtML

[R15] while 逐行读文件
来源：http://mobile.hesvh.cn/Article/details/gvynmfvgg.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.zdbjq.cn/Article/details/gqmecpsjb.sHtML

[R16] until 等待条件
来源：http://read.share.hesvh.cn/Article/details/gcpiwuwjg.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.fehbvm.com/Article/details/glszwjjub.sHtML

[R17] 数组定义与取值
来源：http://baike.zdbjq.cn/Article/details/gnqkiksub.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.zdbjq.cn/Article/details/gqumrevzu.sHtML

[R18] 遍历数组
来源：http://www.share.zdbjq.cn/Article/details/gxlokehpo.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.hesvh.cn/Article/details/gaednsjxq.sHtML

[R19] 数组长度
来源：http://wap.hesvh.cn/Article/details/gbbuejwsm.sHtML

echo "${#arr[@]}"
来源：http://read.share.hesvh.cn/Article/details/gzfzzwgtv.sHtML

[R20] 关联数组（字典）
来源：http://mobile.hesvh.cn/Article/details/ganjewppd.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.zdbjq.cn/Article/details/gceczptze.sHtML

[R21] 字符串长度
来源：http://wap.hesvh.cn/Article/details/gufqjasjd.sHtML

echo "${#s}"
来源：http://blog.fehbvm.com/Article/details/gpcjlyamw.sHtML

[R22] 截取子串
来源：http://www.blog.hesvh.cn/Article/details/gesipvtps.sHtML

echo "${s:0:5}"
来源：http://blog.fehbvm.com/Article/details/gozhlzezn.sHtML

[R23] 字符串替换
来源：http://m.share.fehbvm.com/Article/details/gpomvlhfy.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.fehbvm.com/Article/details/gwugfuyhq.sHtML

[R24] 大小写转换
来源：http://m.share.zdbjq.cn/Article/details/gyajouzpz.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.fehbvm.com/Article/details/gyjpiqkdb.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.hesvh.cn/Article/details/gbguzycfr.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.zdbjq.cn/Article/details/gjjewtaqy.sHtML

[R26] 命令替换
来源：http://3g.fehbvm.com/Article/details/gditpoxwu.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.hesvh.cn/Article/details/gqgnxlalj.sHtML

[R27] 算术展开
来源：http://blog.hesvh.cn/Article/details/goqgjbnyc.sHtML

echo $((1 + 2 * 3))
来源：http://blog.hesvh.cn/Article/details/gsbsflyrs.sHtML

[R28] 浮点运算
来源：http://mobile.hesvh.cn/Article/details/gilyxovrd.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.hesvh.cn/Article/details/gmkqqyxae.sHtML

[R29] 定义函数
来源：http://wap.fehbvm.com/Article/details/goijcmqxw.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.fehbvm.com/Article/details/gqrsxtjzf.sHtML

[R30] 函数返回状态码
来源：http://blog.hesvh.cn/Article/details/gvtwtpqdb.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.zdbjq.cn/Article/details/ggyhvncmn.sHtML

[R31] 局部变量
来源：http://www.m.share.zdbjq.cn/Article/details/gfyyypnbo.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.zdbjq.cn/Article/details/ghmneyzqg.sHtML

[R32] 参数个数校验
来源：http://www.share.hesvh.cn/Article/details/gbltpospc.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.hesvh.cn/Article/details/grdvqgnlw.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.zdbjq.cn/Article/details/gtjmqyuxc.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.zdbjq.cn/Article/details/gsmlolxjs.sHtML

[R34] 退出时清理
来源：http://3g.zdbjq.cn/Article/details/ggqihazkl.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.hesvh.cn/Article/details/grvanjwrp.sHtML

[R35] 后台执行并等待
来源：http://www.blog.zdbjq.cn/Article/details/gbbnrcqag.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.zdbjq.cn/Article/details/gblkwrsdo.sHtML

[R36] 并发执行多个任务
来源：http://mobile.fehbvm.com/Article/details/gdlmzrvkv.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.hesvh.cn/Article/details/gbehajtgb.sHtML

[R37] 把输出赋给变量
来源：http://3g.fehbvm.com/Article/details/gqlqxwula.sHtML

files=$(ls -1)
来源：http://blog.fehbvm.com/Article/details/grhrhyfwt.sHtML

[R38] 管道串联
来源：http://www.share.fehbvm.com/Article/details/grfgkfwlx.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.hesvh.cn/Article/details/gmogrxhhi.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.hesvh.cn/Article/details/gnbjnsiup.sHtML

cmd > out.log 2>&1
来源：http://blog.fehbvm.com/Article/details/gwghlsemd.sHtML

[R40] 追加写日志
来源：http://read.share.hesvh.cn/Article/details/ggeyfwxvj.sHtML

echo "log" >> out.log
来源：http://m.share.hesvh.cn/Article/details/gvctanmny.sHtML

[R41] 丢弃输出
来源：http://www.m.share.hesvh.cn/Article/details/giqreoppp.sHtML

cmd >/dev/null 2>&1
来源：http://wap.zdbjq.cn/Article/details/gllulcieq.sHtML

[R42] 输入重定向
来源：http://mobile.zdbjq.cn/Article/details/gdeukqoxl.sHtML

wc -l < a.txt
来源：http://www.blog.hesvh.cn/Article/details/gxwqxygfo.sHtML

[R43] 按名字查找文件
来源：http://read.share.fehbvm.com/Article/details/guzqdcxfk.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.zdbjq.cn/Article/details/gydzuujcx.sHtML

[R44] 按修改时间查找
来源：http://www.share.zdbjq.cn/Article/details/ghpdfxpgg.sHtML

find . -mtime -7 -type f
来源：http://blog.hesvh.cn/Article/details/gcewkcugh.sHtML

[R45] 批量删除
来源：http://mobile.hesvh.cn/Article/details/gfejxkgqu.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.fehbvm.com/Article/details/gtyibikri.sHtML

[R46] 递归替换文件内容
来源：http://read.share.fehbvm.com/Article/details/gozowsunm.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.zdbjq.cn/Article/details/gyoounpxw.sHtML

[R47] sed 单行替换
来源：http://read.share.zdbjq.cn/Article/details/gtfvbeqjx.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.hesvh.cn/Article/details/gpwbwoqym.sHtML

[R48] awk 取指定列
来源：http://mobile.zdbjq.cn/Article/details/ggalrxfwr.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.fehbvm.com/Article/details/gnxlhyrvv.sHtML

[R49] awk 带条件
来源：http://3g.hesvh.cn/Article/details/gpyotqyzd.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.hesvh.cn/Article/details/glgxpidjm.sHtML

[R50] awk 求和
来源：http://read.share.hesvh.cn/Article/details/gultdarvj.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gmugklnre.sHtML

[R51] 排序去重取前几
来源：http://read.share.zdbjq.cn/Article/details/glkiviyzp.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.fehbvm.com/Article/details/gbxnwirmm.sHtML

[R52] 统计行数
来源：http://blog.fehbvm.com/Article/details/glfhsmcsw.sHtML

wc -l a.txt
来源：http://wap.hesvh.cn/Article/details/geseaigtb.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.zdbjq.cn/Article/details/gustunrkn.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.zdbjq.cn/Article/details/glftkwrye.sHtML

[R54] 比较两个文件
来源：http://www.share.fehbvm.com/Article/details/gqognajpm.sHtML

diff a.txt b.txt
来源：http://wap.zdbjq.cn/Article/details/gnkzgtsod.sHtML

[R55] 压缩与解压
来源：http://m.share.zdbjq.cn/Article/details/gqbflmcnx.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.hesvh.cn/Article/details/gumluzfpq.sHtML

[R56] 远程拷贝
来源：http://3g.fehbvm.com/Article/details/gvvywfvtm.sHtML

scp file user@host:/path/
来源：http://mobile.hesvh.cn/Article/details/gtdvvajxe.sHtML

[R57] 远程执行命令
来源：http://blog.fehbvm.com/Article/details/gylgrjvlh.sHtML

ssh user@host 'uptime'
来源：http://blog.fehbvm.com/Article/details/gioqioktj.sHtML

[R58] 下载文件
来源：http://mobile.hesvh.cn/Article/details/gzstzauke.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.zdbjq.cn/Article/details/gntdfjyhi.sHtML

[R59] 发 POST JSON
来源：http://read.share.hesvh.cn/Article/details/gcsqmdpic.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.zdbjq.cn/Article/details/glmbulenz.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.zdbjq.cn/Article/details/gxfgdzcge.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.hesvh.cn/Article/details/gyxxdkmrm.sHtML

[R61] 磁盘占用
来源：http://baike.zdbjq.cn/Article/details/gfycvauor.sHtML

df -h;  du -sh *
来源：http://read.share.hesvh.cn/Article/details/gnkwymvzu.sHtML

[R62] 找最占空间的文件
来源：http://3g.hesvh.cn/Article/details/gqzexgioa.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.hesvh.cn/Article/details/gqmhcklce.sHtML

[R63] 内存与进程
来源：http://m.share.fehbvm.com/Article/details/gvcvpfxgr.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.fehbvm.com/Article/details/gkomdiaan.sHtML

[R64] 结束进程
来源：http://blog.zdbjq.cn/Article/details/gitvtbuew.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.fehbvm.com/Article/details/giidxuzno.sHtML

[R65] 查看端口占用
来源：http://m.share.fehbvm.com/Article/details/gewcpopal.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.fehbvm.com/Article/details/gglskyive.sHtML

[R66] 定时任务
来源：http://www.share.zdbjq.cn/Article/details/gulevlwyh.sHtML

crontab -e;  crontab -l
来源：http://m.share.fehbvm.com/Article/details/gkzrplzcp.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.zdbjq.cn/Article/details/gbnathaaj.sHtML

openssl rand -hex 16
来源：http://baike.zdbjq.cn/Article/details/gurjthlrz.sHtML

[R68] 计算文件校验值
来源：http://mobile.zdbjq.cn/Article/details/glxivgfml.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.fehbvm.com/Article/details/gvchdkcrk.sHtML

[R69] 生成随机密码
来源：http://blog.hesvh.cn/Article/details/grtbgpsya.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.fehbvm.com/Article/details/geoatpidd.sHtML

[R70] 时间戳与互转
来源：http://wap.hesvh.cn/Article/details/gsuxohqau.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.hesvh.cn/Article/details/gnigdlrcq.sHtML

[R71] 日期格式化
来源：http://read.share.fehbvm.com/Article/details/grfmcjokm.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.hesvh.cn/Article/details/gglaftvmm.sHtML

[R72] 等待端口就绪
来源：http://baike.fehbvm.com/Article/details/gykoclrgb.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.hesvh.cn/Article/details/gkotuphkh.sHtML

[R73] 分割大日志
来源：http://baike.fehbvm.com/Article/details/gzfbmwmgr.sHtML

split -l 1000 big.log part_
来源：http://baike.hesvh.cn/Article/details/gitmbpxjx.sHtML

[R74] 批量重命名
来源：http://read.share.fehbvm.com/Article/details/gxjwvkjfn.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.zdbjq.cn/Article/details/gccikkcfc.sHtML

[R75] 导出环境变量
来源：http://www.m.share.fehbvm.com/Article/details/gxnxkquaj.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.hesvh.cn/Article/details/gnbbhydsi.sHtML

[R76] 使用临时文件
来源：http://wap.fehbvm.com/Article/details/geqrbgdov.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.hesvh.cn/Article/details/ghcphvgtt.sHtML

[R77] 读取用户输入
来源：http://mobile.zdbjq.cn/Article/details/gyvamshcd.sHtML

read -rp "请输入: " ans
来源：http://www.blog.hesvh.cn/Article/details/gsoksmlkr.sHtML

[R78] 交互式菜单
来源：http://blog.fehbvm.com/Article/details/ghucuroob.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.zdbjq.cn/Article/details/gclxjuluq.sHtML

[R79] 解析命令行选项
来源：http://mobile.hesvh.cn/Article/details/gunlyumbd.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.zdbjq.cn/Article/details/goxxvcyma.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.fehbvm.com/Article/details/gzubcuxbe.sHtML

time ./run.sh
来源：http://baike.zdbjq.cn/Article/details/gslynipgg.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gmorfriwd.sHtML

S. C / C++ 专题
来源：http://www.blog.zdbjq.cn/Article/details/glnmgazjs.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/glgsjtixw.sHtML

[S01] C：Hello World
来源：http://wap.zdbjq.cn/Article/details/getwppemz.sHtML

#include <stdio.h>
来源：http://blog.hesvh.cn/Article/details/gloppdpes.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.fehbvm.com/Article/details/gixwmuluq.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.zdbjq.cn/Article/details/gqzsvukjm.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.zdbjq.cn/Article/details/gxwhlllwf.sHtML

[S03] C：读入整数
来源：http://www.blog.hesvh.cn/Article/details/gaippckuj.sHtML

int x; scanf("%d", &x);
来源：http://www.share.zdbjq.cn/Article/details/ggcewhdxe.sHtML

[S04] C：字符串复制
来源：http://wap.zdbjq.cn/Article/details/giclxteug.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.fehbvm.com/Article/details/gmrhxezxm.sHtML

[S05] C：字符串长度
来源：http://baike.zdbjq.cn/Article/details/gygfhcmfj.sHtML

strlen(s)
来源：http://www.share.hesvh.cn/Article/details/gsyujoxjk.sHtML

[S06] C：字符串比较
来源：http://wap.fehbvm.com/Article/details/gnjdnpoiw.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.zdbjq.cn/Article/details/glpyrqsta.sHtML

[S07] C：数组遍历求和
来源：http://read.share.fehbvm.com/Article/details/gzxyspcrh.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.hesvh.cn/Article/details/gwdpiwmek.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.hesvh.cn/Article/details/gbngaaeuq.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.fehbvm.com/Article/details/gghumhwdn.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.zdbjq.cn/Article/details/ghgoeorky.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.zdbjq.cn/Article/details/gbttadlro.sHtML

[S10] C：指针与解引用
来源：http://www.blog.zdbjq.cn/Article/details/gietrpozn.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.fehbvm.com/Article/details/gqvpcswud.sHtML

[S11] C：逐行读文件
来源：http://blog.hesvh.cn/Article/details/gdtqifjic.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.fehbvm.com/Article/details/gyshwnwiy.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.hesvh.cn/Article/details/goxjziwbl.sHtML

fclose(f);
来源：http://mobile.hesvh.cn/Article/details/gptvvokch.sHtML

[S12] C：写文件
来源：http://www.m.share.zdbjq.cn/Article/details/ghunnbcme.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.zdbjq.cn/Article/details/gdxedcvaw.sHtML

[S13] C：宏定义
来源：http://www.m.share.fehbvm.com/Article/details/gxdjnnpbb.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.fehbvm.com/Article/details/geneszkox.sHtML

[S14] C：枚举
来源：http://www.m.share.hesvh.cn/Article/details/gthsdcbas.sHtML


<!-- 参考信息 -->