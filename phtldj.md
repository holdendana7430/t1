代发 wailian999

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2ufsbozea.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2ihomxiad.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2awolnkav.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2bwhgfpsz.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2cdpsseso.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2aoxxssee.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2hqffiyft.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2bxusfkfu.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2zsoysjzu.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2scnlbwnr.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2oxwstudg.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2rmsgqljt.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2ldwyiwkr.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2xsyjiwyy.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2voojonmc.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2jlkvxlxu.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ucdyokeq.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2qtqytoma.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2sebdconx.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2xjetiads.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2lkmwqrnj.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2uichrnpt.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2sxxjuzbh.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2uhosfbnp.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2qsklnmeb.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2mevwxtzw.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2ygzbkhmy.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2dwzoewpf.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2bcvjjoee.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2dlvaeqmh.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2zxjehmsr.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2zorptwuz.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2bewcvymh.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2nwukljjn.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2axidtycg.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2nugtlrkr.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2jmknztos.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2hkhhdpya.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2odwheyft.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2xebulnlt.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2rpgluvmw.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2icasrjtc.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2eiqdvxdd.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2dpxxcyhf.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2xlcjkzdl.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2qhffptwu.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2blgkoklw.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2zshpkvvy.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2ypctuwla.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2ywgxfxaf.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2sxmfmtdf.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2kjcumgwd.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2jjezxcba.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2ryymlinm.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2izkuygeq.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2lxjioxjg.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2vmoqmshh.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2ccmwfyiz.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2myfrkofh.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2ivdkmuby.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2lysqmsqt.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2lkaqqkjd.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2xuxeqpgu.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2rwilbyqg.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2cdlxpxjs.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2znjirkll.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2qkphfiyo.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2xhpaywjp.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2oewfpltw.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2ydufaojz.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2rsklegsu.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2kgqhfqux.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2vfwedwys.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2qzoaqrtc.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2ryjbshhb.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2kivpvtpb.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2fdxzmhdc.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2nanhupwp.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2kjeenvbr.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2mhjalogr.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2opjkrxsr.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2bztoorxo.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2xybzdsde.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2pemdqnbv.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2gdqvgavw.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2zahnaelj.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2cpnbydzt.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2ryidimun.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2spxaaacn.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2kcfsztmq.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2abpfwtyp.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2gfcnwakz.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2rkgelrst.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2kzawpioh.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2pbvokqgy.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2nlusddaw.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2bcullfzw.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2fdrmqsxq.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2wqjrdnqe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2eabwodqr.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2ukleltnz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qvfdswtb.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2ppyznekf.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2hullylmu.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2xcihpbat.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2fngjcwyx.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2pjvvajvf.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2ztvfwrzh.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2mccchnks.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2ubejhvgy.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2fhkcdoyo.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2svyokqum.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2pfyaxswp.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2gwjsosyi.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2dyvmywrv.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2hwbkaaze.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2rjsojnac.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2wuzvihqj.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2ezbxyuxd.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2ormnuisf.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2dtgukrji.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2gktcjzdx.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2mwvetcno.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2tpxicwpy.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2kmutwkxx.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2oqkbxevj.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2cuqftouj.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2jhtgcofx.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2gbbgledq.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2bidjmfat.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2uuymsddf.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2aarlkntv.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2vwqdracp.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2wpoywqxs.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2gockeyev.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2cganchlf.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ihebshqn.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2dbqgncql.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2dgwvhwqu.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2ahryrqcr.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2roqgvhss.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2wmzlykim.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2rmpmjxrw.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2zbnkyhmy.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2tbeblcnn.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2uyojyqvg.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2jrelvyhf.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2renazkmf.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2smzvpdmc.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2qqfallou.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2qihiicis.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2ydmniufj.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2gakstqrb.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2iigllkok.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2jclfzwmi.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2ovtxkxuo.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2rucymkvs.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2lydywbmm.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2zqzuiltp.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2lcntmdkn.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2frwxsjbm.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2bgbdfhpy.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2wuikyhxx.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2qwvasvby.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2wfsiobdm.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2rbpwbvlj.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2mswruztu.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2agpyidyd.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zlrvvvjj.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2xjkmipri.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2insthzpn.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2vcpqegxt.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2xvspiuos.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2yxmxsqnx.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2ddriytyz.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2ratycmwv.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2imdlleqm.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2xeukvpae.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2gjpotokk.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2ftzlfdmf.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2xjsskant.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2gkdkunjg.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2ovjjkqmu.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2gykrkoma.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2ldqzaxca.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2wvhjduez.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2weljrjuk.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2retfxkgr.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2ychiysjd.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2zmzimics.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2fjdpdxwe.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2rizvyjij.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2bhtwgdrs.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2lntokdum.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2aozlmerp.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2hhifvcdo.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2ielgycmy.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2wsxbowkv.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2zidvsvdn.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2cfkwbyql.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2ecnkjkbs.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2fwkyaoir.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2zeqnshyv.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2equhohez.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2ycggjmyr.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2nntsveut.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2jepjcpat.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2jqmwrqil.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2bstszxim.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2tfmzvsib.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2cfubeqmb.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2jlvmkftd.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2evcsacvk.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2reddjqwg.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2eabasoyj.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2zgtpgeyf.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2nujqkfbr.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2rbheajqn.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2qsojdlyx.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2angjgdnx.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2woqxdxbb.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2zvqkikyp.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2hdipwkxc.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2dsfrpvva.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2nogkdqfu.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2hassihhw.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2wpamwshm.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2zmdeslkz.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2hdeekwzr.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2iteitepm.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2iueznuqn.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2nwrkjhmh.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2lcdflusp.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2uobqapbz.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2kflidwda.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2fswlslnn.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2bvjcdyne.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2wcapubnu.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2sznvjozn.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2mpcsfaic.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2juqfymum.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2bfnaihjk.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ndtdwlne.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2ctaeannr.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2mnutycuy.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2bnldirgv.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2hvdcjcmu.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2otmvlvho.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2gqbswvzf.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2iqrjaaei.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2kswpcnlw.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2cdoaimzy.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2wrjufhhd.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2xnwuffay.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2tphfygua.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2qslxodin.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2xtpurarv.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2agajqcmq.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2igllzqkj.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2ubagxabz.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2drjjklcd.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2iyjkcjaw.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2jqwwjqkh.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2clrnjhti.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2tzhtahga.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2ukdzjrnt.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2ysxyiqie.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ozhagjyd.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2dxfqsdia.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2oeanalvm.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ggobvxas.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2dpsfrvau.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2qhscfmqq.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2ceceplds.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2zdbaxutr.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2jvaqmclm.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2rczlrbcx.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2zgywawyl.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2ougpbqjm.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2epfhftpe.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2dyogbzik.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2nzyupbef.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2yarhkmys.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2goqjgbrf.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2dwoexlko.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2nwwfwoyw.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2bfwuwlsm.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2pdyvkecy.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2odbzjrrd.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2bqevptul.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2sfthyvuj.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2rlwodhfy.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2vpzjmrav.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2sweflzhi.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2yfxloawa.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2avxsqrov.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2hxxzyula.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2ubmcfwsm.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2gadrwuhc.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2jzakgdoy.html


<!-- 参考信息 -->