代发 wailian999

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2eysylsoo.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2hkaiptmo.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2mmrgceep.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2jmxszmek.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2hhurnmpz.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2qqdcnhdi.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2zyoqmorr.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2riegzcqo.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2ilncnoku.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2qbqqbusu.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2fziwcnkp.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2hxsifffo.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2jgudxuur.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2mjhfmlop.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2euvlqtub.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2hlzcffqg.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2ldwbxshm.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2tsjyxosz.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2xupvewcz.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2xulrnfuz.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2hvttfofh.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2ilpyulvl.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2cncanelw.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2pxwkftfn.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2pcngkjud.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2qogyqsbx.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2qotosjqc.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2fdlpawyt.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2uytwsadv.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2ttmcvfcn.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2rvsotxce.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2cgayxnnx.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2nicrfnkz.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2jkblnvsj.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2eqwtywos.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2kmcpeksy.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2vblcozkh.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2qxjfjufn.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2xfvqwlrm.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2ccyhsbrg.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2jljvoecx.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2xhioharv.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2vwsoqaen.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2fxtpwxmi.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2yaxoyrzk.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2nxvfanev.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2zjznzcry.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2xdnqhrhf.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2mpkmvamu.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2jpiwvpbf.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2ebtffegc.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2ydxqlufa.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2bvamntsz.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2laxopbsk.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2yivpayjb.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2ufwqnanw.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2ebpmjpwa.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2miszmteb.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2dvtbdujg.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2gcjvuxxd.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2tacgadhp.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2fywxpjkd.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2nzuprdhz.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2ultamraf.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2jppclnil.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2xnnfoxjv.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2oyjkrvtc.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2xmcztwfa.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2hfstcfws.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2oydsflgz.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2qualxtqq.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2crqdoazf.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2xahzczxc.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2aqwrvmfb.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2jgdjnmtb.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2oldwdeyj.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2bqxlelvn.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2hqzobwyi.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2qbgaqhfs.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2obdjemsc.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2mkpajmfk.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2frufftte.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2kkvgqnrk.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2ioqeytbi.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2ftnbqvxq.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2iwghbvax.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2qbprkjpy.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2qrckdhua.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2cwqllntn.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2zwaxfkkk.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2rhmtrshj.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2gtlufzkc.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2jpuytkje.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ytyxzfio.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2dxuwrtfp.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2byudsyql.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2jpntkskm.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ctrywjos.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2vcboeqcq.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2blonspwv.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2mczmluhq.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2coodnqcl.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2yronwbcv.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2ljhsiuzu.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2takotpim.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2yaouwvrn.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2zvvxqjgh.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2vskjcufo.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2fihfgibq.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2lzxgliay.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2cbehmmbd.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2exylpccb.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2angenyry.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2vcbfuehq.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2kiytmaez.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rcukblie.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2itpdcjsc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mtmjnkil.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2mmujojhg.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2avaynezb.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2vujlrilz.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2woqdpjxg.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2rnaaqxgo.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2nalyvyhh.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2yclgdeqb.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2ezyhkrbd.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2cbcamslf.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2mtypypuv.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2noywbzjm.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2lsdshujd.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2ecripusa.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2agzwlift.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2mcmazfuv.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2uysnmxvx.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2scfbhwhk.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2irhusuyn.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2islehwnh.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2yghhwsyy.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2omeeldfy.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2yrwzxkjv.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2tisylwao.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2qppeygdp.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2spqokxod.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2jdktajxl.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2yvxkwyci.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2dpkzzsqx.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2npqszksi.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2aervbaze.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2fwbggilh.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2ynqfejxv.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2kjyergdm.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2ksezvrpf.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2wzbejasg.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2yqrbpgfh.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2tzqbromz.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2ihhgufnh.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2bgrbzglt.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2hgrgilgd.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2tbraoapb.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2jprjaywa.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2uoeahgol.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2kreuiioo.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2outivgyf.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2limjiwqc.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2faltrjzh.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2rltmllot.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2eqoprcth.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2yckklvgw.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2nmxlmrxc.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2frozxayc.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2gcaelelp.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2rvqkcjvb.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2kyccdzza.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2gcspyptz.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2bflssrci.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2sjlrhmfp.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2bkjfsgar.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2xqugfbks.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2nznwrnhj.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2wzsfosnz.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2rhakheaj.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2fluhjaxk.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2yozyrffh.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2dddzfcai.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2yusddniq.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2apcumqgj.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2ilspftpz.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2ibkfcjqe.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2ylkgzdmu.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2lzxegrhp.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2tulhwaih.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2irrgoyiv.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2rmzwwjts.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2onhefgbc.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2fqjfxkis.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2cjaugzht.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2ghbrntyu.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2lfealmkg.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2bcwjxdiz.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2hvzncnxu.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2bagbrmdn.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2zxhuzgsb.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2ckbxwkuj.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2ounyyqhi.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2jgwbsuxp.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2ghokhsqp.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2nmyilwsd.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2ixfwjhfl.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2nvghqsaz.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2cyvkquon.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2tyqqssyt.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2wshfujsn.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2bqdwvmyu.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2ovtmdwbb.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2akpnfsnz.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2wnisulli.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2oeclthai.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2ipkzbafx.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2bfesmymn.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2oxiubxue.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2avqfwnww.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2furujzct.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2sqjtewfj.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2fvwuapqi.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2tclzmlnv.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2yppiajrs.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2wyposhtw.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2umlggwkf.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2eohkexqa.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2bhdukrvd.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2acjwxfgv.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2ixwxrwvh.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2ogzqxgva.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2qkpduokl.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2balhqrji.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2xgjpjfin.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2udqqcmup.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2nfmqabhm.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2ziwwtnff.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2fpmywdyi.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2xvoqipqe.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2lkhecmtl.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2gvjrbgfa.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2jvsseqod.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2szxvopbi.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2ccoiuskt.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2ewdeeawy.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2utlbphcf.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2isdydwfh.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2bgfafroc.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2gidkjnko.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2ioprbilw.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2tgjxsdgm.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2icqexibo.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2acuzkvsi.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2nrnpdfhi.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2modyhkna.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2olmuueyi.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2dwwxuzum.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2seysgmzd.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2vdqlfsnl.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2vgcrlhah.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2jiaynwcf.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2rttwzouk.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2knwnaktf.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2cojcealg.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2pqbmutkg.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2ejtainly.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2zcosxvvu.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2wavkbzmh.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2uomjuvlj.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2picvqsrb.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2klgwcwki.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2tcpnhhnl.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2clmsxezd.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2aufsqvvd.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2jgumysfm.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2yrabpbhy.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2vkvhtble.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2ovdjhdkz.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2irfvkubr.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2wscunqpw.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2kfqpmnoo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jlbuardj.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2puqshwul.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ycjyhmea.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2hhllmqsk.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2gaexyxnz.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2yzrknmdx.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2bbhenzyj.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2gsmwmyra.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2ohhjwmfp.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2fvxszwqg.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2cphxrpbz.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2fehepiom.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2yjhrcrqy.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2wyownmdr.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2cpapumdm.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2snhvpnvy.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2czyavxcz.html


<!-- 参考信息 -->