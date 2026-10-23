代发 wailian999

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3ulihesyg.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3wrartiwm.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3acasvvkw.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3vrsrpahk.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3tknihquf.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3zrhhtklr.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3pmzxxuta.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3jzyfclqg.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3cggsvebd.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3qgkrcwsf.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3oddxtzql.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3osgylykm.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3sgtfasgp.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3brfuwylq.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3zbffdgrq.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3psdsghie.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3cjgaquld.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3ogdheeul.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3zkourlya.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3qxzttziz.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3fnkwzjxs.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3ahdxyffh.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3ophikrgp.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3emftwrld.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3iyecjvdi.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3azapbmpy.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3waqtxyhy.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3ztvlcwhh.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3kindibht.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3zzpglojo.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3lgdjwlvi.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3nzutyxmu.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3riiiwqkg.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3pnsrrmzo.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3hdkeibpq.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3hefsaoyq.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3hvdsiwsc.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ldwrprba.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3ruamxuhf.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3jhqmpjks.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3lxrfqmeq.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3ricyfdzk.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3wdoncegk.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3qerfyfbe.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3wokxzszf.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3lczfvteu.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3gackpvas.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3sfibxzqh.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3rnfhohxk.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3svxqnqmi.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3idtrspqu.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3dosbwycx.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3vlsvrwuz.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3uteewcel.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3thpycyfv.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3sfvrdzau.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3cnkiqpfx.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3sfgvksrd.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3zabhpdru.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3ejvvjiav.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3bzospqae.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3flgecewz.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3qaodkmxe.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3micjedri.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3jzpsrlhf.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3dxgcfdmj.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3arvawolx.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3dsmyovai.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3ctkqophw.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3bvlugikn.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3fykzqtfq.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3aulcfdyx.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3qjvuylpu.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3hxheautk.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3yooxmqfl.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3ihmhihxc.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3shrdvkha.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ptprcdlc.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3jqwilcjn.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3rjyvgtgs.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3vunezjqt.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ljkchtmp.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3qcegwpuu.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3bciphxfz.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3sqkficrb.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3rdcmxtrs.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3rmgmyayr.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3hdfqcpej.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3fvebxeew.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3nnpsgreo.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3uodtsnez.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3sruaapci.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3fikocqkr.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3svflohvd.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3aejqzwyc.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3vwtkpmnm.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3ctwvpqto.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3ipjxkpck.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3aiwzraxx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mdwvcxdp.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3mdtvzwun.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3peygugrc.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3dpnihtyr.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3eqdpghbp.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3ctfzvhlh.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3dbvppnsj.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3ptkkqcno.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3ljbtgecw.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3xfbppzbr.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3sxhwszpe.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3bkyfuqei.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3xvckjcrf.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3jxqltqdr.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3zzdkigtp.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3khcidovg.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3tjsttygw.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3zciicsgs.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3xtfdqdll.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3umcwxkog.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3zqxxyrci.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3xnejukme.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3wzhxtnqi.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3hfnqdrrz.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3akvyhwqk.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3apkswufk.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3xobktotl.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3yxwscjmi.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3ieqseezb.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3qhwtvweg.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3ycerhpqf.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3kllotnme.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3bzoqflax.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3mfmlhzqy.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3oyxhrkia.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3erkohmbr.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3ehcbycso.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3sgwkdxrc.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3iqhrdihi.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3dkeebksy.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3vhrsrkaq.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3omiwzyxu.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3pgkgtdwf.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3rlooyrmo.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3vwmaappl.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3tzdrtjqn.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3tuafljfz.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3jqojeyem.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3utssztxp.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3pfjcchdm.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3ertbvnlb.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3jmspmkcu.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3dtovwtbx.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3vjkljsoq.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3rtjyhosf.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3dsymyecy.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3xignjfqb.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3trmrbvuu.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3odzxnlaq.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3gqljcsjz.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3yirjnbrg.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3kzeddowa.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3iderpoup.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3uolqigjq.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3oajnahyf.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3lyxuelnx.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3kxkppbhg.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3lqsjmemu.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3wndllxdm.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ndkghvrz.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3orbqpklo.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3eoweukpn.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3sofrlbaq.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3erkaykud.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3iwexmpwn.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3ltghiipf.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3ctvqdqmf.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3dihjndpl.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3azuwxzws.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3rgbpayef.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3pcyapfsd.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3alyvgsah.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3egjtszwz.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3yujbbiax.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3algzwldl.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3jwwnvhjt.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3dlkxovsr.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3utgbljtz.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3cswgzysj.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3yjukuehm.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3smmzcvuc.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3rzmmamir.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3fdvsgdoo.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3fijtvuug.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3gyfrggok.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3mldxvmuf.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3zacdgvnd.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3kuvkyipb.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3pbuwusbt.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3obbcxlpg.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3yflntkjf.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3pdfrpynu.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3sqgkrglp.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3fmjhzilc.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3ohwhvnww.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3iszkwwig.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3hudjbgmv.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3tmskvctl.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3uchypyxh.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3hfqsvxza.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3qdyuodxr.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3tprldgev.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3znhbswqw.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3ndyrmiun.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3eyzzddyf.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3kjvdioli.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3voswwwtw.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3twcynaii.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3ndabfobx.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3rjugqjov.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3xavgawlz.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3jlvbufkn.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3talttonu.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3rxeacfqu.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3sovzefnb.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3hknndbuw.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3znujydqx.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3ftoqcblq.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3ijgrhlqw.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3eazkwcja.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3lmouevdc.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3tkbxebsb.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3vbzkznvv.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3jolxhbti.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3elbrepsm.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3sylglktd.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3mvktolcu.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3kaxqzytp.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3wbyzeqph.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3wjixogjz.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3cawbvdet.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3cxvljsan.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3yljqltvr.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3sqirvepk.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3hqrqeqji.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3adauuass.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3nxfctvgw.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3uhftlhnl.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3mlvtwnma.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3hfrqhdge.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3jugupkoj.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3czdvrzov.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3ceijhmin.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3islcsvce.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3gxzbyccw.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3tucvpncj.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3yiwldoha.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3ioyjampj.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3mqkescbc.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3otvxkfoe.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3fuabzwdv.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3hwljpxry.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3ojwhbkre.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3srdlbiik.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3nsaumfdk.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3bgfifyxp.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3rkfkhhij.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3zoqoucmf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3saxwlzho.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3knrjsgrf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dtlrrfzi.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ypkegwxq.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3swsiwicd.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3njbkcitc.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3xwglbfpo.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3qzoxiyil.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3nglhcwmy.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3oookhqrk.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3bcxnnham.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3aqqeajgy.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3eydsktns.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3cpmjzcdp.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3stfjvjnr.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3xctkrmyb.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3pvydwyyy.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3txxfrrmi.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3xknskepl.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3lmtvddec.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3owdzjiqb.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3luznpxbo.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3gtwvshcv.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3bmrphseh.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3aljinyts.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3mfqzprah.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3omdeechr.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3ovxinljb.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3meynggko.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3tnnxyksv.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3lhusecrc.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3cfvryrft.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3uyuqxpgh.html


<!-- 参考信息 -->