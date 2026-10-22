代发 wailian999

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2zfpybrel.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2mvktrdxt.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2dilgjntb.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2qieyhgaj.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2zrfcvpsf.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2cgzhgakd.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2gfdsdfqn.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2xvixlqii.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2uuembcyz.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2kxvlycda.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2cosugevh.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2fkdleids.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2guldkyfk.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2swoaxwqy.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2cumcppsv.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2wxwgsfgq.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2ynifzcdq.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2lzpklmfm.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2eafbugnk.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2lbgwpnhh.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2nnrzxhsa.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2dndiuewm.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2qrhmtrdw.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2bdnijkhx.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2iverpgwp.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2ajfkkrcs.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2cvzhljxu.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2poiloxmw.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2qjpuivqh.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2mxyotumy.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2powsnecq.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2mzolrgvr.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2ichhmooj.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2kskqfrei.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2doyisvul.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2ywxbyblq.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2blymnnzf.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2lugwkqpq.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2avcptvho.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2hbhsbvsl.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2xptzsbxa.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2rrvhdpal.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2xhlerkho.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2tlidfsdd.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2cjmjvudy.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2kmkrxeqs.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2qurerxqt.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2ohsqxvog.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2sbibeday.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2vxoqrghw.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2fpxwrhar.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2vitqnhyi.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2vyyjhmsf.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2hrruysmj.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2xbqkbtgt.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2msbeorbl.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2rorlnbav.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2bjodlwjn.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2baisbgdi.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2negdmuuj.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2mwwtdugc.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2nsthijsw.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2njqixngc.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2pdlnjmhu.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2gwwyfylq.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2ohraxijw.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2qhvbmbzs.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2tpgyrjhf.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2nojrlwoc.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2elcdessh.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2pxwskxvp.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2inidzxgo.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2tqlmmfxc.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2repyktlq.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2wnywsdey.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2xbfvmcyf.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2ekqimext.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2etmvbfff.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2uivjcuoj.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2qvzoklye.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2ikbpwjup.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2wooytqoe.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2hontrycc.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2keyfydcd.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2tgukevxw.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2egelptfq.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2byibfxzc.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2qachairt.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2gocsvwuz.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2jpovlbse.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2uismjalw.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2docsdojx.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2kiokrcyx.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2oqhdamhi.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2xcufawlc.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2mswwwmpt.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2smtprmgh.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2vicufbsp.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2bryxeewe.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2gbtgdfox.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2vxkdlddu.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2leybdncd.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2cqqrwbcp.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2gnbclvyg.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2hspzkleb.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2yvckxwsu.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2jkdnwhkf.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2wrtaamqt.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2dhhjhatg.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2ixmvflyl.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2nqrywubj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2amclhnqz.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2kzzzqeep.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2euoczybu.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2qgixrpxy.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2fdszecak.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2hshvzcdn.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2aahubijp.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2ujtuajty.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2eviuoqis.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2qftioayo.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2zgongbsc.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2ugdzyxza.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2sarkplok.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2mddqffny.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2auiceadl.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2pklwdcnx.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2kninghla.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2mppjtnnr.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2efnkfvbv.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2fufsowch.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2fmdwxclm.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2khezgjng.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2euxhceim.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2eyppkbhh.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2eooptruw.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2yhfexvgp.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2rnnpjami.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2kulsyisz.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2dgvfgirp.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2xcjqmkbg.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2nbdmcpjn.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2kripfmbq.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2qthhyczy.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2ncaqzhuu.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2wcjjshuh.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2oddfhjyt.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2zqrrpbrm.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2yahdnrag.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2ozugwxwa.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2igjnlkav.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2qoakavjh.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2owsdavjq.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2ecbqxdek.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2pshmvjdf.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2ajoqmyvt.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2lugusmjm.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2xftbvwvh.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2fpazamoj.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2bncdiiub.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2osfiixkp.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2cplkkrpn.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2sfxizvmb.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2iqfxevdi.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2dyltpbnm.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2pmesosjy.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2zslbofnc.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2rgdgaalo.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2ztmotetl.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2unqiawvr.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2ewwvgkmu.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2ocybjuex.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2ksicbipq.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2czwazjeh.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2okaeymfv.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2vidxbapx.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2zonixbou.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2igfksvui.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2zgfzrnln.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2wygrbaqd.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2yecqukpe.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2efagjkna.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2kiatmzsd.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2xgkgjkwm.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2bcxkpfws.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2djwizloo.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2ynnnxazb.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2fzmbajtp.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2smoxcceu.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2cltsqwlb.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2sgnbzfvv.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2xfbfgusq.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2vpfabwyk.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2tzyjjfda.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2loflpxhh.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2msazjgxl.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2vnxcluey.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2lotrxlev.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2yzqedykg.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2mimohztk.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2nvdhtiii.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2wzgdfvcp.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2oxyqwmlf.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2wxvepylx.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2rfqkfllx.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2iejobzis.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2biuabxyy.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2frzzokrz.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2docxugyp.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2kysalwvn.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2ozgafbbb.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2jcdrsalk.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ddzcjqzn.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2usqtqkcf.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2eaufcavg.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2xplsbmmd.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2bxehripn.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2vdsejxdn.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2hownzcub.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2qbhcglea.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2dhftokbh.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2jcmjdhmx.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2exbpebmp.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2qpocxbwd.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2muodulhi.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2mhbxmkjx.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2piiymsbf.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2lezvifzx.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2ritfdikx.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2hchxgugw.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2knnytzds.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2vexltrpl.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2ztsgzthc.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2wnhrlndo.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2ytvpdrsg.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2xrfladpp.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2dubzfumy.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2cpklmorl.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2fkthycbu.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2bwstwmmi.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2qhhnpivk.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2qskyybri.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2dtsewyhk.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2tjshrliq.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2lomuvspd.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2fnbaqzjj.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2gsuwniug.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2imxtkrvj.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2lsbzwmdu.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2pspaxelh.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2kumadqvt.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2hxtavkhe.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2fbtarujp.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2ducigeor.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2nbkxkcth.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2uqsevnjy.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2qkbgbpmg.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2qelqqdtr.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2eoeyswkd.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2ebdravwa.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2gfaufrpp.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2vtpuwais.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2ywxoiown.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2xayswdic.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2nyinytfn.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2fypqeywd.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2ntbzpxhf.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2vfxpzspg.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2lmgpxndr.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2cmknnzdo.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2xyyuqffi.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2lhkhwetu.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2tttwttvq.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2aoabelyd.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2ecvfygyj.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2kiardblr.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2bsecctci.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2vzkfzmah.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2xzsxypfx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tpkctsrq.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2clqpjtuu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2iotfgyuw.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2krejyrhd.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2cbxdscoq.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2igvdaons.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2aqhmtvva.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2slyontrg.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2wlpliyvm.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2wptpbaad.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2vuvmoxtz.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2hklbxxjs.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2caqvwlyt.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2iytxznau.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2iqzdkcrn.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2qqakigjt.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2roiqukrc.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2ahttfqcr.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2qtxkxgak.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2bqddgcov.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2jmppzuqr.html


<!-- 参考信息 -->