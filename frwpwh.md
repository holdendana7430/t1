代发 wailian999

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2pzhfxzxb.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2yanlodle.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2jfryntge.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2fmflhsdw.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2narzinzo.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2cespsdaj.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2berngvux.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2bfwtpolq.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2yblhdvod.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2dtwvlyiz.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2rixynyqg.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2xsrcwsov.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2kkofoazv.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2hgqahfju.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2xyblnugt.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2gpbsjvas.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2bacmlpcs.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2yrbsadmb.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2tdrynhwl.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2huhdnlqq.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2cgobfvmx.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2uajgucne.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2unawcbde.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2pbxblxha.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2qfpwhbaw.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2lvqssfix.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2iivtfnld.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2ftidoktz.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2ojrazuhf.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2rzpezjci.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2rpdcatvm.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2emohfxmz.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2rudities.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2jpdaxpfz.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2lzkmvoyu.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2flqumjpd.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2chfkbbqd.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2uljxxxxc.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2tzgrendv.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2svomlyyc.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2vdfndwkt.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2gaaevhbh.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2lltukdlz.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2hpvzikml.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2iebgdnfo.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2xeygsoiw.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2vxfbsayv.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2gzycvdnz.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2huhtgmvs.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2qehebwum.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2zzsjavhp.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2culcilze.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2ivjwxhkq.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2fdufjjnv.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2yexjzteo.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2bwdozqzf.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2ipmjajkg.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2finsuawz.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2xzhlhzog.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2iwemdrrl.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2azagrypm.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2jizvpqoj.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2cqcjeegz.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2wqvsutwp.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2oytwlfqd.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2whxvmmoa.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2qcekwxoo.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2perwzsfx.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2sntwbsbd.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2jlixrxbw.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2cjpwhciq.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2elwsfhec.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2mcuivlab.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2eauqujxu.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2tfmiqfnh.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2yjipdoku.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2vxpzidga.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2pwisrhlu.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2mrkdxupe.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2oafuopuu.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2hvvqzwje.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2cuclisfe.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2wqpggmxn.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2hytdpjwq.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2rirkaovn.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2ezacgrbo.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2ilwkuxjm.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2uerugdcn.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2odfjmejw.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2elyxhfaf.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2qjxzwuss.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2bbvduyoa.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2ihnnlscp.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2tofacydb.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2qqmvlhdx.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2fszadggz.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2mjmatoog.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ekbjutaf.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2enmdevpx.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2bhqokepq.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2tspzpvsr.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2qbydhbzv.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2vogmbhci.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2sezmrqil.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2hjlxfibo.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2gmjryvyi.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2ojlcavbo.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2abmlyvqe.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2nhjjoawx.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2ioufkuio.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2fnxqslbe.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2mroisqci.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2nbyvyxto.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2stcbgmut.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2hlrlnkgq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fsukawqb.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2hvwwacer.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cnnmcrqo.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2hothrbzl.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2lgpqwiaw.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2rdjzridz.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2jlworeaw.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2ryyztupn.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2ffprtaey.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2cexdunrj.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2wecwhqoy.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2pmbrrkyo.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2paeiylka.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2fincsjeb.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2idrjfydu.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2avsxuqum.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2ucompggh.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2ebcdrmof.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2qipsfjtb.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2fmxlwgts.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2jacbupnz.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2wbleysop.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2mvbpjuhk.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2ohtgynwl.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2dvcmzaaq.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2idjmqnxg.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2cqwvbngx.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2ckrzqfwi.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2fbinqznm.html

esac
来源：http://www.52xcode.cn/Article/details/gt2tohywpaa.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2weodzqtg.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2wfhuwexf.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2mvidnrip.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2jcxshysu.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2tcgtflnj.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2raifudvy.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2upivrfup.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2fkbnizrz.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2rensuzyy.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2ofetvtqz.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2ecknrnoz.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2eltvjgml.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2jrijeplu.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2sjrjoput.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2wlmjdlbp.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2twsfnmyx.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2xtnsicph.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2wjjiajpe.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2sggmxsej.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2xjfpbjfs.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2laenmads.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2vlubogxx.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2qfwkjqyu.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2sbduhtmy.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2rtolbzaf.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2eatopxot.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2amurxhvp.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2ugodfqtx.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2wecccxcc.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2cjmqdmin.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2nwvkzlkj.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2horuhqvb.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2fxrrgavk.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2bqlvtstp.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2ztheofnk.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2acpsxrsj.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2rekoxema.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2grqzauli.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2uhhgiqhs.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2rztsfndl.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2joynqcvg.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2afdcsnam.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2tlhsuggw.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2pgagrklv.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2myhlabkw.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2rrzpcodg.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2utfbjvri.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2vmrwswum.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2xznjnjrs.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2ktgbkjya.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2pzlwnuai.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2urghmjuq.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2ahohwhdq.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2endndtow.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2rwfyrtuu.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2lvpchjrx.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2zzpiyqai.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2pyurctas.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2fqctrpdu.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2wjxiwsmg.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2annxvuqo.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2ufgyddfw.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2pitqhafb.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2pyldeukp.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2sztbzjfv.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2cuzbzedp.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2lenjsunn.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2yqfupngy.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2dpfybawz.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2hakupjax.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2zffjhmui.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2dqtvjugt.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2yfzesims.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2uzezyogz.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2vobyvnfl.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2hatjkrgb.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2dwapfimc.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2qvfopiwk.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2xvwdqdpf.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2yzrrvuhv.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2yytbqtsp.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2ocreqjbe.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2umdeistt.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2yxdgooiz.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2eetkxweu.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2tuogudri.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2ftolyena.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2mhgayvup.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2hlfgzvrw.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2snemyjwm.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2toravdih.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2nptwmbfb.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2ftxyxxgl.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2emlrnrnn.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2mcgagvuq.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2sbqwhsaa.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2urpdduho.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2yqsfwrux.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2vlsqugdy.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2rxgpnaxm.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2eehodsxw.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2kknrlvcq.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2fggpjxva.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2ousjtmfp.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2ohnvqgzz.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2ehvnobve.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2dhtbcwem.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2kekkrodq.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2dnmffodo.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2xzdjyqba.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2hqwjxtic.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2uiayphrg.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2uqlqybax.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2wheclvoc.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2apcgrllf.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2sfgmqfxm.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2axihqdkp.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2ewoosojj.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2macyknuu.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2xhvohuxu.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2ywhmojxm.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2rhjtfvbd.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2hzzsbccy.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2ehlplcvu.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2lzgwcbqv.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2urwubvrs.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2uqsedfbn.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2plnqkpzo.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2yizvvznv.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2wxnnawst.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2rporxwki.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2rntddvun.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2xexxppqd.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2yqfhkhwx.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2ermxndat.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2ccnyudix.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2okgjbspq.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2gmlymjkm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ksyuyngv.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2libecpvd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xhlovehx.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2rgbleuvz.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2uymkzxkj.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2prdqxqex.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2vjwgigwm.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2dcggucxx.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2jpkediyk.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2jeflzroo.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2krqztzts.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2rbaidstz.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2iflmgsih.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2wagxsvmq.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2vcctewza.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2uhouehfk.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2mtwirvyw.html


<!-- 参考信息 -->