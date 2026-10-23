代发 wailian999

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3piccfxac.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3jjrjpgkf.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3lhjvgbhp.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3ljunpeqe.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3qreattwx.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3eajnhcka.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3esqfdbgt.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3wmimqaxa.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3zqtulroz.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3ehqrbxkd.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3awzzgokk.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3nymybfwi.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3cjimlcny.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3tbtqgikj.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3nccdabgj.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3abbmefcu.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3kbztptjg.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3qcgdimlu.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3rypugffq.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3hmzwdoqs.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3iczoumpt.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3izmarmvf.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3wmknsvjb.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3qoqaftmy.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3zoaizpdj.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3pqwxcikz.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3hwinkxfp.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3eftcehxu.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3sqokiszu.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3ymlvxmbr.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3yahdhgaj.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3iksyycvm.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3fgmenjsi.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3mijnnabh.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3piimrgwf.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3wdwzchba.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3hhuibwhm.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3kfxtqlzk.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3hnehtpyv.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3obmfhlwi.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3bmmpvkqd.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3afoulafp.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3zhgmnqiv.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3azjoemcj.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3svijkisv.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3mccwyoqk.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3zihsqdwu.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3scbjwxrn.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3twcdqmro.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3ckadzpuz.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3aapalvce.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3dxvtwhbt.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3fcwrklie.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3sthlfxml.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3bsmfnnbe.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3vbbqahok.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3bogyzjsf.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3qlxanegw.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3ftdjdgus.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3ecqfqose.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ocjukgbw.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3iuiwkorj.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3eattkden.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3kezeapuh.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3yiuqxizs.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3ewmpinuh.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3jzkajmli.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3zkdgeryv.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3pgwwmsyq.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3gowksoei.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3fxyugvoc.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3jgsccdet.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3pfcasehp.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3ydrlgtpk.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3bmjpjqhz.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3hcmitcvr.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3uhatgrfd.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3azolmfkk.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3ooypwiyt.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3eaptnrnh.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3xhnjzgpc.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3bdiyewvw.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3pnaffyom.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3nochlwcr.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3nzvdmejv.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3uuotchzw.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3usulkale.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3xesipqwp.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3gizrsumq.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3vaxzyjzf.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3zliipfwu.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3qhgkwsrh.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3yhafhmll.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3badbarsg.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3iajfvhwr.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3sogyjkfx.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3siecmipw.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3jxoyckkr.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3pzgbixti.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gfrafhwt.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3abolexhe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hkesdaxg.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3pqmtbzrv.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3zkkijnld.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3txkqnxjz.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3vvpbktwm.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3senupuwp.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3gqhbzzab.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3bvrlfbwt.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3efyjpbrx.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3dgjnjddx.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3pyykgcqj.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3xpjufgll.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3mwqgqdcd.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3mydlwjwp.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3rhkoiyyi.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3emasyybx.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3nkgpnxbw.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3pntcjarj.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3fvrmzchi.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3blgrpzrj.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3yglnhymc.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3ihmbiyls.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3aevxvyaj.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3ehrvsymq.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3itmkopki.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3vctifqlt.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3xyyogzll.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3bwouxdlj.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3ztrfctbc.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3zovxpzih.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3gpaacbyu.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3ihlujpbi.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3bkgkvncn.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3oiqxqisw.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3hlutwstt.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ybmbcimp.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3tfforwzr.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3wpnlwuxn.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3nopnlala.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3tbfijgbx.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3lztcoubi.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3yygkqmjw.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3helhtxro.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3qjnvqkmi.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3jzdggzfn.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3cdfiylhj.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3tvfaobqf.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3dzcnpkux.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3mlotvhpl.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3jkihaaqp.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3pvshiksp.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3wycpziwv.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3obnbryrb.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3dzavuytd.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3ydsfcszp.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3tkeztyqc.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3holvtatm.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3tpgfwwdo.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3fsmlmrst.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3houxgbqt.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3xsccfiob.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3eomkqsxj.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3lpbqwhta.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3tzsymzuy.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3nyeohwea.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3iscrtgje.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3ppedtzyl.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3gcrbzswz.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3yxbmntic.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3aorwpsns.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3wadlzpru.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3cmsfafir.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3oxrbaemk.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3evnjaswt.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3ronhpzev.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3wlddmycn.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3waanazjn.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3xvmxhjcs.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3owzawhlp.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3vgrqhkza.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3amfjpgwi.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3rfkngggw.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3utvwevvw.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3mfbzwlvh.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3ppjtfmji.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3taykkxeh.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3aldzkcgb.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3myidyyqk.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3nazaeers.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3jtdzgvbn.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3mzayaxvv.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3lfsmjnua.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3pmvifqmn.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3wyktjlsx.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3mmvwakyp.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3bpsjvhev.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3uounnepg.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3lpbgrauz.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3edgwapkq.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3eifsjttc.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3wdruykjx.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3wefpxbvf.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3mitczaxb.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3roeoafdt.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3tfegmtlc.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3trpgtepy.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3agvrmuwr.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3sgbljhms.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3ovgtawal.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3fwlzfuia.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3cciafcrm.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3uovtlgst.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3xegttlci.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3krhxonmv.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3lkamapvf.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3ejmltebz.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3pmyrvugs.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3voqdfrwe.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3bwortcyf.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3uhivzxpu.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3shqrighj.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3ciworlky.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3kldxorpa.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3dxkwgquu.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3liodlglh.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3etuiywna.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3progyjka.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3qdwhcltn.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3uncyfpms.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3gsiizgvy.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3gzxnsmns.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3qkcdlsgc.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3bulqepto.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3ybppzxze.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3bxiqzzco.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3ltrycxos.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3zinewrmo.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3bjewgnzk.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3jhpeqlkx.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3ewcrzpix.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3aqdoossp.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3tbkuvezh.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3rbpyejzq.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3yhjruxpf.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3ocglhkaj.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3bxxbfelz.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3trqvsdkp.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3ctfcymip.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3zbzaofno.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3deqzidwx.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3memzfbun.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3rvgayjhb.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3zwqxxamz.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3crhliaru.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3scfkkqxp.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3csgsyscy.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3wcqmjlkc.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3wxbwtjoi.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3oxfgnryk.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3amumzkbg.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3yrobfxsd.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3aaisldrk.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3dmvgfbht.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3pezdpsff.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3leutxkff.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3wpizvlds.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ddcuptom.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3rhujhpxc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ulgodahj.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3wkyojvtr.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3gkwmddfl.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3imdbyxpb.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3jpsesbuh.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3fnbngvtt.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3ibiizuao.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3ydchchmw.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3lnpyowhf.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3uftppupj.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3iuzxxivg.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3whhlxfnb.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3qydugpty.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3seshvphh.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3ezwibezd.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3guxpztbd.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3eathfkyl.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3dpxqzcyx.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3bnhjwbev.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3kyxcmlrl.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3jwwwrtmx.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3bjetjgvu.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3dhzmbghg.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3lhfkhjjq.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3ywknmlre.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3kljcpslu.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3edxbxsot.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3tsbvsjir.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3elheaebn.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3clwnbhki.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3ltlppafx.html


<!-- 参考信息 -->