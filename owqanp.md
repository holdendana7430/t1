代发 wailian999

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2alzcieee.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2qppwpbyh.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2erdhdlna.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2jfvepwkj.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2vqjhswde.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2hblsbdvc.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2feunnrxl.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2ndmdcruj.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2rpvmctpi.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2noscrwki.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2mkybtpnk.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2elsmhomy.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2zityehvb.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2nznmrsrc.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2swsbyjjj.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2jdcrdtzk.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2pxnvmbwk.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2dlizgmwa.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2faelbxjz.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2dsftaqtc.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2rqiamiio.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2hltfudqf.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2qwygfouc.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2pnjfayuz.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2figiyvap.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2hxiqzgfy.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2ukijacna.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2eptidkaq.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2agxfzyis.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2exxedylt.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2plzfyhir.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2wiyvfavg.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2getbsqao.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2gpnbhhmm.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2fevsnjow.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2wjulzytn.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2axqlmxlt.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2leaovukq.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2mwbwnjic.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2iuqokvtx.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2rtshansw.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2maqkbsiu.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2etedtpgr.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2fqedcubb.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2hzbixmov.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2zxxwqrea.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2feeyscao.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2dblqxqdo.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2ixjprijj.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2hhvtvcxg.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2jlzsdgng.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2pjvwclcv.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2vmyrvpos.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2xhykfton.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2qexxhhlk.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2kmsmpjtd.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2mihuqfhw.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2axnozlyp.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2wwmlcewt.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2gckndili.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2cdbuoimo.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2szoqwpfz.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2tbpdohqv.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2hywtbwgn.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2fdsnxkrg.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2kvcoeqec.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2rnqbyelz.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2otmowylb.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2yfxslpzp.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2gsyczxtx.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2kokpfknu.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2xjofncdu.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2pheucjsu.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2lgwzzrpo.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2jkmeqhvw.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2edrxweor.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2kgevugny.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2ewihpbso.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2xwvrnznu.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2nicvyphm.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2lkapefaa.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2djsmzqad.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2vkbvpnpg.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2usaweiht.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2vgmlgvkt.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2xmlyahfx.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2obsjfsyn.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2sdggrkok.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2atcwwbbz.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2vpreziyq.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2spbunxrb.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2sozrgjoj.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2nlddwkbe.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2klknxryv.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2ctznvqqf.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2inqnbusb.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2edgoqjur.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2rtldswoc.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2bftviein.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2ctnlpazk.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2rbdipere.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2xqoggdbd.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2urbcijcj.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2joeqnblf.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2zcubonkb.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2fexqmaov.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2uinyibjg.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2ffkgjzpb.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2yhsgmmrb.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2lakdzvxu.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2kagwmdio.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wpdhxomb.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2vawgegkh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fxlckzvz.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2adoqgmtz.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2swfrlpsi.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2vswdvzco.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2fzpvbnzl.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2fflwyirg.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2uejnykwd.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2zywyxnoa.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2abwofkbw.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2vmhgpavl.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2yetrvnuc.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2jllywbbt.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2mmvkuvxk.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2rscxukft.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2impzyysl.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2vviivmxe.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2dcxpjpde.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2spynqxud.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2kohpfsoc.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2ycwhlbyp.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2pqoiuiph.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2yywkchch.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2nhqsnxwu.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2lwmkhvat.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2liualrtf.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2kitivttg.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2pbywncki.html

esac
来源：http://www.52xcode.cn/Article/details/gt2vlgrzkfm.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2goythgwo.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2lsmczvsy.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2uhyolqqg.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2qrwqgaoq.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2xpdcpnji.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2vxcekolq.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2dqqttoau.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ydhtznbc.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2qsjipcfj.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2yednjwtf.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2zvtafqkj.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2gvlsjbdh.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2xeohoxxc.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2foadquwl.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2kerqbubb.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2fgajxwms.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2skkuxzal.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2rszfluxb.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2yawzphcv.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2qxyhipod.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2hshezaha.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2yxwdocph.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2pgomzdxc.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2buvcqibm.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2qgxsmlqz.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2dlrxghhw.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2kpxhxsqw.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2icrqzxlh.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2omwittto.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2nwhquseh.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2ydcstvsw.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2ukuflhoz.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2mbfbllfc.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2fgrqrwky.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2ttkhneab.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2xpjotchp.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2aqlqkznh.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2afntghrc.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2lhuivdfp.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2vidpcbna.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2nmuxfnhx.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2pudhvsjb.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2tggzvxbt.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2zdcxvsgz.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2wlnzuenj.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2uazgznjh.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2vkyrsuvo.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2rqvoeqod.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2drikanlg.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2boppkdvf.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2ucfgmtes.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2pfemkhil.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2bohsmnna.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2zrynptwb.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2vkmoojvf.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2kbmbqejt.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2dkrhialm.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2zaoajtgf.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2jphyqdao.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2kuonydww.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2dlffvxtc.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ywynauuq.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2lyitimdg.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2kglfmsbd.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2ctjrfdzh.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2ddtgsgod.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2fsmfwppy.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2hlgbxjel.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2qwkarjez.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2izfqltdq.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2cscernvz.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2iflntbyt.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2fpxjpula.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2tjwvdivl.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2jxktjtvj.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2pchnoprz.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2jatzayah.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2uerqhwef.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2iwusaexe.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2yuwozkxu.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2buyxnnnh.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2gsmqaqiw.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2jntkvpox.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2twnnmhcw.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2yamydqgu.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2elqhapoz.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2qtykktxf.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2pzdyctby.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2uhqjrszg.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2nkwxppae.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2oodbarke.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2ideevwel.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2woaijcil.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2daeqwbhf.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2vxcbhusk.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2tmwccrlm.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2xbamhynx.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2gnygexql.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2ivizifvx.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2mgiikrek.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2prbxlmpb.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2faotwsfj.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2cvmssxxk.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2guhuciaa.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2aqsrohqy.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2ietjulnn.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2vlizzazk.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2rteajohr.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2ovoqooay.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2vwjoybxt.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2budmcxdr.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2dptqowsf.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2ictxqaai.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2xupsxand.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2uepiuygq.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2izlqwbbc.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2evnejmie.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2vqnaazvj.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2bbposibb.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2iaynsgxg.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2zevzyaed.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2eovsrxtq.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2xfqfsdaf.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2wbwevbxu.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2uispdogw.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2qqsqijqi.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2llszjnsk.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2vdpfkogg.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2kjagsnbl.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2maxwiiap.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2npdcamcv.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2vrfznuqu.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2akgoavxk.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2rdyrjeki.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2uifxgumx.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2ueliblay.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2nfmxjswt.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2ipuvyony.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ilrsciii.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2dpwrczff.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sdswodyx.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2kmgxrnbf.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2etaorjba.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2ifgleqac.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2kauubtap.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2zdzcilrf.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2horwmkxy.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2hqoycnrc.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2bgpxjwte.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2hchtxyre.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2scrvwpnl.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2qutzzuva.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2uxvmoqvf.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2hqjddvos.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2gcflomic.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2vslornxl.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2tgbjtpyy.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2koitshdu.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2kvuqbpie.html


<!-- 参考信息 -->