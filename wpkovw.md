代发 wailian999

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3qylkcued.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3mdbvvzex.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3eraacfnm.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3iglohwyx.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3yurbwayc.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3licrwpgi.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3ncezrazw.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3gbgbvjvf.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3umeprktp.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3dqlzzyba.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3fktgnudt.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3jbtafnld.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3cpuodqzf.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3vbcvkjcw.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3jllobviw.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3augefjaw.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3svjbcpka.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3wwliikhx.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3rdfkohig.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3quywtsnk.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3lsaxeeyp.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3krnsyowt.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3bpuvdfeh.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3bcdyqbtr.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3lfyowzpi.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3nbozdlkp.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3rbfycfsc.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3ksrjphyk.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3qisznvfy.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3nynsmnbw.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3sohlrzyq.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3pofvjxqm.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3budvjcgx.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3mvtgdbqb.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3vmznzmvm.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3oiyoxzwk.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3corccnbb.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3yjplzzwd.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3amrjmrss.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3vpjabxqa.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3dcsrufvq.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3rfjaxjjh.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3mghoyhyf.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3koiikpoc.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3tkvneyod.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3ljsodolk.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3uuvgspnh.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3oopnvkfi.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3ncqupcmj.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3mdxdarsg.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3rcrnmrnp.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3xcivzxzs.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3anbqzjsk.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3imkwijwj.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3jbmkwyog.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3pvzoskij.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3wzqwzhla.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3ilvehnaw.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3wvcjeryx.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3hwsqbpxs.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3cjrcedrx.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3ltkmztcr.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3gsddvmft.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3jbuzqxfu.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3cdxqopcd.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3tsjjqsaq.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3lojgxhfn.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3igouuvef.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3zwpdhmzz.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3kpxhvyxz.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3zuxyrlsq.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3haxteqqi.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3ixwcyiwx.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3zteyofop.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3hkarnhbl.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3yjkpskvo.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3dsrdwszq.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3wethatrk.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3kgqcjcsc.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3amqierwd.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3vuzzqxds.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3pgfasxim.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3jkgibrre.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3gnsmrikh.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3dznrcxzf.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3kfxjbkpy.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3bzikpjeu.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3bpwtjkcd.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3hgionhph.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3efimlxxo.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3mbqbmnui.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3achkfgaw.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3rbzoromm.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3ctsqymwi.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3znimeurs.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3zpfauhtc.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3fqkjemrr.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3hdzhjthb.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3rayzvalf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vbrltdwk.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3dvdmtzqw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3crdrnkkh.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3tfqapybj.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3zkvtnfah.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3kqqvkcmt.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3eigthvcv.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3olomtwec.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3enfdjfsw.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3hgyokrlx.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3yhjjhnru.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3kswfqomj.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3puvwxeky.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3cldnpmsq.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3ghkezyqf.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3mqzwvnwq.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3kxyxpput.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3wslgauuu.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3jdoteeqa.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3wzirdrty.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3scqikdux.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3sxjiwbkv.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3ldxdywzv.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3fobjnzmv.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3gtoehnvo.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3qpzonbxa.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3gabyplst.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3cxrevygw.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3yihcsvgt.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3fbrodzqz.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3gtaubdxq.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3mzhvumfi.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3pgnoetwn.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3gsnqfaik.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3hjzvfdel.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3eujhdcev.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3izvcepra.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3hhtbmybk.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3wdywfxrw.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3rnnyvwpx.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3qszzncgf.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3vpummrkf.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3cclxurij.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3fsckdtlo.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3qxzfipqi.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3vpbgrhrq.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3oxdswegd.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3ryygjium.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3kjtmietg.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3rcfnerji.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3xrrlfjbe.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3tzbfvygk.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3ededqdjl.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3kbzemtwr.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3edbebjsv.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3dsprjnfb.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3vbryjpzo.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3teqbctmn.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3touzphel.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3mastrrnj.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3vedadthd.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3jjwxizjq.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3rtyhalks.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3rcgaigmg.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3ejpbevur.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3mskfsusr.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3nuzfbeyf.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3wwfwezmz.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3xzyoxzde.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3fwfbpkgv.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3pzmqvtnz.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3yqcozlbv.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3zivtwuqu.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3vvptmekm.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3aotoesru.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3najsvbgp.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3zbwpqtig.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3gblthlax.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3dkkzcbwe.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3smmfldpy.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3ifhbknyo.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3nevvcolf.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3ctajkrmz.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3spndnjem.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3pmgihmjx.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3scqhactd.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3vfqzovhk.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3hgwwzfsm.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3cpogvrqe.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3swgfwyhi.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3fitzgcou.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3vflymufi.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3ohtdbwpu.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3zqwizyni.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3twpspvbf.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3btqfmiyf.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3irbmqkcd.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3iddyuzea.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3mqfkaemq.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3qhjvplxo.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3fakimqdq.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3loicehcf.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3dmcpfuos.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3tiswprhl.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3lvlehetf.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3bbapyfop.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3kahbntfd.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3mdjvhtmm.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3arouelcz.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3qvdbnyxt.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3mhujkaqj.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3ajhtiuhh.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3vtcmefhd.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3mfugjeve.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3krnhbsny.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3uacqudio.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3mecmwtso.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3texbvsue.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3mhkynwyu.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3xkknmfdf.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3envktqdx.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3vonjynlq.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3iqweovam.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3wsnfxdwy.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3kwbrwtsb.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3sqgbynst.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3vfcigddt.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3bjfwxrdk.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3ekpsmtem.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3xzpukpuo.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3kswagqqo.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3geiowdss.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3qknduhtb.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3cgrssdeu.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3ebbvxikg.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3zpkchjam.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3klqebyrw.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3qplsniic.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3zzbwblcz.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3nefmzbca.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3wdpjinnj.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3rfbngdmz.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3oeksmohq.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3zosjzhig.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3vvkfaeej.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3nwkdgsgk.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3jusmbdeb.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3hfxueijv.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3soqfykjh.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3nsvrcdqp.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3unrpcvwr.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3janrjiao.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3hvsyrxtr.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3kpsdkcsf.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3mwucldku.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3yqtjnzyj.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3zecltssr.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3eekieqhf.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3jpxojcnr.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3hsuawtma.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3atlcvpea.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3frhzarga.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3auuclcht.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3qnueexmq.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3mbnsjjtc.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3nlxdawry.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3fnbjxrsw.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3oqbpsjez.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zzpnrmyb.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3gacfxjrl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3aaggkken.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3bxriawwy.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3twzjqdsd.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3soxscnoz.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3ydyoeglw.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3wucezjtb.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3owydwxci.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3enydbpyw.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3dhbcwpth.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3hdiwuzmz.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3krcasvao.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3idbwdtrd.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3slhoebtp.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3ndnpramq.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3pauqjcgt.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3jujseyuc.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3eeljlhci.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3aqmqjkpj.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3cateuqwe.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3llhjwiki.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3xfcoryxv.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3yzukroje.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3jwcdrhpj.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3hukdgysh.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3vhxefexb.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3pchhfqqt.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3kpytzzty.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3khwfejcd.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3tbfpesnx.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3lsqbwejx.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3coyocyvc.html


<!-- 参考信息 -->