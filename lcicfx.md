代发 wailian999

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2qpqknbjh.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2wtvcpuil.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2nxgvlyeg.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2ytrjqsaq.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2tletbksb.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2snjxyrpy.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2afxnhrfs.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2zyghalkn.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2knzxnwln.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2sslrqavv.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2nbyqbqlh.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2wmauzaei.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2yyrjylar.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2qdywfsbc.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2xlevcwtw.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2wgqdfwii.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2rlmriuef.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2rscrkzvc.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2adayffpy.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2ffzthoxi.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2lfswnzcj.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2abowwrmr.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2nnealdnj.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2sbhakgbo.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2wwicccjs.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2ksdrakkv.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2trvuoyug.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2qjcbzqdp.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2lfnbvuav.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2uwfuvuul.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2otzunmsi.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2bajtvswt.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2afyugesx.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2rbywscps.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2ebpxdcsn.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2vejfgvdb.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2jisroxqc.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2zveeiegc.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2huaribfc.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2abvdjdvj.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2hdkyains.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2sdecufnl.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2sbkrghzb.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2wyhvcyvr.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2nsvllwzi.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2fcvwavbr.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2dlqpdwqq.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2tbavwrbb.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2klpxwewd.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2fhptjbbi.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2cbwlswxd.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2mzouboeu.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2dqxpctej.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2maoessxs.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2lzguggzj.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2xnjazbai.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2kvdhyaub.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2fyhepmbd.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2dxowrufw.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2mindajvq.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2fjeqrchm.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2smygfklc.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2dvxybamq.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2kextmgge.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2mnuhodea.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2xosahzgg.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2cpkvvtwr.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2ikxgghji.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ujcbsjaz.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2ttusajef.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2dzdtuwsp.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2oltemspd.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2nuetwdik.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2vfsqzpet.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2orvilcgv.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2fvhixwed.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2iqolgiwf.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2onijmrdp.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2lzwnmxue.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2jrmuksqu.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2jqynrxlx.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2bhaljoek.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2tiauasys.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2gyrwdvgg.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2xdfzshkl.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2vrtjoojb.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2mydcmjtx.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2zqlsmkwe.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2ajlylyfm.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2tniemxcd.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2wajfujnb.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2jexujpzd.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2caerggeg.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2kdpgtmss.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2borujkyx.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2otgfqozc.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2zplfjimm.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2hfqbqiiu.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2ttuyrmnd.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2bvfzhfkh.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2ivhinwyq.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2nmdfzxtr.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2qmtwotta.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2hwmrgvxl.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2tkbggecy.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2jyudopwd.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2fiylwanz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wjotwaqj.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2kmdhfsil.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xpyyvhsk.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2tdhjckac.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2pygkevkf.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2dnlnjacq.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2ayjcsunk.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2qdhctsab.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2sqrgfhfg.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2ewyljbjh.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2ldyesqkx.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2htukwpkj.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2nmttqcgj.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2vmsjzhfo.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2agvksadh.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2izylqiri.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2azbdkfwm.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2ilrbcrks.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2uucxbcne.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2qrrettbh.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2wjqkmrod.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2qdmpwaxx.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2czwdsibd.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2cffqwama.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2znaoiico.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2agtonrhx.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2kgtcdqwz.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2sujvrfjh.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2pgsftsjr.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2cwrzkvff.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2ilkgjzgf.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2bwwltijz.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2xgctqaxv.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2qbnuwlqi.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2dlhdnkxh.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2yhfkwetq.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2vslvbkgc.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2dxmtgnld.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2ebpwxpxm.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2tkwsqdwv.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2swkcexag.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2ilfmgxwy.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2siqfcowv.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2fggrkzlu.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2nzispgyj.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2vhzcoyal.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2vbioyvty.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2oooxqrbs.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2mwupkldt.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2mtsjkyjp.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2njzgzloi.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2pbxqfemc.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2mtzadnpi.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2juzrktca.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2ohjiynzr.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2ugybjnnm.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2vkguezwb.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2dcxcrrke.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2rsipgdlb.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2ogoapzil.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2chhntefb.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2gojvrhwd.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2icmcnoyc.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2qgxqyoel.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2xklfndjf.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2qyuutjsz.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2epcnujgx.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2sixepiew.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2njdfeoqy.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2tsvlwxuk.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2mfhmofyf.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2ssylvybp.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2hydotcxc.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2ccrgxfxt.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2pkzntfdz.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2gkvmbevl.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2hnoxzbvp.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2mwpgfcpf.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2blrblzhh.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2qtlujpjb.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2gywndrui.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2sxhuvuig.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2xolejocx.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2qpbuiqzo.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2mnvxlhez.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2vtgztjiq.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2cxxpepcw.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2pemgdcwb.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2fxmeojcn.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2crtrlelj.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2ssveqoof.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2twudfrjs.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2ckimhgiy.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2rptipugj.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2xpbvxwgl.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2czpltcip.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2ofifbzmf.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2nmnuyziy.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2knqjuskm.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2bnsdudwf.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2hrhswhue.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2dddtccaa.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2zrrkhfjk.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2zldkozcd.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2hhvogvjg.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2gpgqjxpa.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2lfivztth.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ptypedhr.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2jauciaob.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2creskkwi.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2smfnfcwi.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2klgxbpqe.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2seyfdbkx.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2hrhgkfuj.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2hvjqsgie.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2hsamksai.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2vragvdku.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2xfhwmgzh.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2yneapkcb.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2ahsxjplf.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2zpbsufxc.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2qgrpkgev.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2dampponc.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2xizrczrt.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2ssknwglt.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2hvmtfele.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2qrupvelx.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2uvbvwunt.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2nhxzxzha.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2olvemqwb.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2fcnjftxl.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2wossmxsf.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2jbjofkpx.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2gjkgrren.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2rhzamawf.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2zukvsxwl.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2mkuvjqnf.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2jfrbhljg.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2ndasjopf.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2iqiasygu.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2lapiudxg.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2ldmegnaa.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2xonlyrin.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2skegtfdt.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2yhbqarue.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2dclqyadx.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2sauvgzgq.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2uodgdxxo.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2zeffsrzf.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2irniiylv.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2sivmejpv.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2cwcelomu.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2klpmafwn.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2axmvwalx.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2lwgafshj.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2iqytnbid.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2sixsbipr.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2llsstskn.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2mmxutvju.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2saatgddr.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2cykwavms.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2nygkngiy.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2nxrsqxyr.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2qnueihto.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2vnfwcpnc.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2aoklcqqy.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2muueypjd.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2bcopujbh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2skxhuhaz.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2andqlyuc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gqpwisuv.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2risbgkth.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2chsxszsr.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2kxfzbcsl.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2zckonxne.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2zqdfkbnz.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2fnebgkvr.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2iqrbmzyt.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2jiqevjvi.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2nrrgnito.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2cljtuvlo.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2dtbyqoyg.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2trqxgckn.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2kerqeqzm.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2bclrrkai.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2smosogku.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2tjynacmm.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2fetdbsbv.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2dcxbxkvh.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2gqodynyv.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2tlhobpmf.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2qrnrkbld.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2txvpqqaa.html


<!-- 参考信息 -->