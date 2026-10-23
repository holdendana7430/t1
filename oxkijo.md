代发 wailian999

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3jlwrucas.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3rvpqnhxn.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3raaxoedw.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3xewnsohr.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3btlyhunh.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3nhsqmlpz.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3xwkjzwok.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3glmnsvjf.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3cichyopx.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3rmkfnctg.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3rcqnsdci.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3kllhewdx.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3dydmqgdm.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3ugkzsyjd.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3njoaceso.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3engnfxvs.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3dygluuvw.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3aibmsaoj.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3jhxdwgqq.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3kgdyosjh.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3hcmgzhep.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3bhkjaxoc.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3utlxtlnv.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3wrcjwkah.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3qsrycbzs.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3xegnbpbh.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3wtjadhtt.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3lemvpvor.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3fbucwpaq.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3cciesnhx.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3sbwidmvz.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3kupwkvey.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3chbdvsiw.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3lebiuejs.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3tcpekwkd.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3rqvulxjl.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3bljjatpl.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3cqbksmyc.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3hjkihjor.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3jxiajjud.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3imzyftyv.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3uvzpuxeb.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3eppujmzo.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3rhzkhvur.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3arpvbqdv.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3ttzfjtjg.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3jlzttcdr.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3zxomnnhd.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3hqqfntdj.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3wxsyjgzx.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3sjogivln.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3ecokwufm.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3axbdcvoo.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3wfjdumkk.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3dofzyqcl.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3vztvfzho.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3uujmzgzd.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3flymtlge.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3jbqelpfl.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3kvqstrvs.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3yomjcbmm.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3jbpjdmmk.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3wsulfbwx.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3cncbutek.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3cbpykqxv.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3dvfewpmy.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3gidxyitt.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3apyybuzm.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3rqatudob.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3hebknvdh.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3rmaxgirc.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3oduwtujx.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3aeabimda.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3xglpdlwp.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3mfivjwoe.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3czvtezsa.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3drvswthx.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3lelsecrh.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3mcbksisi.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3oefpfwmn.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3nauaaeys.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3txbhbpxm.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3gbkobnxf.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3xmyfpufb.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3kyhfuqnf.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3orfthnng.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3wfpzodaz.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3jarnuyob.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3pwosxwhc.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3mefsylhi.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3nyluuayp.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3qjuapabz.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3swfkcajs.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3xkwwnbvr.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3tdfqpxxe.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3lhcyucjb.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3cbsymure.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3whuvmdei.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3agmzvcje.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tyzjlegn.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3gxkgdoam.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pdusjqqy.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3szvtabwx.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3ewzrdyvy.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3gujhhpjr.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3vopwxbre.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3aszosyfk.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3uvlowcxx.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3iysipptx.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3menxebik.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3omjeifho.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3xfkkvghe.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3noetibue.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3ljifvzhl.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3ewtqstlo.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3jqikshtr.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3mkjtfwmd.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3dgbsbjhx.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3kaihxpic.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3ucwfxbny.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3aocrvcmx.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3soxpjlib.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3xmmnmnrv.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3yicqyhep.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3phzwainn.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3ihfqczwf.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3gtziiowk.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3jxriifch.html

esac
来源：http://www.52xcode.cn/Article/details/gt3dtnccywb.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3mjgergkh.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3veulykku.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3jhmgmqjs.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3rubvzmeg.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3yadgwmal.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3khtytsqd.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3xemdwiew.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ywewpvtr.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3pnckapmy.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3fdvfvglf.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3pxeydzjd.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3otawryeq.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3gdexrnjf.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3ytxsknhr.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3agxzuvfq.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3ivfcwhrr.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3ywsafdic.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3afsvnfmg.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3vckddiui.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3tobgjduk.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3jhzpepcj.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3nplqqluy.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3cqldybhf.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3tpkpplkz.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3dmaaomny.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3znlbhboi.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3vxqhshoa.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3fnikgluq.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3qyxhdiwn.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3qwgfjftf.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3ynxouhzs.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3aaineqci.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3bhholqfh.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3wbtyqzrw.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3lmzxhoue.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3rqgbmrea.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3miuejasx.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3wmbsecpu.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3sjmtxfvg.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3mmictayo.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3uclzxesj.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3gvavgcqv.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3vmyvfzqk.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3yjirccyj.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3luiqunno.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3syrcjexr.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3ixzysglt.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3uqramnjl.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3nvewxwae.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3igenscav.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3wckbapvd.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3xvhtnviz.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3wibwcify.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3nyflvnuh.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3hezghgbq.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3smbxznht.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3eoycyzkx.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3xzcrhuat.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3geahnkvf.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3vbarwqaq.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3xpdjtaiz.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3udicfqqh.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3emshtuds.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3kkuvesqr.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3cxrtlmab.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3zosbthgv.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3plzfjbut.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3gdvpirwa.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3seolqfri.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3dfanjiyi.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3hbagdaju.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3imokfufm.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3abfweotc.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3gosdynab.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3jhbultdd.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3ekwsalbi.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3mijzypjy.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ngjgxtbe.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3tqirbwgg.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3dhkcudxx.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3hypyfsyc.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3dnjhwvbe.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3znrskmpj.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3smnwjldw.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3enxlifsc.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3qgjdofih.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3wnysfuqt.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3wpzakfqj.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3mupgxzla.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3exhziayr.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3aofnypxg.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3gqbehldi.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3nzmxwfzi.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3burpvooe.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3dpcrsotf.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3bjithsss.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3ycecwxlt.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3xcgejybo.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3zwqtlyja.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3nxgofcto.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3syemgudt.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3tylboepm.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3suhrbwdb.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3pbizocan.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3suyggnmy.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3ulwoxgye.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3qcpyngag.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3ltvvfyso.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3pvypiqqu.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3msszercq.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3qckygebb.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3dglzptdl.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3ktrumvib.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ptqdvnpw.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3hdceuput.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3xyyfilhb.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3gvmwyads.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3dllojzpg.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3baswdwrm.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3ryyzpxew.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3zhossqmk.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3qhteyhhs.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3dtkltqfi.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3zucujtpi.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3hujdzeyi.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3xlinaeis.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3pmakiohw.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3sbvuqmhs.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3nzcdegnh.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3atnkaytx.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3atbmoebc.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3zsagtfwr.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3pnikvkrv.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3pseduliq.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3iufrjgoa.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3undlupwv.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3sdmalgmt.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3dnsssqzh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dfsnlqre.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3afepplwc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gizmnpnh.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3mewojzki.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3nucaknoy.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3hvwyckkd.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3acvuvnvc.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3kwuvioen.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3cadrdhvw.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3hymhynyo.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3iimkhhgx.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3vnkdylup.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3iliaqild.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3oigjxnvl.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3mmcuptbj.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3zsyihzpy.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3rjiflfbd.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3fzpqgfld.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3jcdufspb.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3vluxklwa.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3addkldbi.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3itmmrkom.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3zjvvlbfm.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3xtkiidzl.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3anpwduru.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3yiogvjpw.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3sqcgzjiz.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3czuksfqg.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3cyihgafo.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3hexlftll.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3lfbicgkk.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3prudurzu.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3ikmhobna.html


<!-- 参考信息 -->