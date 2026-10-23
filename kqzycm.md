代发 wailian999

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3fjteeziy.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3rgmnmusy.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3fjhhvqjt.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3httyyufw.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3cwuqmmuc.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3vevsrhin.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3slmmpunf.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3jsubwxbp.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3ezhnhcxx.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3ymufhkvc.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3gtnskeau.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3stjopwgi.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3yajpmfkq.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3kecqpmhk.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3qphzcald.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3ihmnlhjq.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3aspmeepw.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3zvlbsvhi.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3yjqauwot.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3fcpfbxmp.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3sbkjczqf.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3nllpslcv.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3quabfxfd.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3iizunlbh.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3prmvsehq.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3crpcfycb.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3tfbxzyby.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3xwauaitm.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3qutbsnqo.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3rtshdgfa.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3oxtohein.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3yzxnkjrg.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3tvfgkady.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3hfupfvzg.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3cvmnyzzn.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3pvmnzmqx.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3jftuhiho.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3dpkwmpzm.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3kyfwddyv.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3xljnkvzs.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3fnjapgbc.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3hnlwmtcg.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3xkwlzurw.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3datyxqrs.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3nrcfjjok.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3vupvgxer.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3lwbfyniz.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3ljmtewpr.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3tgipanxp.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3xeierzau.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3qqwbbitt.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3vitwjqhg.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3fmrepdmt.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3dbmsadng.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3eokviyni.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3akgqqwhj.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3voqqjfpe.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3zupwhlcw.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3kjyqngoj.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3dlmsutkl.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3kvffdqtq.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3nwpivnqx.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3mfzqfomk.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3xeawrfvo.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3spuryfoj.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3remvrpgw.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3cbglglns.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3keowrhzo.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3nnvbtzvf.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3npwjxign.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3izscjzjx.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3wnayibkj.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3bkmveyfu.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3taiwncrw.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3xyhovyyg.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3vhwbjcgk.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3ojjtgzgm.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3mkmgyvvg.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3chanadvl.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3nvkwiyaq.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3jjyrpqlz.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3mwujjzbr.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3yjeevctr.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3sohvwery.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3zrjiywko.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3bufqcpyi.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3lqmuvuja.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3dxoyowol.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3ksjwiwqq.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3jsxyanbn.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3qghtzarl.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3ocfmvimb.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3auvcjmij.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3ahbjpany.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3eddngjir.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3hgjvulry.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3oltdocxb.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3azgssnpt.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ccalurbb.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3nsjxguhp.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3eoyvmdts.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3koqpffrq.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3apoorogw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fykokbcy.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3psmizecc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cpbnimdp.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3bipwhbzx.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3cycnvqbw.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3jhmjtinw.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3fogmukat.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3zardkhkl.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3nxnewxva.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3ytfruhtp.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3ivcqsjyx.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3cicqfmfk.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3qnqzfzvd.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3qjyjcztd.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3kursmpqt.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3lypolvvl.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3lzkuoxdp.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3rvikrdxb.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3eixneudo.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3tfvxkoar.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3hmpzypoa.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3bpnafxvz.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3xdnvpobs.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3ecumjydh.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3ehiamjpy.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3rdjdarcg.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3qqylqfdz.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3pvrwgvze.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3matbpvgb.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3egxpptpb.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3johqkdkh.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3ldvpevyb.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3blmrbxbw.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3ysydhgef.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3rorcdjry.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3zsqwzmso.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3fqqnbwmx.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3vfhfjboy.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3ssnzaboe.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3itcemeos.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3hlyttots.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3fnclkkfk.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3tbevbtvw.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3jcmsbvej.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3fynranlz.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3taentgxz.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3ogxuushd.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3vcyzipey.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3ryxqnvom.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3mvmaqkna.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3rgfztwam.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3plthyhlc.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3czlkdtvl.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3nhkugvpe.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3zxvuitld.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3vytrjvlc.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3dytednuk.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3gqwilsvj.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3aanjakuc.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3jjurwbce.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3pmpfwrmb.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3jceiifik.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3ogicphuq.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3sdsdaaco.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3hrphsxgf.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3rflomkzy.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3fdqgtclo.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3cpueympq.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3kzcrazna.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3cdmvqazz.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3uciweeer.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3yxqavktr.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3klyzryml.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3flyxxzzk.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3ctyiccpz.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3owriirnm.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3apbgpwve.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3ojppsuhn.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3mjmkkdoh.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3evnbfnow.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3fnawmvld.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3qsedmghh.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3cvbgyheq.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3ybrsvaio.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3ujpddmth.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3kuqkbesf.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3fasnmagk.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3teevmanh.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3jhywvyiw.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3wbdoicdq.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3wpwcczrd.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3dfxmzopw.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3kmjnqqys.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3excvndsj.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3mtdiizue.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3jdzmdvlg.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3tandbphb.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3piskuilq.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3eiehtmwu.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3mpvbcknh.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3khxjdxud.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3tbyxmfdd.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3dznmgerw.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3qhueosua.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3pdtrlofw.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3ldrqbbwv.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3bhlbpbzh.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3enokmxpq.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3zujsnaml.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3lwznhalx.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3aoeymylr.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3cyhczbmp.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3xhprjwvb.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3ldpcxfgj.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3sphlprlg.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3nuirqorx.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3yrgnnfdk.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3lhzzyjvb.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3bjxedgdq.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3acuqusbv.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3qyvffdee.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3lyjticrv.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3jldznzna.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3covqhkyk.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3ghvqwwjl.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3kfllgnxs.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3jnbytpas.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3jneqypfy.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3yumagnml.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3fxfzcffy.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3jsrqstyi.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3mqjwonap.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3earqulnu.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3esnskycf.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3mdxvfksq.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3oyuocyhf.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3xcuuezic.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3ohkgtrji.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3hptsaudu.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3odkxreig.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3rslrnykp.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3srfdlkod.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3tmneojha.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3uqihkxii.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3ivjlrnpf.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3mdelneiw.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3jpvxpygh.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3rvzhzfmt.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3esufzggf.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3tezxnuzr.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3tksdnisr.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3jamhprsf.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3gtdisqgs.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3nyciwfzl.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3pnelhoag.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3nlemwpah.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3ydcihndb.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3hbcaudxj.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3ljdjvfdf.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3nupwyhwh.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3siuqlyqj.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3fxcajamu.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3xiyodzik.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3qgbzdhtg.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3onbjenjn.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3hmszdifs.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3dxcqjfkf.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3qketavnt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uhrlxxug.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3ylpxlxcb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sulvifnq.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3spldzdkf.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3znvbbqqe.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3duvwuccj.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3mhqlhoep.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3qwoeympp.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3cbkyskvb.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3gedcaxnf.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3bonbxnkv.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3rycwrctq.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3olgsudzw.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3hixtzrvj.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3komlvfqe.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3fzbtdvxb.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3dfqxitdd.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3fwgyrayu.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3aczdpmqh.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3blzjcskz.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3hpescplq.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3nulxicxo.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3yqmtlmhg.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3pkzcnjst.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3castzskd.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3ufnonnqj.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3bpbucibb.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3silcqqcs.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3esturkez.html


<!-- 参考信息 -->