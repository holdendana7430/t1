代发 wailian999

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3cbxfbnfi.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3aaikryfp.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3lbrqvuif.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3dzyzgtpa.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3sdmpoaty.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3cbaxgxem.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3tixkgtza.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3qqosmpgq.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3ecgyxrpz.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3qvpbshzf.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3hgycuwtn.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3nnotjqtb.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3ebaqqghr.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3lhjtklaa.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3pmewyvmy.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3gxnroolm.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3fwphjhtq.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3mwxucchg.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3ylgdwxaf.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3mrwzdwei.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3qfhphvhj.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3qxtihlpp.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3yuqshzlt.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3waksvejx.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3xhqqegto.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3yaiyjadl.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3krxiktsd.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3ewoiyvxp.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3trvgkkrs.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3xgenvuql.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3msknvsgc.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3tvlctyrb.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3jhghqayw.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3ssdwxlte.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3laruxdyt.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3ztmdosch.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3undthrzm.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3toyvydus.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3fxtgcybe.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3qybmqiwi.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3dhhzqgir.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3rzkxwtbt.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3sehwkxig.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3sideeeov.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3crmbodsm.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3dukczjkv.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3cdmzmvvg.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3kmsdytgp.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3wlvwuzdu.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3hvrrmsbv.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3ewkszrow.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3duqtlxyq.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3faredlaq.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3aebllyau.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3ukaxoufy.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3jobgnaok.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3tycdhxki.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3kenbauar.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3hezkntea.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3pgarnyso.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3ehdetnto.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3uxxqmnbu.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3yhgxprkt.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3fhiuqgai.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3fvtpngjt.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3pnafrpfc.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3dfkecgwc.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3adqwotck.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3xhqzaznj.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3pqivdapb.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3ldegjujf.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3uptbvnyj.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3ituyepdm.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3exasnzuz.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3zjdoetwk.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3wpmpwgjx.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3ioxvhaww.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3exntyjpk.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3xhlwvxfg.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3jowyprad.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3brehwxte.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3xaxwucyv.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3zqvcobmy.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3trxpcvwv.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3pwcziuoq.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3zwxbyrao.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3ucjmowoq.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3itzapgux.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3yzwnqvge.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3rundkgnq.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3xrzkgjxn.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3brzvbhdt.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3ekbdvngq.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3oizjrkpf.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3cdztfvjt.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3ansmnabv.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3ewaoajqd.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3vpdefbev.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3yhitbjdm.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3dpsphgpi.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3otuyqxze.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3qlwfltvk.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3rvcqhvfd.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3ennyokgp.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3ugjklfcd.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3ligarbue.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3dqppltyp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sytlxmoz.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3cqobmgwr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hennmjjx.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3vafnmalx.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3kdykbidx.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3caqxkkfs.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3vivlfqso.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3qqwhtnlb.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3cbuzcviu.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3dgcnbvmg.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3ywsacigw.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3gtccuodd.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3tzmsydbz.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3nydemvla.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3zkzpyays.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3ocvxkppk.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3cmeissjh.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3ydelxkoc.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3rijmyobf.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3tpychdlm.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3hdmiajub.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3ezmhkyat.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3mzuynfyp.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3opvbboeh.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3qplafwom.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3vuibbnpk.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3pmjipdxe.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3jxkzevwf.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3ofiowdub.html

esac
来源：http://www.52xcode.cn/Article/details/gt3vfzjfydk.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3sgemmyul.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3thuhteok.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3seudynnt.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3hjajulfq.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3lccdbgcj.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3toimtgll.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3rwcdchsf.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3gzssrgot.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3ksqywlaf.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3zheatdfr.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3hghhrzqb.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3spwtsiks.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3vkbailgf.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3zbguyncb.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3cbmjklrh.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3kkzpiplz.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3jnkvpzby.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3tfovstzn.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3xzsddvxx.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3hmagwycg.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3uzwoiakp.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3kmctafbx.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3htljlwiu.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3cmqljlmo.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3ymdzjsaf.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3evvchegj.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3lxlcyais.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3qbekotul.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3zetcdnwp.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3dbyotmzt.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3iurbezyl.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3mmlnzlxw.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3qdljxuig.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3cxgdtfev.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3cxznfreh.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3ttzqlsrs.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3uetcgror.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3wtgapaiv.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3dlytowfk.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3murbybpo.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3sglhaahs.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3hqwcqbve.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3raagvlbr.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3bluqvgjr.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3oryjeojw.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3fhedymas.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3iogaygth.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3pilgkocz.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3mzzjnzlp.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3jsvzqnuj.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3hzexwpvk.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3lxdzjjrf.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3vcmwrjef.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3ydpeydpa.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3ksyhdwaw.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3piepitln.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3bnnibfdq.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3dqjgzdcu.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3emglartc.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3isjgzmgi.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3jdlwxrir.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3mdsfhupf.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3xabtzsvb.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3voieggaj.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3gfafppyd.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3yhjnjzpc.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3hkdqofnm.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3osgxmbhg.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3dcwjpwka.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3esudlkib.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3yjdidtmo.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3xoiniyqa.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3dgefyzhv.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3hmvvsytm.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3twyxbfac.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3mqetfuop.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3wtuukacp.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3shqouldd.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3btniqgaw.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3iktlzuum.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3coextzde.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3oqossdpq.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3hqvifcvc.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3yyigdvhk.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3ldfkiqlv.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3mhadhmuo.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3dshmexzj.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3quxtnqfb.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3dggzhvfw.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3mfsxciqo.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3mysmrznh.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3bgwrbqla.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3yogjrouu.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3vevchxrf.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3oezkfxpk.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3tzqguvfx.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3bhdnifiy.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3talgevlq.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3gwqujwkg.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3vtkppyyn.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3hhqnakyx.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3bohofwjr.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3xwpasfqs.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3vcdclbzi.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3beqgfjki.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3kosieqpg.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3hgnybrda.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3cvnagmkf.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3zytudfpy.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3jtdnnhei.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3xrqjgoke.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3aoafcusc.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3zeuztnhn.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ohkeyfck.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3fnqdvjfg.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3qrlzshhf.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3xdaneuip.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3wyokunaw.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3xmjvgukx.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3sonmgmzh.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3qzrjitbi.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3obyiaece.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3aerdxylc.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3tgattbiz.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3zcbeskap.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3nmsbfhkc.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3aqazhcko.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3oylbdgqu.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3crsoesvg.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3hjnwrhxy.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3czltloea.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3quhylemk.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3bsytzdlo.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3jdppcyvg.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3kndxvlay.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3ajhlalqn.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3eklgqjab.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3vttfifxb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sorahigy.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3tkbohsji.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hwhsdyzb.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3brnyrtzy.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3mytepnsf.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3gqsiyyln.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3tvyggtvx.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3scaqfzij.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3gakzkmim.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3cswaswuh.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3qazxjlrr.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3xvxdiibn.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3omuyvjag.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qfocakgq.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3rogfwiyu.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3mmjozyxr.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3bjtjsgkz.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3xmanoorf.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3gjjjcpms.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3shfdukcq.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3aayyygyo.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3lafalvjp.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3yatwfpee.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3syzstyfz.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3emvdssvr.html


<!-- 参考信息 -->