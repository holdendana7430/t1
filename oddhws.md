代发 wailian999

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2oiiczjys.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2silhrqll.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2dimirbtm.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2wafnopju.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2doylcoly.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2uhkqsqwv.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2rgctbyrh.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2clwnbqdt.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2kykzowrk.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2foigzfdi.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2cdqtvazv.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2chemuwjw.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2jfmnqxvc.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2fsvrsbdz.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2sfjdfrlv.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2gkshqrhj.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2qkjpaats.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2dglnrygu.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2vuuqcsvb.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2bczquwva.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2txoydgaq.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2nzrtazbj.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2ypscxexw.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2yjykcwqz.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2verqxswe.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2qapddkcl.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2taijxeto.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2ncydanil.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2xchhlbep.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2dokijswq.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2slgnrsld.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2vtyzkqps.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2wblovkkd.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2xmzzalue.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2yryvlkdu.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2pjnaooaj.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2gjzshckf.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2casjymqv.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2kmnaydth.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2pdffhkva.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2aaqazmlf.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2pvykenco.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2lelznzpl.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2mgpxbcvl.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2xnsdpane.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2hskjfwaq.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2zublasbh.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2poccbrjh.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ndfqskbv.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2jigpdgnc.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2jloaykfg.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2eubrkklx.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2seyhwyhc.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2gjpvfgtt.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2zwvuogrs.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2jfngkans.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2nbxrjvad.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2hmwhxqjb.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2iqbdjbmu.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2pldabxtp.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2nssiokya.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2qcugbvlk.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2zopwoduf.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2ymilhqxo.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2nscgjvcc.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2sudqdkep.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2smsczgae.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2qexulgkp.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2xnocuwxc.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2afcumgwz.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2pfiweter.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2rglbrohg.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2ynsvivae.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2xvjymakl.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2vkdcthyi.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2hbtrtadp.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2iruanbty.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2gkoqahwn.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2mpjyamcm.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2cmafpdga.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2aqldqpcg.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2rlucyrox.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2bwzgscdq.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2zvlmiuwh.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2bebbbjfa.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2sqqtabtw.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2udyfeneh.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2rzegrkuo.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2anpgzhww.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2hiqwcpjt.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2spctpphm.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2orivcrzj.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2sgspjhmm.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2jafunnpw.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2wccvijrz.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2yqxwgxmj.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2cyaigaek.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2zkxzorza.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2ricgxceq.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2vmjxsfnv.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2ykdqdwmn.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2lpxlpvnl.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2ebefyjym.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2pwkdqcdh.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2jqftpqyk.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ofwdahoq.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2jqiiuycs.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2xmsohvlg.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2ojtgnnaj.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2owpjbwsg.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2upkurcso.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2ounigjer.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2uwdbgsnn.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2wtoesleh.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2axwcpayw.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2aikjekgb.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2jwlfigwv.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2trezsatv.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2xrkqeylc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2trffcusf.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2ogynxdnv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rosnfofy.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2sbdshfmg.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2kqwpgvpr.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2oxvfuano.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2svovbild.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2avcwwydw.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2ekvtpnef.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2ocjoeacr.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2obdqnvdc.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2zjedngma.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2twcfwiuq.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2wsiexogu.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2iumphhtr.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2hawusnxq.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2gaxrujrh.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2lmmbmbhu.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2fwgipknt.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2pfutizqu.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2uzqnuzwl.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2bfabhoxm.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2hsmobvgd.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2ylnbdhtv.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2bajtheyn.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2kzcpdhcm.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2svbptpuy.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2nlaektic.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2bofjmvuh.html

esac
来源：http://www.52xcode.cn/Article/details/gt2pmlledoc.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2xqnqejod.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2bxcrcnhv.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2stkorchf.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2fessstga.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2gjfbjerp.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2thfvjoad.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2meunbdud.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2yijtboxv.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2llqzootl.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2zucftawz.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2vparassa.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2gbsevbwx.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2wfocxjew.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2umqvahqg.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2xbsuqhlb.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2bzebfrgp.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2ovnbopmb.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2hayburue.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2kqxxhtes.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2mhfscqqh.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2vcfvmsbm.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2dtipunvb.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2ronefavw.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2rbbfhjiq.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2yrapkpnh.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2nvllvmdw.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2endorhal.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2nfcfidjo.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2grpbznsi.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2oiyqxqsg.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2zjkhspel.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2mnkzkmms.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2gtcjrkem.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2afokcgvg.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2fildwysu.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2usdvllsb.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2jbovpsee.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2kbpevxhk.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2ltqztklb.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2vdmqlgiq.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2ktlfogrw.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2awppvpto.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2syvapeah.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2yrrfrhab.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2urvczsjd.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2ovtpnzud.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2aokspnag.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2zcrdksks.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2hqbngfbp.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2zxcanjoj.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2gagfsubz.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2uapurasl.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2nbayqymw.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2yjydfupj.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2rthjzccg.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2forvjwdz.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2qbgfjkgx.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2qudzytxc.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2nawqvoaw.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2ebomswqq.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2tykurrdo.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2ymzxpxqj.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2qkdgtbkl.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2eoulpthi.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2ydkzzohj.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2ncsimewv.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2vmfohkla.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2akkxyzzd.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2vpiwcamb.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2komhkixj.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2obrhhwzq.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2fkhcsnak.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2ovgcdyzq.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2czhhrnzb.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2dlqbyuas.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2loynwbaa.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2ztgkpfwx.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2rxnlpbfa.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2wfpuhhtv.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2srnrmmuc.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2hqabmqhp.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2ilulesbu.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2nlmjbgvk.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2ckusatdb.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2zzqxeymw.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2dtepzuwi.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2omopwddy.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2mruivcmv.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2demenpxj.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2qrmfysfc.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2fjsrycqf.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2ncvjheja.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2pqqganxi.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2wmgjhpzc.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2rwjaveva.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2jqokqozf.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2yshnhwrr.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2jxpsvinu.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2jqmtppog.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2kicbjhmg.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2icttpzeu.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2itfipfjx.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2vqcnstqq.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2eujyddeg.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2kslxjoux.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2japgowsw.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2glcpvdfo.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2gncszvpm.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2jovwjqwl.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2calzjnjg.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2wdfsgpbn.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2pdrhqpvw.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2hnchkrag.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2fhxeflyh.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2wrfwugjf.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2eupwujrx.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2qiaqxnbi.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2drwdymwn.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2zdnspzax.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2ezicpyrp.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2yjpigvsx.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2usuflbst.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2pgimbrrx.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2lanvnjas.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2kokmcrbs.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2huadhecd.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2vckbssrm.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2cvoockmu.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2lvwvbfye.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2cqjvdbbn.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2qrxbbgtx.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2zwjacnfi.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2daoihahc.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2drlnghxo.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2krkvspxj.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2imawuktp.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2kggxlmmt.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2pzaojtsd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cmtfuanm.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2gdjrcvjv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zjoyexdz.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2kqkwomam.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2dhxagmrz.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2nhsbplqn.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2mdrdxuxg.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2ngwrlcyd.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2dbxamkor.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2auvlnxek.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2hvempvhk.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2cqsoftlv.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2qhadcftf.html


<!-- 参考信息 -->