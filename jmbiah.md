代发 wailian999

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2pcnfnqow.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2rlploblf.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2agqtbvip.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2qrrdnhii.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2vkwwzjye.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2fjeiqcsx.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2jbyltbpl.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2fxqjpvpn.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2oapiyrdu.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2lgdyjkqg.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2pvvuwgig.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2ifewkxmx.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2nzjrgcyr.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2sdkqdtox.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2safyeapw.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2adedqecr.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2nglywmyb.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2jiqlghdx.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2haigpgpn.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2iuufklyk.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2hjgeyjig.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2avdtlyye.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2ljytqrzc.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2yvoymznk.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2kzguivps.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2cimktitd.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2pnhgjhlu.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2qfiikzqp.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2drmbsuhz.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2yfqedjpe.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2waurlkyj.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2vnkcvtwg.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2tybsimyl.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2ajdfhsoi.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2enxwvbcu.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2upvbjzwb.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ymxrvbpx.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2mlyytacy.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2pwzxrjhe.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2junwgwpm.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2yxwugmtf.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2cvadeyrh.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2frpjeamz.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2izrkwqoj.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2qncnlcku.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2tkvlpcyq.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2ofrpdnlb.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2lmqesrov.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2nxrdhvhq.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2vaxpytxn.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2knivhrei.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2yujhszsq.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2quuezcid.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2odlqgkum.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2tnoxtizq.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2uwkpwyuv.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2kdunonbq.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2aezuzbfg.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2rcpxjagy.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2ehpzbdqg.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2ljznvmux.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2ldslzbik.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2vkrrrpln.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2lmznrkof.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2xtuhkogc.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2ilngjdmi.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2uduequmu.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2xjpckeyg.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2urugdgbd.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2evscrqry.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2tdyxzxyg.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2bbldbzmw.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2atqetxhx.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2izjiyyfy.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2mbdgpppv.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2fsbvrxoo.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2mkgsyzta.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2cjhazaqq.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2jpinojqc.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2ycfxmbqo.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2vrodzgqe.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2awebolow.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2rcgmjymw.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2rptstokp.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2cbebzfaf.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2mcqdjgdl.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2crztogpt.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2jclgppzl.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2rydqidhs.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2sntnnivn.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2kpybqvns.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2qnqlqhje.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2xgnnytbc.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2htbfijbt.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2eaajloqw.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2jgupznze.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2lymbrdsz.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2bvzbihlt.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2sdcmjfpg.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2enxisspn.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2thmdezcc.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2zhyqdzjh.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2qxthcnkc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2shsjipdf.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2ayinaxyu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2clqgyoxw.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2rrwjagdi.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2ozvxpvij.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2kfnffinm.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2bbqqbazy.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2qwcqsghk.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2uyvavpgz.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2yjpjxeiq.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2oprttype.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2ckeufneo.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2ainzovek.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2faivilmk.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2qojwzopo.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2mtikseiy.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2rrpuoplg.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2sbknfqce.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2oinwotlq.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2ctydgben.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2eygzmenz.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2jajdcukc.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2rlonjmvw.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2gibrddvw.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2vkeyites.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2aadpluwv.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2bhddftiv.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2khbgldpv.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2ykvjvxsi.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2kxlhnlwf.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2mtqmyehz.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2jtsdmsxo.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2djtbyqjk.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2svdrcpcc.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2qwhwqpug.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2oorfgtai.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2przutzvu.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2aycjptqj.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2ygaxoygc.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2nefkhehl.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2rzbzgovo.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2uodaixks.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2fpojccbb.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2ctxvquxp.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2uynaogcz.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2ixvcyxcb.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2awtzjhhy.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2whzdbjvc.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2dorpdfqg.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2zfvitgen.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2wcgkahgf.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2ozwonohh.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2yfashfkv.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2yrmjigcl.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2tryxhsra.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2vajzdelm.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2rwwrcfyo.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2qixkikgq.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2fktkqtju.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2lyxqrtkk.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2iiksgsqd.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2kkiqctdm.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2mhanqnzg.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2bcguoqlp.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2ozbemadc.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2jbocltcd.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2idbrejog.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2walahikp.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2yqfcskcg.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2tpxpokvg.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2zpmikgyh.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2xmrlxgqz.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2ozhbcfmj.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2wnnwqcxd.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2vaakihdz.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2qqotsiuq.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2xamlfxxz.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2jhzmmlyz.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2hcmbnhiw.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2krvyaizk.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2allxizsz.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2qbzmajmt.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2yjhympsi.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2wzniheim.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2jgaeuqve.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2hqhmnqfj.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2tmbqbcem.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2eqysdmbn.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2gsoifrar.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2bpohgieu.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2kovhcqyd.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2ccrcgomy.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2fwvnwgvl.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2oxydsque.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2qlxamsjx.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2xvbwzsqe.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2zheniwur.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2eedegfnu.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2wqfoqhxc.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2poycaaec.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2vkvrweem.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2zizfaxuq.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2xdoyokxl.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2qpihwerl.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2ttfkawdu.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2ozuggqce.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2ougzdqat.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2vkbhscdo.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2awvjgech.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2onbohckh.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2pcjhewqg.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2uxbztmdo.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2vlfnzicl.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2xueqcwgk.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2tagyvgrf.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2fagmmpkh.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2jcniljhl.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2iemdhser.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2aiuyvrbx.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2xcqiwuqw.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2nzbhsnct.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2llcpglmp.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2hzthwtso.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2bgdxxrtt.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2sddylzqz.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2euanrjmb.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2lrczykml.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2gweeufvv.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2gbplweik.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2mqyanpuo.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2eurwxrwt.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2cjwozrnz.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2vjpeewwy.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2zyqrsaoi.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2pukesvvf.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2fuohfeie.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2gqjpypdu.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2jcwlyvjm.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2wlagqccj.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2tzpfazrh.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2bjxaintq.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2unydkgkt.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2qyaginow.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2pkjlduer.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2qvxjmthq.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2jnvrissb.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2kcslwryt.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2zshjvsrf.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2qpxnzirf.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2zgdsugfh.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2gdksfndx.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2rzlrzttj.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2ivvcfqsh.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2rheunisi.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2kywdcqeh.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2huxtqfga.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2lptzzslo.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2lhkjsxhs.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2kakhirih.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2ikbpzqrs.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2zrqbnwpg.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2ypidvoxj.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2dhdzrcgo.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2nxdriiic.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2aozvdzmj.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2vxsdttii.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2smleufid.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2xuydwiwe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bveeotov.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2merphzoe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nrqiddec.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2nlykpyzo.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2tfeqgwqx.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2nliqhycg.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2qfsrhpli.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2oiroawxn.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2tfekinjf.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2pcmowvld.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2mygseoyp.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2mseikhbt.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2qedjgmds.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2llohwwan.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2narxkmab.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2rxxshwan.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2unmbgsdu.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2yklbqqqb.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2durhitis.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2csfrgraw.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2skaxppzz.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2wszoemur.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2lndzckul.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2rnuysrht.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2koqxaasz.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2zwurlqnb.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2bnkkfvfk.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2ntjcavzx.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2dxmdzwwb.html


<!-- 参考信息 -->