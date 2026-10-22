代发 wailian999

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2cmihqxjm.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2oznydafy.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2aswvqpir.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2mrtqdahv.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2zcwvnbaw.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2fkuzsbib.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2iqdrnmvu.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2aathgnvs.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2ngpfwhzc.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2dhkbwyzu.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2zmpxxhpm.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2hoynsdvn.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2fexpbrgj.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2nepwtyft.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2tyqrkgaz.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2edcntwoh.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2zclwdspq.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2valefipp.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2oiogzsim.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2ievksmwm.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2ongunhkk.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2dubsicbg.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2ozqjdcjq.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2qitiwcda.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2cmmqdrrq.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2nremibkm.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2tybdvesm.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2vlkuqcqa.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2trsamlbw.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2xubkoati.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2sbrmprln.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2zkgvcwmj.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2belyhyta.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2sqkxtxfk.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2zhziupwd.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2rwpipupn.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2ppxysvqc.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2hcddenwk.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2kkxcpacr.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2uzlopyxw.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2jpmxrniz.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2moeeiygn.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2hwmhgrol.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2uokhgmpi.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2uftrdies.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2spddzsao.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2olryjzmh.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2cyzwxabe.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2hnvsesei.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2gzqscymu.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2cfemmwhu.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2atoovhmi.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2petoahbd.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2xvuassbp.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2lvjvvppb.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2sfmgdllb.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2kdapquxd.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2iveiyogj.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2dxrnpmtp.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2zlqraieo.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2avhcbuzi.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2aczkeksk.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2pzeopxhr.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2wbjoxkwy.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2nwvnltkf.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2gyxioqvr.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2ogmdrhnc.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2vefugtlk.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2irkntovl.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2xuoqwlfn.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2oxbbenmu.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2wfofvnjk.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ygywpyvp.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2yifwcoql.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2ccccggxg.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2hcfmougy.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2fyhkffeq.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2ccvwllgi.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2dsqhfotx.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2locnozar.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2gapwhnpz.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2oytdykps.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2dbnwmebw.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2wpusravc.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2pjfaidab.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2zlhwvngp.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2mhkdtnhn.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2utkvpnxr.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2miwiouxk.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ccupjomd.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2tvsgaxef.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2smdfbuuh.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2bvsvrfdz.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2uxhhtibq.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2ddpoagil.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2akvryjsb.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2umoqpsor.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2domfacat.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2cykodgqe.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2tftqdhcp.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2ifdkdbhh.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2mdhcnjby.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2movdxnzw.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2xwmtroif.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2govsacra.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2bqawwlrg.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2jimmjdmd.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2avolgnxu.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2htebpdtl.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2lnishjmm.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2hstxjwmv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ppjgylim.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2nljoxfpq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ommplinv.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2yxuiehtr.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2qptcofhi.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2mywueqfg.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2vxgxrzkl.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2ouyfpjny.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2uavyidpz.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2xlkvrakm.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2ikmyyple.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2jnsqejwm.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2wrggpxns.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2axewjvip.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2cirqrgzc.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2ytwebmjo.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2zmlagjpv.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2xuuegxhr.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2dmuxbleb.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2buavlyxj.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2aguvpvzp.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2xdqwabfd.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2qojleuut.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2zbmvipzz.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2lobrqnkx.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2wzdnhskr.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2hevzevpy.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2slcxgqcv.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2kouqecqt.html

esac
来源：http://www.52xcode.cn/Article/details/gt2vrttwhbb.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2nsyucsng.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2ayjktrni.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2daiapuaa.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2tnlhuimr.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2hzfguntn.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2ndvrzmmx.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2kzxfocyd.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2gstfvbxq.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2dlsddmhy.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2srxkvftw.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2icpuifqr.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2rbckuefq.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2kwotkwzc.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2ahacsrcx.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2csskzlmk.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2sgxupbiq.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2ifxuovbg.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2vsdeedgw.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2mtccqdsh.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2wnkkrjdr.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2bbggpyfp.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2bhgsjqyu.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2uwprhkyj.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2ybtbimsp.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2icijzidw.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2ptrpmafc.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2cjqamawa.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2ofveuvfc.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2tnztbyvq.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2wsanrqsd.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2gcykpkzb.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2jfkvwsmn.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2poktnlon.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2xjobwnao.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2jdmslolx.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2ruwanzxk.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2hbmqzrwv.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2ybyvcuhj.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2yfufyzhk.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zekpfnup.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2unubgiii.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2nxpzfsny.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2vfujdpsa.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2palqfnpr.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2uglzynuw.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2kqozvwxp.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2iruomcug.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2fzhjiuxi.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2dtonssyi.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2hbylwopd.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2rzkmmsms.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2gipyiqnd.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2kphmycrm.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2vggkejwn.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2awatdhts.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2jtrvnqqi.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2ogbihjgu.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2aavhshqj.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2gvsnpfwb.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2juooapcb.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2iruaaxum.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2xybzycfc.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2htevwpiy.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2aoklmxys.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2ainzridu.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2qbjeanva.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2eqzjhlgy.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2ujopwudx.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2yecbzdcm.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2wlunlvuh.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2zcwspllv.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2sqnsqhmv.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2zzjyxmuv.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2zdlxzjiv.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2aqrutlvj.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2kfcjmjze.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2eeodauda.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2daiujjbl.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2urgtbmdw.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2ufefhxnw.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2bdgagbel.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2fiwqziaf.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2dixcalyb.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2umyvoqnt.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2rsabhwqc.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2mpugkupe.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2bpnyemjw.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2mbdvukou.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2kniydnpp.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2eybrlaav.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2ejunxqpy.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2sedascgc.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2npebnpuz.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2npuzrzic.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2ragtmknm.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2teockhja.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2dyiiiare.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2xbmtpwsi.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2lyitptce.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2mniciyjj.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2brpqtzry.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2nlainvwv.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2ozxeaioh.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2zfvihtpu.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2lwjcsuzj.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2gllpgdtl.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2kwuxqhph.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2noccvdid.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2fjepiqgd.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2cnbzffjv.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2cbkldxup.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2tncqvmqv.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2cohqoerr.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2qzoyvcdg.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2qtfzjnna.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2bufwjoix.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2wuwhvbvw.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2pnpzdbya.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2vbnnhrlq.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2lqebogei.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2gwqqdehe.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2slhpzuvx.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2caqunnbc.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2cgqqvjkx.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2iyqcnbjy.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2uylrsciq.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2ulqoamlj.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2xfeuukbd.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2rwpfjoyk.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2wgdoqpou.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2myhmgkgt.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2xkxjbqjy.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2okjwddul.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2wqeyvzgo.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2gvegzqfv.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2lnlgbvyh.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2ibhhwfzl.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2pwjslrov.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2onntimsp.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2nyfxddpl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ddzasaec.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2bnmnfyct.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2obcpytqf.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2hpixzxxy.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2hsxyjeyk.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2kmjdqitj.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2ogfbpjgi.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2zqhfbyhl.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2argknnob.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2hqaeklav.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2jdgqxnqc.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2stvkdeeh.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2nzsjitsp.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2isbpsqvm.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2bmzaybhk.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2afqzjwha.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2gzoszpfb.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2twfnylaa.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2shmdeayd.html


<!-- 参考信息 -->